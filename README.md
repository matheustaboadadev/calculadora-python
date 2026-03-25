# calculadora-python


"""
Calculadora Simples em Python
Autor: Matheus Taboada Chibani Rocha
Descrição: Um script básico para realizar operações matemáticas fundamentais.
"""

while True:
    # Menu
    print("\nEscolha a sua operação matemática")
    print("1 - Soma")
    print("2 - Subtração")
    print("3 - Multiplicação")
    print("4 - Divisão")
    print("5 - Sair")

    opcao = input("Digite uma operação matemática :\n")

#Logica do menu

    if opcao == "5":
        print("Programa finalizado")
        break  

    elif opcao in ["1", "2", "3", "4"]:
        primeiro_numero = float(input("Informe o primeiro número:\n"))
        segundo_numero = float(input("Informe o segundo número:\n"))

        if opcao == "1":
            print(f"Resultado da soma: {primeiro_numero + segundo_numero}")

        elif opcao == "2":
            print(f"Resultado da subtração: {primeiro_numero - segundo_numero}")

        elif opcao == "3":
            print(f"Resultado da multiplicação: {primeiro_numero * segundo_numero}")

        elif opcao == "4":
            if segundo_numero == 0:
                print("Erro: Não é possível dividir por zero!")
            else:
                print(f"Resultado da divisão: {primeiro_numero / segundo_numero}")

    else:
        print("Opção inválida! Tente novamente.")
