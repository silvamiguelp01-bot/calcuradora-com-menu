# calcuradora-com-menu

while True:
    print("\n=== Calculadora ===")
    print("1 - Somar")
    print("2 - Subtrair")
    print("3 - Multiplicar")
    print("4 - Dividir")
    print("0 - Sair")
    
    opcao = input("Escolha uma opção: ")

    if opcao == "0":
        print("Saindo...")
        break
    if opcao in ["1", "2", "3", "4"]:
        num1 = float(input("Coloque o primeiro numero: "))
        num2 = float(input("Coloque o segundo numero: "))

        if opcao == "1":
            resultado = num1 + num2

        elif opcao == "2":
            resultado = num1 - num2

        elif opcao == "3":
            resultado = num1 * num2

        elif opcao == "4":
            if num2 == 0:
                resultado =  "Error: divisão por zero"
            else:
                resultado = num1 / num2

    print("Resultado", resultado)

else:
    print("Opção invalida")
            
