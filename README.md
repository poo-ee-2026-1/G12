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
 
 O projeto tem como meta a excelência técnica na implementação de conceitos fundamentais de engenharia de software. O sistema utiliza o Encapsulamento para garantir a proteção e manipulação segura dos dados através de métodos específicos, a Herança para permitir a especialização de produtos com atributos únicos, e o Polimorfismo para conferir comportamentos distintos a diferentes tipos de mercadorias sem perder a integridade da lógica central. Dessa forma, o objetivo transcende a simples automação de vendas, consolidando-se como uma aplicação escalável e bem estruturada, pronta para futuras expansões como a integração com bancos de dados e dashboards de análise de vendas.

​Estrutura do Sistema

​O sistema é fundamentado em três classes principais que interagem entre si para garantir o fluxo de venda e a organização dos dados.

​ Classe ProdutoEsportivo

​Esta classe representa a entidade base de qualquer item disponível na loja, como tênis, camisas ou acessórios fitness. Ela é responsável por carregar as informações fundamentais e as regras de disponibilidade do item.
​Atributos: Incluem o nome, preço, quantidade em estoque e categoria (ex: calçados, equipamentos).
​Métodos Principais:
​atualizarEstoque(quantidade): Gerencia a entrada e saída de itens após vendas ou reposições.
​verificarDisponibilidade(): Valida se há unidades suficientes para atender a um pedido.
​exibirInformacoes(): Retorna os detalhes completos do produto para o usuário.

​ Classe CarrinhoDeCompras

​Funciona como uma entidade temporária que armazena a intenção de compra do cliente, permitindo a manipulação dos itens antes da finalização do pedido.
​Atributos: Mantém uma lista dinâmica de produtos selecionados e a contagem das quantidades de cada item.
​Métodos Principais:
​adicionarProduto(produto, quantidade): Insere itens no carrinho.
​removerProduto(produto): Retira itens previamente selecionados.
​exibirCarrinho(): Apresenta o resumo de todos os itens e subtotais acumulados.

​ Classe SistemaLojaEsportiva

​É o núcleo (core) da aplicação, funcionando como o administrador central que conecta os produtos aos pedidos e gera os dados financeiros.
​Atributos: Gerencia o catálogo completo de produtos da loja, o histórico de pedidos realizados e o faturamento total acumulado.
​Métodos Principais:
​cadastrarProduto(produto): Adiciona novos itens ao portfólio da loja.
​listarProdutos(): Exibe o catálogo disponível para o cliente.
​registrarPedido(carrinho): Processa a venda, atualiza o estoque global de forma automática e soma o valor ao faturamento da loja.

Aplicação dos Conceitos de POO
​Para garantir a escalabilidade mencionada no objetivo, o código aplica os pilares de POO da seguinte forma:

​Encapsulamento: Os dados sensíveis (como faturamento e estoque) são protegidos, sendo acessados apenas por métodos seguros, evitando alterações indevidas.

​Herança: A classe ProdutoEsportivo serve como base para especializações, permitindo que classes como Calcados ou Vestuario herdem comportamentos comuns, mas possuam atributos específicos (como numeração ou tipo de tecido).

​Polimorfismo: Permite que diferentes categorias de produtos reajam de formas distintas ao mesmo comando (como o cálculo de desconto ou exibição de detalhes), mantendo a interface do sistema padronizada.

????Funcionalidades do Sistema
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
