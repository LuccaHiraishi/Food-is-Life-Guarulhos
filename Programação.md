# Food-is-Life-Guarulhos
# Pontuação de cada alimento
Arroz = 5
Feijão = 5
Farinha = 2
Leite_em_pó = 4
Macarrão = 5
Molho_de_tomate = 4
Alimentos = ["Arroz, Feijão, Farinha, Leite_em_pó, Macarrão, Molho_de_tomate"]
AlimentosEscritos = ["Arroz", "Feijão", "Farinha", "Leite em pó", "Macarrão", "Molho de tomate"]
Locais = ['07012-031']
Email_Cadastrados = ['luccahiraishi@gmail.com', ]
# Email_Cadastrados = ""
Pontuação = []
email2 = []
escolha = []
usuario = []
feito = False
sair = False
Sair = []
Feito = []

usuario = input("Digite seu nome de usuário: ")
print("Seja bem vindo ao Food's Life, um desafio para acabarmos com a fome zero")
print('O que podemos fazer para você hoje, {}?'.format(usuario))
print('\nLista de seleção: (1) - Quem são vocês\n')
print('(2) - Quais alimentos podem ser doados / situação com os alimentos\n')
print('(3) - Cadastrar email\n')
print('(4) - Minha tabela de pontos / lista de prêmios\n')
print('(5) - Onde posso entregar a minha doação?\n')
print('(6) - Entrar em contato conosco\n')
print('(7) - Sair')

while not feito and not sair:
    escolha = int(input("Digite onde quer ir: "))
    if escolha == 1:
        print("Somos a Food's Life, uma pequena ideia que visa a diminuição dos casos de fome em Guraulhos")

    elif escolha == 2:
        print("No momento, estamos aceitando os seguintes alimentos:")
        print(AlimentosEscritos)
        print("(1) Continuar/ (2) Sair")
        Completo = int(input("Você quer continuar?: "))
        if Completo == 1:
            print("Aguarde um instante")
        else:
            print("Espero que tenhamos ajudado")
            feito = Feito =+ 1

    elif escolha == 3:
        print("Digite seu email, ele será cadastrado para que toda vez que você realize a doação, os seus pontos serão"
              " atualizados")
        Email = input("Digite seu email aqui: ")
        Email_Cadastrados.append(Email)
        print("Email cadastrado com sucesso, na próxima vez que você for até algum posto de doação, informe seu email "
              "para")
        print("contabilizar seus pontos")
        print("(1) Continuar/ (2) Sair")
        Completo = int(input("Você quer continuar?: "))
        if Completo == 1:
            print("Aguarde um instante")
        else:
            print("Espero que tenhamos ajudado")
            feito = Feito =+ 1

    elif escolha == 4:
        email2 = input("Digite seu email:")
        print("Seu total de pontos cadastrados é: {} ".format(Pontuação))
        print("(1) Continuar/ (2) Sair")
        Completo = int(input("Você quer continuar?: "))
        if Completo == 1:
            print("Aguarde um instante")
        else:
            print("Espero que tenhamos ajudado")
            feito = Feito =+ 1

    elif escolha == 5:
        print("No momento, estamos apenas localizados em Guarulhos, consulte os locais abaixo")
        print(Locais)
        print("(1) Continuar/ (2) Sair")
        Completo = int(input("Você quer continuar?: "))
        if Completo == 1:
            print("Aguarde um instante")
        else:
            print("Espero que tenhamos ajudado")
            feito = Feito =+ 1

    elif escolha == 6:
        print('Para contato direto, ligue para o número (11) 980572003')
        print('Para dúvidas, mande mensagem para:')
        print('luccahiraishi@gmail.com', 'felipemarcelino2806@gmail.com', 'rubiegamer6@gmail.com')
        print("(1) Continuar/ (2) Sair")
        Completo = int(input("Você quer continuar?: "))
        if Completo == 1:
            print("Aguarde um instante")
        else:
            print("Espero que tenhamos ajudado")
            feito = Feito =+ 1
    else:
        print("Muito Obrigado por utilizar o app do Food's Life")
        sair = Sair =+ 1
