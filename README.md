# calculadora-phyton
Um projeto simples em Phyton feito para praticar lógica.

operacao = input('Escolha uma operação: (adição/multiplicação/subtração/divisão): ').strip().lower()

# Lista de operações válidas
operacoes_validas = {'adição', 'multiplicação', 'subtração', 'divisão'}

if operacao not in operacoes_validas:
 ração inváli   print('Opeda.')
else:
    try:
        nu1 = float(input('Digite o primeiro número: '))
        nu2 = float(input('Digite o segundo número: '))
        
        if operacao == 'adição':
            resultado = nu1 + nu2
        elif operacao == 'subtração':
            resultado = nu1 - nu2
        elif operacao == 'multiplicação':
            resultado = nu1 * nu2
        elif operacao == 'divisão':
            if nu2 == 0:
                print("Erro: divisão por zero.")
                exit()
            resultado = nu1 / nu2

        print(f'Resultado: {resultado}')
    except ValueError:
        print("Erro: digite apenas números válidos.")
