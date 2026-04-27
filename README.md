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

 Sistema de Gerenciamento de E-commerce

Projeto: Sistema de Loja Esportiva Virtual com POO

 Este projeto foi desenvolvido para aplicar conceitos de Programação Orientada a Objetos (POO) em um sistema que simula o funcionamento de uma loja esportiva virtual.

 O sistema permite cadastrar produtos esportivos, controlar estoque, gerenciar carrinhos de compras e registrar pedidos realizados por clientes, simulando a experiência de compra de grandes plataformas de e-commerce, mas voltada exclusivamente para artigos esportivos.

Objetivo do Projeto

 O objetivo central deste sistema é simular o funcionamento completo de uma loja esportiva virtual, utilizando essa estrutura como base para a aplicação prática dos pilares da Programação Orientada a Objetos (POO). A proposta foca em gerenciar o ciclo de vida dos produtos esportivos — desde o cadastro de itens como calçados, vestuário e equipamentos até o controle dinâmico de estoque e faturamento diário da loja. Através de uma arquitetura que integra as classes ProdutoEsportivo, CarrinhoDeCompras e SistemaLojaEsportiva, o projeto busca replicar a experiência de grandes plataformas de e-commerce, permitindo que o usuário gerencie carrinhos, registre pedidos e acompanhe o histórico de vendas de forma organizada e eficiente.
 Paralelamente à gestão comercial, o projeto tem como meta a excelência técnica na implementação de conceitos fundamentais de engenharia de software. O sistema utiliza o Encapsulamento para garantir a proteção e manipulação segura dos dados através de métodos específicos, a Herança para permitir a especialização de produtos com atributos únicos, e o Polimorfismo para conferir comportamentos distintos a diferentes tipos de mercadorias sem perder a integridade da lógica central. Dessa forma, o objetivo transcende a simples automação de vendas, consolidando-se como uma aplicação escalável e bem estruturada, pronta para futuras expansões como a integração com bancos de dados e dashboards de análise de vendas.

O sistema é composto por três classes principais que representam as entidades fundamentais de uma loja esportiva:

1️. Classe ProdutoEsportivo

A classe ProdutoEsportivo representa cada item disponível para venda na loja, como:

Tênis de corrida
Bola de futebol
Camisas de times
Luvas de boxe
Acessórios fitness

Atributos:
nome
preco
estoque
categoria (ex: calçados, equipamentos, vestuário)

Métodos:
atualizarEstoque(quantidade) → Atualiza a quantidade disponível após venda ou reposição
verificarDisponibilidade() → Verifica se o produto ainda possui unidades disponíveis
exibirInformacoes() → Exibe detalhes do produto, incluindo nome, preço, categoria e quantidade em estoque
2️. Classe CarrinhoDeCompras

Simula o carrinho utilizado pelo cliente durante a compra na loja esportiva.

Atributos:

listaProdutos (produtos adicionados ao carrinho)
quantidadeProdutos (quantidade de cada produto)

Métodos:

adicionarProduto(produto, quantidade) → Adiciona produtos ao carrinho, incluindo a quantidade desejada
removerProduto(produto) → Remove produtos previamente adicionados
exibirCarrinho() → Mostra todos os produtos no carrinho e suas quantidades

O carrinho permite ao cliente revisar os itens antes de finalizar a compra, simulando o processo real de e-commerce.

3️. Classe SistemaLojaEsportiva

Representa o núcleo do sistema, responsável por gerenciar os produtos e registrar os pedidos dos clientes.

Atributos:

listaProdutos (todos os produtos disponíveis na loja)
pedidosRealizados (histórico de compras)
faturamentoTotal (valor total das vendas)

Métodos:

cadastrarProduto(produto) → Adiciona novos produtos ao catálogo da loja
listarProdutos() → Exibe todos os produtos disponíveis para venda
registrarPedido(carrinho) → Registra o pedido do cliente e atualiza automaticamente o estoque dos produtos comprados

O SistemaLojaEsportiva é responsável por organizar todo o funcionamento da loja, garantindo que os produtos estejam disponíveis e que as compras sejam corretamente registradas.

Relacionamento entre Classes

O fluxo de interação entre as classes é o seguinte:

SistemaLojaEsportiva
       │
       │ gerencia
       ▼
   ProdutoEsportivo
       │
       │ adicionado ao
       ▼
 CarrinhoDeCompras

O SistemaLojaEsportiva administra todos os produtos disponíveis na loja. Os produtos podem ser adicionados ao CarrinhoDeCompras, permitindo que os clientes finalizem suas compras de forma organizada e eficiente.

Conceitos de POO Aplicados

Encapsulamento:
Os atributos das classes são protegidos e manipulados por métodos específicos, garantindo maior controle e segurança sobre os dados.

Herança:
A classe ProdutoEsportivo pode servir como base para diferentes tipos de produtos especializados:

Calçados → podem ter atributos como número, tipo de pisada e material
Vestuário → podem ter tamanho, material e gênero
Equipamentos → podem ter peso, tipo de uso e categoria esportiva

Polimorfismo:
Permite que diferentes tipos de produtos possuam comportamentos próprios em métodos específicos, mantendo a mesma estrutura básica da classe principal. Isso facilita a expansão do sistema, permitindo adicionar novos tipos de produtos sem alterar a lógica central.

Funcionalidades do Sistema

Entre as principais funcionalidades implementadas estão:

Cadastro de produtos esportivos
Controle de estoque (indicando produtos esgotados quando necessário)
Simulação de carrinho de compras
Registro de vendas realizadas
Controle de faturamento da loja
Possíveis Melhorias Futuras

O projeto pode ser expandido com novas funcionalidades, tais como:

Sistema de login para clientes
Avaliação de produtos por usuários
Recomendações de produtos personalizadas
Dashboard de vendas por categoria
Integração com banco de dados
Histórico de compras por cliente
Contexto Acadêmico

Este projeto foi desenvolvido como uma aplicação prática dos conceitos de:

Programação Orientada a Objetos
Modelagem de sistemas de software
Desenvolvimento de sistemas de comércio eletrônico

A adaptação para uma loja esportiva demonstra como conceitos de POO podem ser aplicados a cenários reais de negócios digitais, aproximando a teoria estudada em sala de aula da prática de desenvolvimento de software.
