# calculadora-phyton
Um projeto simples em Phyton feito para praticar lógica.


     choice = input("Escolha uma operação (1/2/3/4): ")

    if choice not in ['1', '2', '3', '4']:
        print("Escolha inválida.")
        return

    try:
        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))
    except ValueError:
        print("Entrada inválida. Use apenas números.")
        return

    if choice == '1':
        print("Resultado:", add(num1, num2))
    elif choice == '2':
        print("Resultado:", subtract(num1, num2))
    elif choice == '3':
        print("Resultado:", multiply(num1, num2))
    elif choice == '4':
        print("Resultado:", divide(num1, num2))

     if __name__ == "__main__":
    main()
