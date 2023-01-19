---
title: Sobre o ABCD
permalink: /docs/pt/index
lang: pt
key: docs-quick-start-pt
---

## Introdução geral ao ABCD como um conjunto de software

ABCD é a sigla para um conjunto de software para a automação de bibliotecas e centros de documentação. Em espanhol esta é, na íntegra: ‘**A**utomatisación de **B**ibliotécas y **C**entros de **D**ocumentación’, que mantém a mesma sigla válida também para o francês (**A**utomation des **B**ibliothèques et **C**entres de **D**ocumentacion) ou português (**A**utomatização das **B**ibliotecas e dos **C**entros de **D**ocumentação). Mesmo em outras línguas não latinas, com algumas variações leves mas bastante aceitáveis, - por exemplo, holandês: ‘**A**utomatisering van **B**ibliotheken en **C**entra voor **D**ocumentatie’ - o acrônimo ainda pode ser mantido.

O próprio nome já expressa a ambição da suíte de software: não apenas fornecer funções de automação para as bibliotecas ‘clássicas’, mas também outros fornecedores de informação, tais como centros de documentação. A flexibilidade e a versatilidade estão na vanguarda dos critérios sobre os quais o software é desenvolvido. Esta flexibilidade, por exemplo, é ilustrada pelo fato de que em princípio, mas também na prática, qualquer estrutura bibliográfica pode ser gerenciada pelo software, ou mesmo criada por ele mesmo. Mesmo estruturas não-bibliográficas podem ser criadas, desde que as informações sejam principalmente informações ‘textuais’, pois esta é a limitação colocada pela tecnologia de banco de dados subjacente, que é o banco de dados textuais (CDS/)ISIS. O bom entendimento de alguns conceitos e técnicas básicas relacionadas ao ISIS, por exemplo, a linguagem de formatação, é crucial para o pleno domínio do ABCD-software. Por este motivo, algumas seções deste Manual também tratarão da tecnologia ISIS subjacente.

O ABCD é chamado de ‘suite’ de softwares para automação de bibliotecas e centros de documentação porque existe de alguns módulos relativamente independentes, que podem cooperar plenamente, mas também podem existir uns sem os outros. De fato, alguns softwares avançados existentes, a maioria já tendo demonstrado seu potencial em ambientes exigentes nas aplicações da BIREME (dentro do contexto da Biblioteca Virtual em Saúde), foram adotados e adaptados no ABCD - é por isso que os nomes originais como iAH, SeCS (ambos desenvolvidos pela BIREME) e EmpWeb (Empréstimos en Web) desenvolvidos originalmente por KALIO ltda. do Uruguai e amplamente testados em Valparaiso na Universidade) são mantidos. Estas partes principais são mostradas, com suas relações hierárquicas, no segundo nível na figura a seguir e posteriormente discutidas brevemente :

![Slide2](https://user-images.githubusercontent.com/20482054/137317710-09934ef8-971e-499b-ac63-0cb54f7677c2.JPG)

### A ABCD Central

O módulo ‘Central’ do ABCD compreende módulos para Administração de Bancos de Dados (criação de bancos de dados, edição de estruturas de bancos de dados, utilitários de bancos de dados), Catalogação, Aquisições, Circulação/Empréstimos e Estatística. Um módulo de administração de tesauro também está sendo preparado como parte do módulo de catalogação para uma base de dados específica da estrutura saurus com controle de consistência dos níveis hierárquicos. Como parte deste ‘módulo central’ também gostaríamos de mencionar serviços de importação e exportação, impressão e ferramentas de banco de dados como bloqueio/desbloqueio e ‘mudanças globais’ de campos em registros. Esta parte ‘Central’ de fato representa a parte ‘back-office’ do ABCD, os usuários finais não serão confrontados com isto, mas o que eles verão e serão oferecidos está totalmente definido nesta parte central de gerenciamento do software!

Qualquer estrutura de base de dados ISIS pode ser definida e gerenciada, com registros atualmente de 1Mb de tamanho máximo e 4Gb máximo, bancos de dados (mas estas restrições serão tornadas obsoletas pela próxima geração de ISIS e ABCD baseada no NBP). Em comparação com a tecnologia ISIS ‘normal’, são usadas chaves de indexação de 60 caracteres (em comparação com 30 caracteres), há recursos de controle de autoridade muito mais fortes disponíveis (listas de seleção baseadas em tabelas ou bancos de dados de autoridade, tais como thesauri) no estágio de entrada de dados com formatos de validação flexíveis) e toda a interação é baseada na tecnologia WWW, naturalmente, permitindo, por exemplo, cadeias de texto codificadas em HTML para indexação de texto completo, hiperlinks para páginas de ajuda, etc.

É perfeitamente possível automatizar completamente uma biblioteca menor com a maioria dos usuários internos com todas as funções necessárias, utilizando apenas esta parte Central, pois, por exemplo, uma opção de busca avançada é incorporada, de modo que todas as funções sejam cobertas com um mínimo de complexidade tecnológica (ou seja, apenas ISIS e PHP).

### O ABCD OPAC (iAH)

A interface de busca pública (OPAC) é uma versão adaptada da ‘interface avançada para informações de saúde’ (iAH) geral da BIREME. Ela permite metabuscas não apenas nos catálogos locais, mas também em muitos outros recursos de informação.

A interface iAH desenvolvida pela BIREME está sendo atualizada para o iAHx, garantindo o alinhamento perfeito com os modernos conceitos e técnicas de recuperação de informações (por exemplo, agrupamento, classificação de relevância com base na indexação Lucene).

### O site do ABCD

A função de busca é oferecida como parte de uma página de portal de ‘usuários finais’, apresentando o(s) próprio(s) catálogo(s) num contexto de informação muito mais amplo, fornecendo acesso a outros recursos de informação (por exemplo, Google, Medline…) e comunicação (anúncios, alertas), abrindo também o caminho para funções semelhantes à ‘Web 2.0’.

O Administrador do Site na verdade é um Sistema de Gerenciamento de Conteúdo específico que permite projetar a estrutura e os componentes da página do portal do ABCD.

### O Sistema de Controle de Séries ABCD (SeCS)

Este módulo oferece uma ferramenta de gerenciamento avançada para publicações em série (clássicas e/ou eletrônicas) de qualquer tipo de publicação pub (referente à periodicidade). Séries como tais, mas também edições de uma série e todos os tipos de padrões de publicação podem ser gerenciados por este módulo. A BIREME utiliza esta tecnologia, por exemplo, para seus produtos ‘Portal de Periódicos Científicos’ (ver :  [http://portal.revistas.bvs.br/main.php?home=true&lang=en)](http://portal.revistas.bvs.br/main.php?home=true&lang=en)) e SCAD (ver : http://scad.bvs.br/php/index.php?lang=en) que é o catálogo do sindicato brasileiro de mais de 12.000 periódicos (com milhões de edições) de mais de 50 bibliotecas.

### O módulo de Empréstimos Avançados ABCD (EmpWeb)

Este módulo oferece gerenciamento avançado de empréstimos com mais algumas características extras para organizações maiores e mais complexas. Ele oferece uma função ‘MyLibrary’ aos usuários finais através do OPAC e é baseado na tecnologia ‘web-services’. Ele pode ser usado para substituir o módulo integrado de empréstimos do ABCD em caso de necessidade de lidar com situações de múltiplas filiais/políticas e de volume de transações muito alto.

A idéia da ‘suíte’ reflete o fato de que o ABCD tem partes relativamente independentes - como é o caso das suítes de automação de escritório (por exemplo, Open Office, Microsoft Office) - mas com vínculos óbvios para cooperar. O módulo Estatísticas, por exemplo, como parte do módulo Circulação/Empréstimo, pode funcionar em qualquer base de dados ISIS, enquanto o iAH-OPAC também pode oferecer recuperação avançada baseada na web em qualquer (conjunto de) bases de dados ISIS, não apenas as mantidas pelo ABCD. O Sistema de Controle de Séries (SeCS) gerencia as bases de dados ISIS para séries dentro ou fora do contexto do ABCD. Mas juntos, acreditamos, estas partes constituem um conjunto muito poderoso de ferramentas, e como parte integrada esperamos que “a soma seja mais do que apenas as partes somadas”!artes somadas”!  