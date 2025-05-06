# Projeto-Introdu-ao
Introdução a programação Wudson
Matheus Oliveira de Camargo Cruz
Giovanni Monteiro
def calculadora():
    print("Calculadora Simples")
    print("Operações disponíveis:")
    print("1. Soma (+)")
    print("2. Subtração (-)")
    print("3. Multiplicação (*)")
    print("4. Divisão (/)")

    operacao = input("Escolha a operação (1/2/3/4): ")
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))

    if operacao == '1':
        resultado = num1 + num2
        operador = '+'
    elif operacao == '2':
        resultado = num1 - num2
        operador = '-'
    elif operacao == '3':
        resultado = num1 * num2
        operador = '*'
    elif operacao == '4':
        if num2 != 0:
            resultado = num1 / num2
            operador = '/'
        else:
            print("Erro: divisão por zero.")
            return
    else:
        print("Operação inválida.")
        return

    print(f"Resultado: {num1} {operador} {num2} = {resultado}")

# Executa a calculadora
calculadora()
