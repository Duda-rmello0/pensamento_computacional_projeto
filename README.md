# pensamento_computacional_projeto

'''
Isso é um bloco de comentário

Projeto Padaria:


>PD (Como dono do negócio: Eu quero criar um sistema de vendas para a padaria,
para que os clientes possam comprar nossos produtos online e para que eu consiga contolar
as vendas e os produtos disponíveis.)

>QA (Como cliente: Eu quero poder ter facilidade para comprar os produtos da padaria online,
para que eu possa economizar tempo e evitar filas.)

>Tech (Como programador: Eu quero criar um sistema de vendas para que eu possa desenvolver
minhas habilidades de programação e criar um projeto útil para a padaria.)

>Dev (Como programador: quero um sistema de vendas para a padaria para que eu possa 
implementar as funcionalidades necessárias, como cadastro de produtos, gerenciamento de estoque 
e processamento de pedidos, utilizando as melhores práticas de desenvolvimento de software.)

>Uk (Como designer de experiêcia do usuário: Eu quero um sistema de vendas para a padaria
para que eu possa criar uma interface intuitiva e agradável para os clientes, 
facilitando a navegação e a realização de compras online.)

>IA (Como análise de dados: Eu quero um sistema de vendas para a padaria para que eu possa coletar
e analisar os dados de vendas, identificar padrões de compra e fornecer insights para melhorar 
as estratégias de marketing e vendas da padaria.)

>>Criar um aplicativo, sistema CLT - Command Line Interface, ou seja, um sistema que funcione no 
terminal, sem interface gráfica.
>>Completar e Implementar o app 




'''





'''

while True:
    print('Bem-vindo ao projeto de desenvolvimento de um sistema de vendas para a padaria!')
    print('\n---------------------------------------------------\n')
    print('Bem vindo ao sistema de vendas - Padaria\n')
    print('1. Cadastrar Produto')
    print('2. Listar Produtos')
    print('3. Excluir Produto')
    print('4. Pesquisar Produto')
    print('5. Realizar Venda')
    print('6. Suporte ao cliente')
    print('7. Cancelar venda')
    print('0. Sair')
    print('\n---------------------------------------------------\n')

    opcao = input('Digite a opção desejada: ')

    if opcao == '1':
     print('Opção 1 selecionada: Cadastrando Produtos...')
    
     if p1_nome == '':
        p1_nome = input ('Digite o nome do produto:')
        p1_descricao = input('Digite a descrição do produto: ')
        p1_validade = input('Digite a validade do produto: ')
        p1_estoque = int(input('Digite a quantidade a quantidade em estoque: '))
        p1_preco = float(input('Digite o preço do produto: '))
        print(f'\n✨ Produto (p1_nome) cadastrado na vaga 1!')

    elif p2_nome == '':
        p2_nome = input ('Digite o nome do produto:')
        p2_descricao = input('Digite a descrição do produto: ')
        p2_validade = input('Digite a validade do produto: ')
        p2_estoque = int(input('Digite a quantidade a quantidade em estoque: '))
        p2_preco = float(input('Digite o preço do produto: '))
        print(f'\n✨ Produto (p2_nome) cadastrado na vaga 2!')

    elif p3_nome == '':
        p3_nome = input ('Digite o nome do produto:')
        p3_descricao = input('Digite a descrição do produto: ')
        p3_validade = input('Digite a validade do produto: ')
        p3_estoque = int(input('Digite a quantidade a quantidade em estoque: '))
        p3_preco = float(input('Digite o preço do produto: '))
        print(f'\n✨Produto(p3_nome) cadastrado na vaga 3!') 

    elif p4_nome == '':
        p4_nome = input ('Digite o nome do produto:')
        p4_descricao = input('Digite a descrição do produto: ')
        p4_validade = input('Digite a validade do produto: ')
        p4_estoque = int(input('Digite a quantidade a quantidade em estoque: '))
        p4_preco = float(input('Digite o preço do produto: '))
        print(f'\n✨Produto(p4_nome) cadastrado na vaga 4!')     

    elif p5_nome == '':
        p5_nome = input ('Digite o nome do produto:')
        p5_descricao = input('Digite a descrição do produto: ')
        p5_validade = input('Digite a validade do produto: ')
        p5_estoque = int(input('Digite a quantidade a quantidade em estoque: '))
        p5_preco = float(input('Digite o preço do produto: '))
        print(f'\n✨Produto(p5_nome) cadastrado na vaga 5!') 



    elif opcao == '2':
        print('Opção 2 selecionada: Listando Produtos...')
        
         if p1_nome == '' and p2_nome == '' and p3_nome == '':
           print('Nenhum produto cadastrado no sistema ainda.')

    else:
        if p1_nome != '':
            print(f'Nome: (p1_nome) | Preço: R$ (p1_preco:.2f) | Estoque: (p1_estoque) unid.')
            print(f'Validade:(p1_validade) | Descrição: (p1_descricao)')
            print('-' = 30)

        if p2_nome != '':
            print(f'Nome: (p2_nome) | Preço: R$ (p2_preco:.2f) | Estoque: (p2_estoque) unid.')
            print(f'Validade:(p2_validade) | Descrição: (p2_descricao)')
            print('-' = 30)

        if p3_nome != '':
            print(f'Nome: (p3_nome) | Preço: R$ (p3_preco:.2f) | Estoque: (p3_estoque) unid.')
            print(f'Validade:(p3_validade) | Descrição: (p3_descricao)')
            print('-' = 30)       

        if p4_nome != '':
            print(f'Nome: (p4_nome) | Preço: R$ (p3_preco:.2f) | Estoque: (p3_estoque) unid.')
            print(f'Validade:(p3_validade) | Descrição: (p3_descricao)')
            print('-' = 30)           
       
       
       


    elif opcao == '3':
        print('Opção 3 selecionada: Excluindo Produto')
        produto_listado = ('Selecione o produto que deseja excuir: ')
        arquivar_produto = ('Arquivar produto: ')
        ocultar_produto = ('Ocultar produto: ')

    if opcao == '3':
            print('\nOpção 3 selecionada: Excluindo Produto\n')
        if p1_nome == "" and p2_nome == "" and p3_nome == "":
            print('Não há produtos para excluir.')
        else:
            produto_excluir = input('Digite o nome do produto que deseja excluir: ')
            
            if produto_excluir.lower() == p1_nome.lower() and p1_nome != "":
                p1_nome = '' # Limpar o nome libera a vaga
                print('✔ Produto da vaga 1 excluído com sucesso!')
            elif produto_excluir.lower() == p2_nome.lower() and p2_nome != "":
                p2_nome = ''
                print('✔ Produto da vaga 2 excluído com sucesso!')
            elif produto_excluir.lower() == p3_nome.lower() and p3_nome != "":
                p3_nome = ''
                print('✔ Produto da vaga 3 excluído com sucesso!')
            else:
                print('❌ Produto não encontrado.')





    elif opcao == '4':
    print('Opção 4 selecionada: Pesquisando produto...')

    elif opcao == '5':
    print('Opção 5 selecionada: Realizando venda...')

    elif opcao == '6':
    print('Opção 6 selecionada: Suporte ao cliente')

    elif opcao == '7':
    print('Opção 7 selecionada: Cancelando venda...')

    elif opcao == '0':
    print('Opção 0 selecionada: Saindo...')

    else:
    print('opção inválida!')
