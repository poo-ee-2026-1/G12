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

​Conceitos de POO Aplicados

​A robustez do projeto advém da implementação dos quatro pilares da Programação Orientada a Objetos:

​Abstração: Utilizada para modelar as complexidades do mundo real em entidades sistêmicas simplificadas. Focamos apenas nos atributos e comportamentos essenciais para o funcionamento da loja (como preço e estoque), ignorando detalhes irrelevantes ao software.

​Encapsulamento: Garante que dados sensíveis, como o faturamento total e os níveis de estoque, sejam protegidos contra acessos externos indevidos. A manipulação desses dados ocorre exclusivamente através de métodos seguros e controlados.

​Herança: Permite a especialização dos produtos. A classe base ProdutoEsportivo compartilha sua estrutura com classes filhas (ex: Calçados, Equipamentos), permitindo que categorias específicas possuam atributos próprios sem repetir código.

​Polimorfismo: Oferece flexibilidade ao sistema, permitindo que diferentes tipos de produtos executem comportamentos comuns (como a exibição de detalhes ou cálculos de desconto) de formas distintas, adaptadas a cada categoria.

Funcionalidades Implementadas

​O sistema entrega um conjunto completo de operações que garantem o gerenciamento eficiente do e-commerce:

​Gestão de Inventário: Cadastro detalhado de produtos esportivos com controle de estoque em tempo real, incluindo sinalização de itens esgotados.

​Pipeline de Vendas: Simulação completa de carrinho de compras, permitindo a adição, remoção e revisão de itens antes do fechamento.

​Inteligência de Negócio: Registro automatizado de vendas e controle centralizado do faturamento total da loja.

​Possíveis Melhorias Futuras

​Este projeto foi desenhado para ser escalável, permitindo a implementação futura de módulos como:

​Personalização: Sistema de login para clientes, histórico de compras individual e recomendações de produtos baseadas em preferências.

​Análise de Dados: Dashboards de vendas por categoria e sistemas de avaliação de produtos por usuários.

​Infraestrutura: Integração com bancos de dados relacionais e interfaces gráficas para o usuário (GUI).

​Contexto Acadêmico

​Este projeto é uma aplicação prática desenvolvida para consolidar conhecimentos em Programação Orientada a Objetos, Modelagem de Sistemas de Software e E-commerce. A adaptação para o segmento esportivo demonstra como conceitos teóricos complexos podem ser aplicados a cenários reais de negócios digitais, aproximando a teoria estudada em sala de aula da prática de desenvolvimento de software profissional.
