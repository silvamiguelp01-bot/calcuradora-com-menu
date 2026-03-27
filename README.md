while True: # sempre repetir o codigo
    print('\n=== Calcuradora ===') # nome do bagulho
    print('1 - Somar') 
    print('2 - Subtrair')
    print('3 - Multiplicar')    # as opções
    print('4 - Dividir')
    print('0 - Sair')

    opcao = input('Escolha uma opcão: ') # para escolher uma das opções acima, serve para digitar tambem o 'input'

    if opcao == '0': # caso a opcão seja 0
        print("Saindo...") # ira printar "Saindo..."
        break # e fechar o codigo

    elif opcao in ['1', '2', '3', '4']: # Simplicar, inves de ficar fazendo muito if e elif, mesmsa coisa do de cima caso seja '1' e somar
        num1 = float(input('Digite o primeiro numero: ')) # serve para digitar o numero que você deseja, caso seja um decimal o "float" ira resolver
        num2 = float(input('Digite o segundo numero: '))
    
    if opcao == '1': # aqui ja seria o calculo, caso seja opcão "1" faça num1 e num2 que ja definimos como resultado
        resultado = num1 + num2 
        print('Resultado', resultado) # e depois ele ira printar, sempre coloque o "resultado" ou outro que defina a conta que esta fazendo
    
    elif opcao == '2':
        resultado = num1 - num2 # mesma coisa do outro 
        print('Resultado', resultado)
    
    elif opcao == '3':
        resultado = num1 * num2 # mesma coisa do outro
        print('Resultado', resultado)
    
    elif opcao == '4': 
        if num2 == 0:   # aqui se o num2 for 0 ele vai devolver um print de erro: Não divisivel por zero
            print('Erro: Não divisivel por zero')
        else:
            resultado = num1 / num2   #mesma coisa do outro
            print('Resultado'. resultado)
        
    else: # caso não for vai dar opção invalida
        print("opcão invalida")

