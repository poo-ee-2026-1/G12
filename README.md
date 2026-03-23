 Sistema de Gerenciamento de E-commerce

CRONOGRAMA	
23/03/2026	Fixar o objetivo da loja
30/03/2026	Montar lista de produtos
06/04/2026	Criação de perfil da loja (P/clientes)
13/04/2026	
20/04/2026	Faturamento da loja diário
27/04/2026	
04/05/2026	Histórico de vendas
11/05/2026	Agregação Herança
18/05/2026	
25/05/2026	Encapsulamento
01/06/2026	Finalização do projeto

Este projeto foi desenvolvido com o objetivo de aplicar conceitos de Programação Orientada a Objetos (POO) na construção de um sistema que simula o funcionamento de uma plataforma de comércio eletrônico.

O sistema representa, de forma simplificada, o funcionamento de uma loja virtual, permitindo cadastrar produtos, controlar estoque, gerenciar carrinhos de compras e registrar pedidos realizados por clientes.

Sistemas semelhantes são utilizados em grandes plataformas digitais de vendas, sendo a base de empresas como Amazon, Mercado Livre e Shoppe.

 Objetivo do Projeto

O objetivo principal do projeto é desenvolver um sistema capaz de:

Gerenciar produtos de uma loja virtual

Controlar o estoque de mercadorias

Simular um carrinho de compras

Calcular o valor total de pedidos

Registrar compras realizadas por clientes

Gerar controle de faturamento da loja

Além disso, o projeto busca integrar conceitos importantes do comércio eletrônico, como:

Gestão de produtos

Controle de estoque

Processamento de pedidos

Cálculo de faturamento

Paralelamente, o sistema aplica conceitos fundamentais de Programação Orientada a Objetos, incluindo:

Encapsulamento

Herança

Polimorfismo

 Estrutura do Projeto

O sistema é composto por três classes principais que representam as entidades fundamentais de uma loja virtual.

1️. Classe Produto

A classe Produto representa um item disponível para venda dentro da loja virtual.

Cada objeto dessa classe corresponde a um produto real comercializado na plataforma, como por exemplo:

notebooks

celulares

roupas

acessórios

Atributos

nome

preco

estoque

categoria

Métodos

atualizarEstoque(quantidade)
Atualiza a quantidade disponível do produto após uma venda ou reposição.

verificarDisponibilidade()
Verifica se o produto ainda possui unidades disponíveis em estoque.

exibirInformacoes()
Apresenta os dados do produto, como nome, preço, categoria e quantidade disponível.

2️. Classe CarrinhoDeCompras

A classe CarrinhoDeCompras simula o carrinho utilizado por um cliente durante o processo de compra em uma loja virtual.

Ela permite que produtos sejam adicionados ou removidos antes da finalização do pedido.

Atributos

listaProdutos

quantidadeProdutos

Métodos

adicionarProduto(produto, quantidade)
Adiciona um produto ao carrinho juntamente com a quantidade desejada.

removerProduto(produto)
Remove um produto previamente adicionado ao carrinho.

calcularTotal()
Calcula o valor total da compra com base no preço e quantidade de cada item.

exibirCarrinho()
Mostra todos os produtos presentes no carrinho e suas respectivas quantidades.

3️. Classe SistemaEcommerce

A classe SistemaEcommerce representa o núcleo do sistema da loja virtual.

Ela é responsável por gerenciar os produtos disponíveis e registrar os pedidos realizados pelos clientes.

Atributos

listaProdutos

pedidosRealizados

faturamentoTotal

Métodos

cadastrarProduto(produto)
Adiciona um novo produto ao catálogo da loja.

listarProdutos()
Exibe todos os produtos disponíveis no sistema.

registrarPedido(carrinho)
Registra um pedido realizado por um cliente e atualiza o estoque dos produtos comprados.

calcularFaturamento()
Calcula o faturamento total da loja com base nos pedidos realizados.

 Relacionamento entre Classes

A interação entre as classes ocorre da seguinte forma:

SistemaEcommerce
       │
       │ gerencia
       ▼
     Produto
       │
       │ adicionado ao
       ▼
CarrinhoDeCompras

O SistemaEcommerce administra todos os produtos disponíveis na loja.
Esses produtos podem ser adicionados ao CarrinhoDeCompras, onde os clientes realizam suas compras.

 Conceitos de POO Aplicados
Encapsulamento

Os atributos das classes são protegidos e manipulados por meio de métodos específicos, garantindo maior controle e segurança sobre os dados do sistema.

Herança

A classe Produto pode servir como base para diferentes tipos de produtos especializados.

Cada tipo de produto pode possuir características adicionais específicas.

Exemplos:

Eletrônicos → podem possuir garantia

Roupas → possuem tamanho

Livros → possuem autor

Polimorfismo

O polimorfismo permite que diferentes tipos de produtos possuam comportamentos próprios em determinados métodos, mantendo a mesma estrutura básica herdada da classe principal.

Isso facilita a extensão do sistema, permitindo adicionar novos tipos de produtos sem alterar a lógica central da aplicação.

 Funcionalidades do Sistema

Entre as principais funcionalidades implementadas no sistema estão:

Cadastro de produtos

Controle de estoque

Simulação de carrinho de compras

Cálculo automático do valor total da compra

Registro de vendas realizadas

Controle de faturamento da loja

 Cálculos Utilizados
Valor Total do Pedido

O valor total de uma compra é calculado somando o valor de todos os produtos multiplicados por suas respectivas quantidades.

Fórmula:

Total = ∑ (preço × quantidade)

Atualização de Estoque:

Após a realização de uma compra, o estoque do produto é atualizado automaticamente.

Fórmula:

Estoque_novo = Estoque_atual − Quantidade_vendida

 Controle de Estoque

O sistema verifica se um produto ainda possui unidades disponíveis para venda.

Caso o estoque de um produto atinja zero, o sistema pode indicar:

 PRODUTO ESGOTADO

Esse comportamento simula situações comuns em plataformas reais de comércio eletrônico.

 Possíveis Melhorias Futuras

O projeto pode ser expandido com novas funcionalidades, tais como:

Sistema de login para clientes

Avaliação de produtos por usuários

Recomendações de produtos

Dashboard de vendas

Integração com banco de dados

Histórico de compras por cliente

 Contexto Acadêmico

Este projeto foi desenvolvido como uma aplicação prática dos conceitos de:

Programação Orientada a Objetos

Modelagem de sistemas de software

Desenvolvimento de sistemas de comércio eletrônico

O objetivo é demonstrar como conceitos fundamentais de programação podem ser utilizados na construção de soluções aplicadas a problemas reais do mundo digital, aproximando a teoria estudada em sala de aula da prática de desenvolvimento de software.
