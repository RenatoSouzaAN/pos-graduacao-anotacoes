
![[img01.png]]

# Desenvolvimento Back-End Avançado (Disciplina 1)

## Padrões Arquiteturais (Aula 1)

### Conceitos básicos

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb1.png]]

#### Arquitetura cliente-servidor

No padrão arquitetural cliente-servidor, a computação é dividida entre várias máquinas. A topologia desse padrão determina que componentes em uma máquina **servidor** forneçam funcionalidades para componentes em várias máquinas **clientes** por meio de uma conexão de rede. O servidor centraliza recursos computacionais, que podem ser compartilhados por muitos usuários, e os clientes desses recursos podem permanecer relativamente simples.

**Na topologia cliente-servidor, o cliente é quem invoca as funcionalidades disponibilizadas pelo servidor**. Em geral, o cliente é responsável por lidar com a interface do usuário e a lógica da aplicação. Ele é executado na máquina cliente e interage diretamente com o usuário. O cliente envia solicitações para o servidor para obter dados ou serviços e recebe as respostas em retorno. O servidor gerencia o armazenamento de dados, o processamento e a lógica de negócios da aplicação. Ele recebe solicitações dos clientes, processa-as e envia as respostas apropriadas. Além disso, é responsável por gerenciar o acesso aos dados e executar as operações solicitadas pelo cliente. Com boa parte das responsabilidades centralizadas no servidor, a arquitetura cliente-servidor tem algumas vantagens e desvantagens.

![[Pasted image 20240724113235.png]]

![[Pasted image 20240724113244.png]]
#### Padrão arquitetural em camadas

O padrão arquitetural em camadas é um dos mais conhecidos e utilizados no desenvolvimento de aplicações _web_. Também é utilizado em inúmeros domínios e situações, variando de sistemas empresariais e aplicações _desktop_ a sistemas distribuídos, máquinas virtuais e modernizações de sistemas legados. **Esse padrão é composto por um conjunto de duas ou mais camadas, organizadas hierarquicamente, que se comunicam entre si**. Cada camada tem uma atribuição específica e apenas se comunica com as subjacentes por meio de interfaces bem definidas. Embora sigam essas mesmas restrições, existem ao menos duas especializações do padrão arquitetural em camadas.

Uma delas é o padrão que determina a **separação em camadas físicas** (_N-tier architecture_). Nesse caso, as camadas são compostas por entidades físicas, como computadores pessoais, servidores ou dispositivos móveis. A figura a seguir apresenta um exemplo de arquitetura com três camadas físicas (_3-tier architecture_), com os dispositivos pessoais contendo a apresentação, o servidor contendo a lógica principal do sistema e a máquina contendo o banco de dados.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb3.png]]

Uma segunda especialização do padrão em camadas é a que estabelece a **separação de conceitos ou funcionalidades em camadas lógicas** (_layered architecture_). Cada camada separa um conceito ou funcionalidade. Eventualmente, as camadas podem estar alocadas em um mesmo equipamento de _hardware_. A próxima figura ilustra um exemplo de arquitetura com três camadas lógicas (_3-layer architecture_), cada uma modularizando, respectivamente, a interface com o usuário, a lógica de negócio e o acesso aos dados. Note que cada camada apenas se comunica com as camadas vizinhas. Por exemplo: a camada de interface do usuário e a de acesso a dados apenas se comunicam com a camada da lógica de negócio, enquanto esta última se comunica com as duas primeiras.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb4.png]]

#### Separação em camadas físicas

Certos sistemas de _software_ têm uma única camada física (_tier_), isto é, todos os componentes de _software_ do sistema estão localizados em um único dispositivo de _hardware_. Entre os exemplos, temos: aplicativos _desktop_, como o Office da Microsoft; alguns jogos para computadores pessoais; e _softwares_ de edição de imagem, como Paint ou Photoshop.

A vantagem da camada física única é que os componentes desses sistemas não têm latência de rede para se comunicarem, já que todos estão localizados na mesma máquina. Isso aumenta o desempenho do _software_. Outra vantagem é a privacidade e segurança de dados, pois os dados do usuário sempre permanecem em sua máquina e não precisam ser transmitidos por uma rede para persistência. Por outro lado, uma grande desvantagem é a dificuldade de atualização do _software_. Depois que o _software_ é enviado, nenhuma atualização de código ou recurso pode ser feita até que o cliente o atualize manualmente, conectando-se a algum servidor remoto ou baixando e instalando um _patch_.

Já os sistemas de duas, três e N camadas precisam de comunicação envolvendo os _hardwares_ representados pelas diferentes camadas físicas. A arquitetura cliente-servidor, descrita na seção anterior, usualmente apresenta duas camadas físicas. Nesse cenário, computadores (clientes) em uma camada precisam enviar solicitações de dados para o servidor com frequência. Isso adiciona latência de rede ao sistema, potencialmente tornando a experiência do usuário mais lenta, se comparado com sistemas em camada física única. Em aplicativos de camada única, os dados estão prontamente disponíveis, pois todos os componentes, incluindo o próprio banco de dados, estão localizados na mesma máquina.

#### Separação em camadas lógicas

Uma arquitetura de camadas lógicas convencional em projetos _web_ é aquela que segrega as funcionalidades do sistema em **quatro camadas**.

![[Pasted image 20240724114618.png]]

![[Pasted image 20240724114649.png]]

![[Pasted image 20240724114729.png]]

![[Pasted image 20240724114902.png]]

Essa arquitetura em quatro camadas **permite uma separação clara de responsabilidades e promove a modularidade e a reutilização de componentes**. Essas características, por sua vez, também facilitam a manutenção e o teste do sistema. Além disso, cada camada pode isolar (das demais) as particularidades e complexidades das tecnologias apropriadas para sua implementação.

Por outro lado, a arquitetura clássica em quatro camadas lógicas também tem suas desvantagens. Com a restrição de comunicação somente entre camadas adjacentes, **pode haver um aumento na sobrecarga de comunicação entre as camadas**. Nas comunicações entre as camadas adjacentes, os mesmos dados (ou mutações destes) podem precisar trafegar entre várias camadas, resultando em um maior tráfego de dados, potencialmente afetando o desempenho do sistema. Além disso, determinadas alterações em uma camada podem exigir modificações nas camadas adjacentes, o que pode tornar **o sistema mais suscetível a impactos indesejados, aumentando a complexidade da manutenção**. Por fim, a adição de camadas nessa arquitetura pode dificultar a escalabilidade horizontal, em que novas instâncias de uma camada específica são adicionadas para lidar com a carga crescente. Coordenar e distribuir a carga entre as diferentes camadas pode ser mais complexo do que em arquiteturas aderentes a outros padrões.

#### Padrão modelo-visualização-controlador (MVC)

Uma variante do padrão em camadas, muito utilizada, é o padrão **modelo-visualização-controlador (MVC)**. Conforme podemos notar na figura a seguir, a ideia do padrão MVC é separar o projeto em três camadas lógicas e independentes: o modelo (manipulação da lógica de dados), a visualização (interface do usuário) e o controlador (fluxo de aplicação). A separação tem o objetivo de facilitar a manutenção da aplicação e fornecer sua reutilização em projetos futuros.

![[stb6-1.png]]

A partir de sua concepção, na década de 1980, o padrão MVC tem exercido uma influência dominante, especialmente no _design_ de interfaces gráficas do usuário. O MVC teve grande repercussão e sucesso, por ser o padrão, de fato, de muitas aplicações _web_ em variadas linguagens de programação. **Alguns _frameworks web_ populares, como Django e Rails, dão apoio ao padrão MVC.**

Por meio da separação explícita das três camadas, esse padrão oferece aos desenvolvedores a capacidade de **trabalhar de forma mais independente**, especialmente no que diz respeito à manipulação da informação pelo programa e às representações das interações do usuário com essa informação. O componente do modelo encapsula a informação utilizada pela aplicação, enquanto o componente de visualização oculta as informações selecionadas e necessárias para a representação gráfica desses dados. Por fim, o componente controlador encapsula a lógica necessária para manter a consistência entre o modelo e a visualização, além de tratar as entradas do usuário e sua relação com a representação gráfica correspondente (TAYLOR; MEDVIDOVIC; DASHOFY, 2009).

A estrutura MVC fornece outros benefícios (mas não se limita a eles), como a facilidade de manutenção pela separação e o reuso de partes da aplicação, mesmo para projetos futuros. O projeto que segue esse padrão também fornece um código mais testável, pois, além de o código ser mais granular, as diferentes camadas podem ser expostas a diferentes massas de teste com diferentes objetivos. É, também, relativamente fácil ter múltiplas visualizações do mesmo modelo, que, inclusive, podem ser habilitadas ou desabilitadas em tempo de execução.

O padrão MVC também tem suas desvantagens. Embora o MVC busque reduzir o acoplamento entre as camadas do sistema, ainda pode haver algum grau de acoplamento entre elas. Alterações em uma camada podem exigir ajustes nas outras camadas correspondentes, o que pode dificultar a manutenção do código. Não obstante, em muitas situações, os componentes de visualização e controle são unificados, como foi o caso da arquitetura do _framework_ Java’s Swing. O motivo é que, muito frequentemente, há um forte acoplamento entre as ações do componente de visualização e do componente controlador. Além disso, o uso do MVC tende a aumentar a complexidade e o tamanho do código-fonte, pois este usualmente requer a criação de várias classes para representar cada componente do MVC. É importante observar que muitas dessas desvantagens podem ser mitigadas com boas práticas de projeto.

### Arquitetura orientada a serviços (SOA) e microsserviços

A arquitetura orientada a serviços (SOA) é um padrão arquitetural em que os sistemas são construídos em termos de uma coleção de serviços independentes.

Esse padrão recebeu muita atenção, especialmente de 2000 a 2010. Um **serviço** pode ser qualquer funcionalidade que conclui uma ação e fornece um resultado específico, como o processamento de pedidos de clientes ou a produção de um relatório de itens em estoque. Os serviços são combinados para criar novos sistemas (NEWCOMER; LOMOW, 2005).

A SOA foi, em princípio, direcionada para apoiar empresas de negócios na internet. A ideia era que o negócio A poderia obter um serviço _b_ de um vendedor B, outro serviço _c_ do vendedor C, e assim por diante. Em um exemplo mais concreto, uma companhia pode obter propostas de preços de várias agências de viagem para uma dada requisição de itinerário (TAYLOR; MEDVIDOVIC; DASHOFY, 2009). Assim, ela pode selecionar a agência que oferece as melhores condições. Por sua vez, a agência vencedora pode interagir diretamente com as empresas subcontratadas para adquirir os vários serviços específicos necessários. Esses serviços podem incluir _tickets_ de voos aéreos, checagem de crédito e emissão de pagamentos eletrônicos ao vendedor. Todas essas interações podem ser suportadas pelos mecanismos de SOA.

#### Microsserviços

Desde 2014, o interesse em arquiteturas orientadas a serviços foi renovado com o surgimento do conceito de **microsserviços**, disseminado por uma publicação de Lewis e Fowler em um _blog_ sobre o assunto (LEWIS; FOWLER, 2014). Nesse mesmo período, também contribuiu para essa renovação de interesse um relato da Netflix compartilhando lições aprendidas com uma transição bem-sucedida de seu sistema para uma arquitetura orientada a microsserviços. O interesse renovado no desenvolvimento orientado a serviços também pode ser explicado por uma combinação de outros fatores, como a popularidade crescente de infraestruturas de nuvem e a constante demanda por agilidade de desenvolvimento.

O padrão baseado em microsserviços promove a construção de um sistema como um conjunto de microsserviços autônomos e independentes, isto é, que são executados como processos separados e podem ser implantados e dimensionados de forma independente (LEWIS; FOWLER, 2014). Cada microsserviço é um serviço de granularidade fina, modelado em torno de um domínio de negócios. De acordo com o padrão, cada microsserviço também deveria ter seu próprio esquema independente de dados, propiciando um desacoplamento ainda maior dos outros microsserviços disponíveis na arquitetura. Microsserviços utilizam protocolos leves de comunicação, como HTTP e REST, independentes de linguagem, e podem se comunicar de forma síncrona ou assíncrona. Além disso, instâncias de microsserviços podem ser adicionadas ou removidas conforme necessário, de acordo com a demanda do sistema.

De fato, uma das principais vantagens de uma arquitetura orientada a microsserviços é sua **escalabilidade horizontal**, que se refere à capacidade de aumentar a capacidade global do sistema pela adição de instâncias de um determinado serviço para melhor distribuir a carga maior deste. Esse tipo de escalabilidade é diferente da escalabilidade vertical, que envolve adicionar mais recursos a uma única instância do serviço, como aumentar a capacidade de processamento ou a quantidade de memória. A escalabilidade horizontal envolve a adição de mais instâncias do serviço em execução, para distribuir a carga e aumentar a capacidade global do sistema, consequentemente melhorando o desempenho deste e, possivelmente, se ajustando melhor às demandas de processamento em tempo real.

**O uso de múltiplas instâncias do mesmo microsserviço pode contribuir para uma maior resiliência (ou confiabilidade) do sistema, pois, assim, este é capaz de lidar com as falhas individuais de cada instância**. Caso uma instância de um microsserviço se encontre em estado de falha, as solicitações podem ser encaminhadas para outras instâncias suas em execução, garantindo a continuidade do serviço. Outro benefício da escalabilidade horizontal de microsserviços é a possibilidade de manutenção contínua. Algumas instâncias de microsserviços podem ser temporariamente interrompidas, atualizadas ou substituídas, sem afetar a disponibilidade geral do sistema. Isso permite que atualizações e correções sejam implementadas de forma isolada, minimizando o impacto nas operações do sistema.

No entanto, é importante observar que a escalabilidade horizontal também pode introduzir desafios adicionais, como a necessidade de lidar com a consistência dos dados distribuídos entre as instâncias do serviço e a complexidade de gerenciar a comunicação entre os serviços distribuídos.

### Padrões de arquitetura orientada a eventos

A arquitetura orientada a eventos é um padrão em que a comunicação entre os componentes é centrada na ocorrência de eventos. Os eventos representam alterações no estado do sistema, determinadas ações, entradas de dados dos usuários ou, mesmo, outras ocorrências relevantes. Os tipos de eventos são os mais variados possíveis, a depender do domínio e dos objetivos do sistema. Alguns exemplos são: “chegou uma nova mensagem”; “chegou um pedido”; “transferência bancária realizada”; “temperatura alta”; “falha ocorreu”; e “dispositivo se aproximando”.

**Cada componente em uma arquitetura orientada a eventos é projetado para comunicar ou reagir a esses eventos**. Nesse padrão, a comunicação entre os componentes é **assíncrona**, ou seja, os componentes executam suas tarefas sem aguardar a resposta imediata para suas requisições. Existem algumas especializações do padrão arquitetural orientadas a eventos, mas aqui iremos nos ater às arquiteturas _publish/subscribe_.

#### Arquiteturas publish/subscribe

O padrão arquitetural _publish/subscribe_ tem um modelo assíncrono de comunicação baseado em eventos, com dois tipos de componentes: **publicadores** e **assinantes**. Os publicadores de eventos são remetentes de mensagens que representam as notificações de ocorrências de eventos. Os assinantes registram seus interesses em determinados tipos de eventos e são receptores de mensagens. A comunicação entre publicadores e assinantes é intermediada por um barramento (ou _broker_) de eventos. Assim que um evento é publicado no barramento, todos os assinantes interessados nesse tipo de evento recebem assincronamente uma mensagem de notificação de sua ocorrência. As mensagens podem conter informações relacionadas ao evento publicado. A figura abaixo ilustra os componentes de uma arquitetura _publish/subcribe_ e suas interações.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb7.png]]

No padrão _publish/subscribe_, há um forte desacoplamento entre os componentes. Os publicadores não precisam ter conhecimento dos assinantes: eles simplesmente emitem os eventos no barramento, que fica encarregado de notificar os assinantes. Os publicadores não se tornam cientes dos assinantes que foram notificados. Por outro lado, os assinantes expressam seus interesses e recebem notificações de eventos, sem ter conhecimento dos publicadores que os emitiram. Além disso, cada assinante pode reagir a um mesmo evento de forma totalmente independente. **A indisponibilidade de um componente, seja ele um publicador ou assinante, não interfere na execução dos outros componentes**.

Da perspectiva do desenvolvedor de um componente assinante, o publicador pode ser encarado como uma “caixa-preta”. Ou seja, **o desenvolvedor do assinante não precisa se preocupar com detalhes de implementação ou mesmo com a lógica interna de funcionamento do publicador**. Se necessário, os assinantes só interagem com o publicador por meio da interface pública provida por este. Tendo em vista a grande aplicabilidade do padrão _publish/subscribe_, existem várias tecnologias que podem ser usadas para apoiar o desenvolvimento dessas arquiteturas, como **Apache Kafka**, **RabbitMQ** e **Redis**.

![[Pasted image 20240724123341.png]]

![[Pasted image 20240724123358.png]]

### Outros padrões arquiteturais

#### Arquitetura ponto a ponto (P2P, peer-to-peer)

Nesse padrão, os componentes individuais são conhecidos como pares. Os pares podem funcionar tanto como clientes, solicitando serviços de outros pares, quanto como servidores, fornecendo serviços a outros pares. Um par pode atuar como cliente, servidor ou ambos, e pode mudar seu papel dinamicamente com o tempo. Exemplos de uso dessa arquitetura incluem redes de compartilhamento de arquivos (como Gnutella e G2), protocolos multimídia e produtos baseados em criptomoedas.

#### Arquitetura "quadro-negro" (blackboard)

Esse padrão arquitetural estabelece um modelo colaborativo em que componentes (agentes) especialistas contribuem com conhecimentos para resolver problemas complexos. Um componente central, chamado quadro-negro (_blackboard_), age como uma grande memória compartilhada, armazenando dados e conhecimentos disponibilizados para todos os agentes especialistas. Os agentes monitoram o _blackboard_, atualizando-o com informações relevantes. A colaboração entre os componentes ocorre de forma assíncrona. Um componente controlador toma decisões com base nas informações disponíveis, principalmente para selecionar, configurar e executar os agentes. Esse padrão é útil para problemas para os quais não são conhecidas estratégias de solução determinística, e algumas aplicações conhecidas são reconhecimento de fala e identificação e rastreamento de veículos.

#### Arquitetura baseada em "dutos" e "filtros" (pipe-and-filter)

Nesse padrão, as tarefas são organizadas em uma sequência de estágios (_pipeline_), em que cada estágio executa uma parte específica do processamento de dados. Os dados fluem de um estágio para outro, permitindo o processamento em paralelo e a divisão das tarefas em partes menores e mais gerenciáveis. Existem dois tipos de componentes: filtros e dutos. Os filtros são os responsáveis pelo processamento dos dados em cada estágio e podem ser executados em paralelo, enquanto os dutos fornecem a estrutura que permite a passagem contínua dos dados de um estágio para outro. Os dutos permitem armazenar temporariamente os dados, enquanto não são obtidos pelo próximo filtro. Exemplos de sistemas que podem seguir esse padrão arquitetural são alguns compiladores, em que os filtros realizam análise léxica, análise sintática, análise semântica e geração de código.

### Diretrizes para escolha do padrão arquitetural

Cada padrão de arquitetura tem suas peculiaridades e atende a cenários específicos, com vantagens e desvantagens. A escolha do padrão é específica para cada contexto e envolve muitas variáveis. Entretanto, existem diretrizes gerais que os desenvolvedores deveriam seguir, algumas das quais destacamos aqui.


#### Entendimento do problema

O entendimento do problema em um projeto de _software_ desempenha papel fundamental na escolha do padrão arquitetural. **A escolha do padrão arquitetural está intrinsecamente ligada às características do sistema a ser desenvolvido**. Ao compreender em detalhes o problema que está sendo resolvido, os arquitetos de _software_ podem identificar características relevantes do projeto, como requisitos não funcionais e restrições, que estejam alinhadas com as vantagens de um determinado padrão arquitetural. Por exemplo, se o projeto envolver a manipulação de grandes volumes de dados, um padrão arquitetural baseado em microsserviços poderia ser apropriado, por sua capacidade de escalabilidade horizontal. Por outro lado, se o sistema exigir um alto nível de segurança, um padrão arquitetural baseado em camadas poderia ser preferível, para garantir a separação adequada das responsabilidades e a implementação de mecanismos de segurança em cada camada.

#### Análise dos benefícios e desvantagens dos padrões arquiteturais considerados

Cada padrão arquitetural tem suas vantagens e limitações. É importante realizar uma análise comparativa dos diferentes padrões relevantes para o projeto em questão. Considere os benefícios proporcionados por cada padrão em relação aos requisitos do sistema, bem como os desafios e compensações (_trade-offs_) que podem estar envolvidos.

#### Integração com outros sistemas

Outra diretriz para a escolha de um padrão arquitetural adequado é identificar a **necessidade de o sistema ser integrado com sistemas externos**. Caso o sistema precise ser integrado com outros sistemas ou serviços externos, devemos considerar como será a comunicação e a troca de dados entre eles. Essa questão pode privilegiar a adoção de uma arquitetura orientada a serviços ou eventos. Além disso, a integração pode envolver requisitos de autenticação e autorização para garantir a segurança dos dados e o acesso aos sistemas. Alguns padrões arquiteturais facilitam o suporte a mecanismos de autenticação e autorização mais robustos, como a arquitetura cliente-servidor com autenticação centralizada.

#### Processamento em tempo real

Se o sistema exigir processamento em tempo real, é necessário escolher um padrão arquitetural que suporte certas **demandas associadas**. Por exemplo, em sistemas com demanda de processamento em tempo real, a latência, ou seja, o tempo necessário para processar uma solicitação e fornecer uma resposta, é crítica. Dependendo dos requisitos de latência do sistema, certos padrões arquiteturais podem ser mais adequados do que outros. Arquiteturas orientadas a eventos são frequentemente utilizadas para reduzir a latência e permitir um processamento mais rápido de eventos.

#### Experiência e conhecimento da equipe

Considere a experiência e o conhecimento da equipe de desenvolvimento em relação aos diferentes padrões arquiteturais para um domínio ou problema em questão. Uma equipe com experiência em determinado padrão pode ter mais facilidade em implementá-lo de forma eficaz, pois pode conhecer certos desafios, vantagens e desvantagens que não são documentados explicitamente. Considere, também, a disponibilidade de recursos de aprendizagem e suporte para a equipe se familiarizar com novos padrões, caso seja necessário.

#### Compatibilidade com tecnologias e ferramentas existentes

Considere as tecnologias e ferramentas já utilizadas no projeto ou na organização. Alguns padrões arquiteturais podem se integrar de forma mais natural com determinadas tecnologias, enquanto outros podem exigir uma mudança significativa na pilha tecnológica. A compatibilidade com as tecnologias existentes pode influenciar a escolha do padrão arquitetural.

### Referências:

FOWLER, S. J. **Microsserviços prontos e para a produção**: construindo sistemas padronizados em uma organização de engenharia de _software_. São Paulo: Novatec, 2017.

LEWIS, J.; FOWLER, M. Microservices: a definition of this new architectural term. **Martin Fowler**, 2014. Disponível em: [https://www.martinfowler.com/articles/microservices.html](https://www.martinfowler.com/articles/microservices.html). Acesso em: 20 jun. 2023.

NEWCOMER, E.; LOMOW, G. **Understanding SOA with web services**. Upper Saddle River, NJ: Addison-Wesley, 2005.

RICHARDS, M.; FORD, N. **Fundamentals of software architecture**: an engineering approach. Sebastopol, CA: O’Reilly, 2020.

ROZANSKI, N.; WOODS, E. **Software systems architecture**: working with stakeholders using viewpoints and perspectives. Upper Saddle River, NJ: Addison- Wesley, 2009.

TAYLOR, R. N.; MEDVIDOVIC, N.; DASHOFY, E. **Software architecture**: foundations, theory, and practice. Hoboken, NJ: Wiley, 2009.

## Comunicação e Troca de Dados (Data Exchange) (Aula 2)

Para que duas aplicações _web_ possam se comunicar, de forma que uma possa acessar funcionalidades da outra, nós construímos **pontes**, que são as **APIs**. Via API, podemos estabelecer um **canal claro de comunicação** permitindo a integração entre aplicações de forma rápida e escalável. No entanto, para garantir o sucesso dessa comunicação, ela deve ser feita utilizando **protocolos** e/ou respeitando **especificações** que irão definir a forma e o formato das mensagens que serão trocadas ao longo do processo. Nesta segunda aula, vamos falar de estilos de comunicação voltados para a construção de APIs.

**Quando falamos de APIs, falamos de comunicação**. Nesse contexto, o cenário ideal de comunicação é aquele em que duas partes interagem, conversam, se entendem e respostas são enviadas em tempo hábil. Com isso, podemos destacar dois importantes pontos a serem observados quando pensamos em uma API: a **uniformização de interfaces** (o “I” da sigla) e a **agilidade no processo de comunicação**. A uniformização de interfaces é um requisito básico de arquitetura de qualquer sistema _web_, sendo que o entendimento entre clientes e servidores irá depender do quão padronizada, documentada e respeitada é a interface que rege a comunicação.

Com relação à **agilidade** no processo de comunicação, o cenário ideal seria aquele em que o tempo entre uma requisição de um cliente e a resposta de um servidor fosse quase nulo. Dessa forma, requisitar algo de um servidor seria como acessar um método de uma função de um objeto local. O meio e a distância seriam completamente transparentes à aplicação. No mundo atual, a distância entre as partes está cada vez maior e o meio, a internet, não para de evoluir, mas ainda existem limites físicos que impedem o cenário ideal.

### Estilos de comunicação

Uma das primeiras decisões a serem tomadas durante o processo de planejamento e desenvolvimento de uma API é relativa ao estilo de comunicação que será implementado. Se uma aplicação _web_ é composta por mais de um componente, como será feita essa comunicação? Qual será o estilo de comunicação que irá guiar o desenvolvimento da API?

Quando falamos de estilos de APIs, falamos de estilos de arquitetura das “pontes”. Os dois estilos mais comuns atualmente são o **SOAP** e o **REST**. Um outro, que vem ganhando espaço e poderá assumir um possível posto de liderança, é o **GraphQL**. Conheça-os melhor:

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/01.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/02.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/03.png]]

O primeiro estilo destinado à comunicação entre sistemas foi o **SNA (Systems Network Architecture)**, criado em 1974. Desenvolvido pela IBM, especificava convenções comuns para a comunicação entre uma grande sequência de dispositivos, sistemas e plataformas.

Desde então, muitas outras propostas de estilos de arquitetura para APIs surgiram, como: RPC (Remote Procedure Call), SOAP (Simple Object Access Protocol), REST (Representational State Transfer) e GraphQL. Cada uma dessas propostas definia um novo padrão ou protocolo de troca de mensagens, com suas vantagens e desvantagens em termos de recursos, desempenho, segurança e complexidade.  
  

Em comum a todos esses padrões, o objetivo de estreitar a comunicação entre cliente e servidor e o desejo de tornar essa comunicação o mais transparente e ágil possível, a ponto de a requisição de um recurso a um servidor ser tão simples quanto uma chamada a uma função de um objeto local do cliente.

**Nesta aula, vamos focar as opções que ainda são mais comuns: RPC, SOAP, REST e GraphQL.** Nosso objetivo não é identificar a melhor, mas a que melhor pode entregar valor a um dado projeto. A escolha do estilo deve resultar de uma discussão abrangente entre as partes envolvidas do projeto, não estando atrelada somente a requisitos funcionais do sistema, mas também a interesses de negócio.

#### RPC

Um dos primeiros dessa lista de estilos é o RPC, ou Remote Procedure Call (Chamada Remota de Procedimento). O objetivo principal do RPC é **permitir a comunicação entre sistemas distribuídos e heterogêneos, em que os componentes podem ser implementados em diferentes linguagens de programação e diferentes plataformas.**

A lógica do RPC é bem simples: um cliente pode solicitar que um servidor execute uma função ou procedimento remoto e receber os resultados de volta. Junto com essa solicitação, também são enviados os parâmetros necessários para sua execução. Nessa comunicação, tanto o servidor quanto o cliente irão fazer chamadas, e o que vai diferenciá-las são os parâmetros enviados. Um não precisa conhecer detalhes técnicos sobre como o outro foi implementado, mas é vital que seja capaz de entendê-lo.

Para que a comunicação seja possível, o pacote enviado pelo cliente ao servidor precisa ser interpretável por este. O mesmo vale para quando o servidor enviar uma resposta. Ambos os lados precisam compreender os comandos e parâmetros que são enviados. Uma componente importante nesse processo é a função **_stub_**, cujo principal objetivo é promover transparência no processo. **O _stub_ age como um intermediário entre o cliente e o servidor, permitindo que eles se comuniquem pela rede de forma transparente.**

O _stub_ é gerado pelo compilador a partir da descrição do serviço ou interface remota, sendo usado para encapsular a comunicação entre o cliente e o servidor. A figura a seguir apresenta o processo de comunicação com o RPC:

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb2.png]]

Quando um cliente chama uma função remota, usa o _stub_ para fazer a chamada parecer uma chamada de função local. Ainda do lado cliente, ele será responsável por **empacotar** (serializar) os argumentos da função em um formato que pode ser transmitido pela rede, enviar a solicitação para o servidor, aguardar a resposta e, em seguida, **desempacotar a resposta e retorná-la para o cliente**. Do lado do servidor, um cenário similar: o stub recebe a solicitação do cliente, **desempacota os argumentos** e chama a função remota. Em seguida, **serializa a resposta e a envia de volta** para o cliente através da rede.

![[stb3 1.png]]

Para ilustrar como funciona essa comunicação, vamos tomar como base a [[stb3 1.png |Figura 2]], intitulada **etapas da comunicação no RPC**. Nesse cenário, temos: o cliente enviando um comando (iniciando uma _procedure_) com uma coleção de parâmetros para um servidor (etapas 1 a 5); o servidor executando _procedures_ de acordo com os parâmetros especificados (etapa 6); e o caminho da resposta até o cliente (etapas 7 a 11). Explorando cada uma dessas etapas, temos que: (1) o cliente vai fazer uma chamada, definindo um conjunto de parâmetros que (2) serão empacotados (serializados) pelo _stub_ cliente, que, por sua vez, irá requisitar o (3) envio do pacote ao servidor. Uma vez que o pacote é recebido pelo servidor (4), o _stub_ deste irá (5) desempacotá-lo, recuperando a _procedure_ e seus parâmetros, que, então, serão executados pelo servidor (6). De posse de uma resposta à execução da _procedure_, o servidor utiliza novamente o _stub_ para empacotar (7) e, em seguida, enviar o pacote de resposta para o cliente (8). O caminho, agora, é simples: chegando ao cliente (9), será desempacotado (10) e, então, processado por este (11).

Existem vários modelos de implementação da comunicação via RPC. O Institute of Electrical and Electronics Engineers (IEEE) define o RPC na ISO/IEC CD 11578, com recomendações para sua implementação. O XML-RPC e o JSON-RPC são exemplos de padrões que seguem o modelo RPC. Sua principal diferença está no formato de dados utilizado: o XML-RPC usa XML para codificar os dados da solicitação e resposta, enquanto o JSON-RPC usa JSON. Vamos explorar esses dois padrões nos tópicos a seguir.

##### XML-RPC e JSON-RPC

O XML-RPC é uma das primeiras variações do padrão RPC que o implementa, utilizando o XML para a codificação de suas chamadas e o HTTP como mecanismo de transporte. Sua primeira versão, criada pela Microsoft, surgiu em 1998. A ideia era aproveitar a versatilidade do protocolo HTTP/1.0, abstraindo as chamadas RPC em requisições do tipo POST, em que o corpo da mensagem teria um conteúdo em XML. Esse XML, por sua vez, teria uma estrutura bem definida, obedecendo às especificações do [XML-RPC.](http://xmlrpc.com/spec.md)

A última atualização do XML-RPC foi em 2003 e, mesmo assim, ainda encontramos aplicações que utilizam esse padrão. Como já mencionado, o intervalo de tempo entre as requisições e a resposta é importante, e a natureza do XML pode ser um problema, nesse aspecto. O XML é conhecido por ser muito verboso, ou seja, permite muito texto para pouca informação útil, representando um gasto, que pode ser excessivo, de espaço em memória. **Quanto maior for o corpo da mensagem, maior pode ser o número de pacotes a serem transmitidos (mais lento será o completo envio de uma mensagem) e maior será o tempo gasto processando toda a informação.**

Para reduzir o tamanho da informação a ser transportada, surge, em 2005, uma nova variação de implementação do RPC, utilizando JSON para a codificação das chamadas: [JSON-RPC](https://www.jsonrpc.org/specification). O formato da informação em JSON é bem menos verboso, o que, consequentemente, reduz o tamanho dos dados a serem transportados. A versão mais recente da especificação do padrão é de 2013.

Ambos os tipos de RPC ainda são populares e podem ser encontrados em sistemas atuais. O RPC foi perdendo popularidade ao longo do tempo, com o surgimento de novos estilos, mas, em 2015, surgiu o gRPC, e esse cenário mudou.

##### gRPC

O gRPC, criado inicialmente pelo Google, é uma variação do RPC. À época de sua criação, era chamado de Stubby, e seu objetivo era conectar uma grande quantidade de microsserviços do Google que eram executados dentro e fora de seus _data centers_ ao redor do mundo. Só em 2015, mais de uma década após sua criação, o Google resolveu criar uma nova versão do Stubby e lançá-la como código aberto, passando a se chamar gRPC.

**Com o gRPC, uma aplicação cliente pode chamar diretamente um método em uma aplicação servidor que está em outra máquina, como se fosse uma chamada a um objeto local**. Assim como todo sistema RPC, o gRPC é baseado em torno da ideia de definição de um serviço, especificando métodos que podem ser chamados remotamente com seus parâmetros e retornos. Do lado do servidor, o servidor implementa suas interfaces e executa um servidor gRPC que vai lidar com as conexões dos clientes. Do lado do cliente, este tem um _stub_ que oferece os mesmos métodos implementados no servidor. gRPCs clientes e servidores podem executar e conversar uns com os outros em vários ambientes, desde um servidor remoto na _cloud_ até um computador pessoal. Além disso, **podem ser escritos em diferentes linguagens de programação**. Por exemplo, o gRPC servidor pode ser escrito em C++ e os clientes, em Ruby, Python, Go ou Java.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb4 1.png]]

A figura anterior ilustra, de forma simplificada, essa troca de mensagens. Algumas grandes diferenças em relação ao RPC tradicional estão na **simplificação do processo** e na forma como a informação é encapsulada para envio. De fato, a mensagem enviada é serializada por [_protocol buffers_](https://protobuf.dev/overview/) que possibilitam a conversão de parâmetros e resultados em uma forma neutra, independente de uma linguagem de programação. Segundo o _site_ oficial, o resultado dessa serialização é uma informação estruturada como se fosse um JSON, exceto que menor e mais rápida de transportar pela rede. Na imagem, “protorrequisição” e “protorresposta” fazem alusão ao processo de empacotamento do comando/resposta.  
  
Hoje, grandes serviços _on-line_, como Netflix, mantêm toda ou boa parte da comunicação entre seus microsserviços em gRPC. A versatilidade, a leveza e a capacidade de integração do gRPC fazem com que seja um dos preferidos na comunicação de microsserviços, onde centenas de milhares de conexões são feitas diariamente, o que faz necessário APIs de alta performance para otimizar a camada de comunicação.


### SOAP

O SOAP foi criado em 1998 pela Microsoft, logo após a criação do XML-RPC, buscando um padrão que pudesse ser universal. Assim, foi submetido à W3C (World Wide Web Consortium) e, em 2000, o SOAP 1.1 foi oficialmente reconhecido como um padrão aberto e independente de plataforma.

O SOAP define a forma de codificar objetos em formato XML e enviá-los pela rede usando protocolos como HTTP e SMTP (Simple Mail Transfer Protocol). O uso do protocolo SMTP para o SOAP não é comum hoje, por não ter sido projetado para lidar com estruturas de dados complexas em XML, algo que pode tornar a codificação e decodificação de mensagens SOAP propensa a erros. Além disso, o SMTP não oferece suporte a recursos avançados de segurança, como criptografia de ponta a ponta, o que pode comprometer a privacidade dos dados em trânsito. Por último, também pode haver problemas de escalabilidade, uma vez que o SMTP não é otimizado para a transmissão de grandes volumes de dados.  
  

No XML-RPC a tipagem dos dados a serem trafegados junto à mensagem não é clara. Já no SOAP, para garantir a consistência dos dados, estes devem ter um tipo bem definido. Essa característica garante a consistência, mas com um custo: as mensagens serão necessariamente verbosas (muito texto adicionado para garantir a definição dos tipos).

Como já comentado, a estrutura (corpo) da mensagem na comunicação com o SOAP segue um padrão que é estruturado em XML. Uma mensagem SOAP consiste em um envelope SOAP que encapsula o corpo da mensagem e que pode incluir um cabeçalho (opcional). No código apresentado a seguir, temos um breve exemplo da estrutura de uma mensagem em SOAP:

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb5.png]]

O **soap:Envelope** é o elemento-raiz da mensagem e define o _namespace_ que ela usa. O **soap:Header** é um elemento opcional e pode conter informações adicionais de cabeçalho, como dados de autenticação ou informações de transação. Já o **soap:Body** é o elemento que contém o conteúdo da mensagem, que pode ser qualquer elemento XML compatível com o esquema XML definido para ela.

O namespace é uma identificação única usada para definir o formato e a estrutura dos elementos e atributos O namespace é um URI Uniform Resource Identifier que identifica um conjunto único específico de elementos e atributos definidos para uso em mensagens SOAP. O namespace padrão para mensagens SOAP é definido pela W3C e é geralmente especificado como 'http://www.w3.org/2003/05/soap-envelope' para o SOAP 1.2 e 'https://schemas.xmlsoap.org/soap/envelope/' para o SOAP 1.1.

Na resposta a uma requisição, quando há uma falha, o servidor retorna uma mensagem de estrutura similar, mas com um elemento **Fault** em seu corpo. Esse elemento Fault contém três possíveis informações, que irão ajudar o código cliente a determinar o motivo da falha: (1) **Code**, que irá informar uma breve identificação do erro; (2) **Reason**, que pode conter uma descrição textual do erro; e **Detail**, que pode trazer informações adicionais sobre o motivo do erro. Segue um exemplo de um corpo de mensagem que traz um erro:

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb6.png]]

A figura a seguir apresenta a estrutura final da mensagem em SOAP, junto com exemplos. Você pode aprofundar seus estudos sobre o SOAP com a documentação mantida pela [W3C](https://www.w3.org/TR/soap/).

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb7 1.png]]

Após a criação do REST, o SOAP perdeu muita popularidade, mas ainda está presente no dia a dia. Um dos motivos para isso é sua maturidade em termos de segurança, especialmente pela extensão [WS-Security](https://www.ibm.com/docs/pt-br/integration-bus/10.0?topic=configuration-ws-security), que permite a criptografia dos dados trafegados.

Outra característica do SOAP é que ele possibilita o **encadeamento de mensagens** à medida que são recebidas, permitindo ao servidor um maior contexto para o tratamento de uma mensagem. Isso torna o armazenamento um desafio para o servidor, mas é importante quando uma sequência de mensagens está relacionada a uma transação complexa, como a compra de uma passagem área, por exemplo: após uma primeira requisição, o servidor pode memorizar as datas pesquisadas pelo usuário e, com isso, em uma segunda requisição (em uma nova consulta), basta informar o novo destino que já é possível retornar um resultado de busca.

### REST

O REST é um dos estilos mais usados atualmente na construção de APIs. Ele foi apresentado pela primeira vez em uma tese de doutorado de Roy Fielding, em 2000. Antes de falar do REST, é interessante entender um pouco do trabalho de seu criador

**Roy Fielding** é cofundador do Apache HTTP [Server Project](https://httpd.apache.org/) e, em 1993, propôs um caminho para a continuidade da expansão da _web_, que estava em risco à época, devido ao completo descompasso com a evolução da tecnologia, sendo um ambiente com pouca padronização na forma e no uso de recursos.

A proposta de Fielding era que a escalabilidade da _web_ fosse governada por um conjunto de requisitos-chaves (_key constraints_). Segundo ele, a continuidade da expansão seria possível se cada uma dessas restrições fosse atendida de forma igual. Essas restrições/limitações continuam atuais, pois os conceitos ainda são válidos, e devem ser observadas e atendidas no desenvolvimento de todo e qualquer sistema _web_ (COOKSEY, 2016). Fielding as categorizou em seis grupos: cliente-servidor; uniformidade de interfaces; sistema em camadas; uso de _cache_; ausência de estado; e disponibilização de código sob demanda.

Além da relevância para a evolução da _web_ que temos hoje, Fielding também foi um dos autores originais da especificação do [HTTP/1.0](https://www.w3.org/Protocols/HTTP/1.0/spec) e o principal autor da especificação [HTTP/1.1](https://www.w3.org/Protocols/rfc2616/rfc2616.html). Como se não fosse o bastante, em sua tese de doutorado, se dedicou ao estudo da arquitetura de sistemas distribuídos, mais precisamente à definição de um novo estilo, o REST.

Com isso, o REST é um estilo fortemente focado na ideia de recursos, ao contrário do SOAP e do RPC, que utilizam comandos para manipular o servidor. Um recurso é um dado real, que está acessível ou é gerado pelo servidor. Por esse motivo, o REST é um padrão que faz uso do protocolo HTTP e dos métodos GET, POST, PUT e DELETE para a manipulação de recursos.

Além disso, em vez de especificar a estrutura de uma mensagem, o REST sugere requisitos que devem ser observados: os mesmos propostos por Fielding para a garantia da expansão e escoabilidade da _web_. Por exemplo: a uniformização na identificação de recursos com o uso de URIs (Uniform Resource Identifiers) e o uso de representações de recursos em formatos como JSON ou XML.

### GraphQl

Como o REST é focado na entrega de recursos, se torna necessária a construção de várias rotas. Um exemplo de cenário: supondo uma API de consulta de usuários, haverá uma rota que, com base nos parâmetros recebidos, retornará os dados de um usuário. Digamos que vai haver uma rota do tipo “/user/<id/>”, que vai receber um id do usuário e retornar toda a coleção de informações disponíveis para ele. Agora, imagine um cenário em que a aplicação precisa somente acessar o nome completo do usuário. Temos duas opções: a primeira é utilizar a rota “/user/<id/>”, que recebe todo o conteúdo sobre o usuário e utiliza apenas seu nome. A segunda é criar uma nova rota, que retorna apenas o nome completo do usuário com base no id. Nenhuma das duas opções é a ideal. Na primeira, muitos dados poderão trafegar na rede e, depois, terão que ser tratados na aplicação cliente sem necessidade. Na segunda, o cenário é melhor, mas implica a criação de uma nova rota. A lógica de criar uma nova rota para cada dado individual necessário é insustentável.

É nesse contexto que surge a proposta do GraphQL, criado pelo Facebook em 2012 e lançado publicamente em 2015. À época, o objetivo era resolver problemas que o Facebook enfrentava em sua API. **O GraphQL não é exatamente um estilo, mas uma linguagem de consulta para APIs, desenvolvida com base em princípios de arquiteturas, como os observados no REST.**

Voltando ao cenário anterior, se o cliente precisa somente do nome completo de um usuário, pode pedi-lo, sem a necessidade de uma nova rota ou o tratamento de uma longa resposta.

O GraphQL também oferece recursos adicionais, como **introspecção de esquema e tipagem de dados**, que podem tornar mais fácil para os desenvolvedores entender e interagir com uma API. Sobre a tipagem de dados, fornece uma estrutura para descrever os tipos de dados disponíveis na API e as operações que podem ser executadas neles, permitindo uma documentação clara e consistente da API.

Com o tempo, o GraphQL se tornou cada vez mais popular e, agora, é usado por muitas empresas e organizações, como GitHub, Airbnb, Shopify e Pinterest. O GraphQL é considerado uma alternativa **mais flexível e poderosa** às APIs REST tradicionais e está se tornando cada vez mais importante no mundo do desenvolvimento de aplicativos.

### Estilo e suas melhores utilizações

![[Pasted image 20240725165731.png]]

#### RPC
![[Pasted image 20240725165700.png]]

![[Pasted image 20240725163401.png]]

![[Pasted image 20240725163128.png]]

#### SOAP
![[Pasted image 20240725163322.png]]

![[Pasted image 20240725163538.png]]

#### REST
![[Pasted image 20240725163949.png]]

![[Pasted image 20240725164026.png]]

![[Pasted image 20240725164059.png]]

#### GraphQL
![[Pasted image 20240725164233.png]]

![[Pasted image 20240725164307.png]]

### Referências:

BIEHL, M. **REST API design rulebook**: designing consistent RESTful web service interfaces. Sebastopol: O’Reilly Media, 2011.

COOKSEY, B. **An introduction to APIs**. Columbia: Zapier, 2016..

DATATRACKER. RFC 2616: hypertext transfer protocol – HTTP/1.1. **Datatracker**, 1999. Disponível em: [https://datatracker.ietf.org/doc/html/rfc2616](https://datatracker.ietf.org/doc/html/rfc2616). Acesso em: 9 maio 2023.

GEEWAX, J. J. **API design patterns**. Shelter Island: Manning, 2021.

GOOGLE. Protocol buffers documentation. **Protocol Buffers**, [20--?]. Disponível em: [https://protobuf.dev/overview/](https://protobuf.dev/overview/). Acesso em: 9 maio 2023.

gRPC. Introduction to gRPC. **gRPC**, 2023. Disponível em: [https://grpc.io/docs/what-is-grpc/introduction/](https://grpc.io/docs/what-is-grpc/introduction/). Acesso em: 9 maio 2023.

IBM. WS-security. **IBM**, [20--?]. Disponível em: [https://www.ibm.com/docs/pt-br/integration-bus/10.0?topic=configuration-ws-security](https://www.ibm.com/docs/pt-br/integration-bus/10.0?topic=configuration-ws-security). Acesso em: 9 maio 2023.

SHKLAR, L.; ROSEN, R. **Web application architecture**: principles, protocols and practices. 2. ed. Chichester: John Wiley & Sons, 2009.

THE GRAPHQL FOUNDATION. Introduction to GraphQL. **GraphQL**, [20--?]. Disponível em: [https://graphql.org/learn/](https://graphql.org/learn/). Acesso em: 9 maio 2023.

W3C. Simple object access protocol (Soap) 1.1. **W3C**, 2007. Disponível em: [https://www.w3.org/TR/soap/](https://www.w3.org/TR/soap/). Acesso em: 9 maio 2023.

## Teste e Publicação (Aula 3)

Em 2022, uma das maiores plataformas para o desenvolvimento de APIS, a **Postman**, publicou um [relatório](https://voyager.postman.com/doc/postman-state-of-the-api-2022.pdf) com os resultados de uma pesquisa que envolveu 37.000 desenvolvedores ao redor do globo. Um dos resultados apresentados nesse relatório é que 51% dos entrevistados responderam que **mais da metade do esforço**, nas empresas em que trabalham, é destinada ao desenvolvimento de APIs. Em 2020, apenas 40% deram a mesma resposta, e, no ano seguinte, foram 49%. Além disso, **89% dos entrevistados acreditam que o investimento com APIs deve se manter ou crescer nos próximos 12 meses**.

Esses resultados evidenciam o crescimento do investimento no desenvolvimento de APIs e do seu papel como “blocos de montar” no desenvolvimento de sistemas modernos. Entretanto, um dos obstáculos mais citados durante as entrevistas foi a **falta de mão de obra especializada** no projeto e desenvolvimento de APIs, o que indica que **ainda há muito espaço de crescimento nessa área.**

No que diz respeito aos testes de código, o relatório mostrou que a grande maioria dos entrevistados afirmou fazer **apenas testes funcionais e de integração** (68% e 67%, respectivamente), um grande sinal de alerta, visto que cada vez mais sistemas são produzidos integrando APIs, “montando blocos”, no caso sistemas que irão também depender da qualidade das APIs que irão utilizar para poder atestar a sua própria qualidade.

### Testes no desenvolvimento de uma API

Quando o assunto é desenvolvimento de APIs, existe uma série de testes específicos que visam a avaliar e validar a **coerência, a corretude, a _performance_, a usabilidade e a segurança** da solução desenvolvida. Aqui vamos explorar aqueles tipos de testes mais comuns no desenvolvimento de APIs: os **testes unitários, de integração, aceitação, carga e segurança.**

#### Testes unitários

Os **testes unitários**, ou testes funcionais, visam a verificar o comportamento individual de unidades isoladas de código, como funções, métodos ou classes. **Eles garantem que cada unidade funcione corretamente de acordo com suas especificações.** No cenário das APIs, também podemos incluir como teste de unidade os testes de rotas – a implementação de uma rota como uma unidade isolada de código.

Para ilustrar, podemos pensar na **função que serve uma rota** – que recebe os parâmetros e, com base nos parâmetros, **constrói e retorna uma resposta.**

No teste unitário, **simulamos uma chamada real, com parâmetros reais** (ou, no mínimo, coerentes com a especificação), e verificamos se a resposta retornada está correta em relação ao que era esperado.

No código a seguir, veja um exemplo de teste para uma rota GET que recebe um parâmetro de id no formato “/api/resource/<id/>”. O valor do id é fornecido como uma variável chamada test_id no teste (linha 14).

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb1 1.png]]

Nesse exemplo, a classe TestGetRoute herda da classe TestCase fornecida pelo flask_testing e implementa o método create_app(), que cria uma instância da aplicação Flask para a execução dos casos de teste. No caso, temos apenas um caso de teste representado pelo método test_get_route_with_id(), em que definimos um valor de teste para o id (linha 14), nesse caso 123. Em seguida, usamos o cliente de teste self.client para fazer uma requisição GET à rota com o id fornecido (linha 15). A partir da linha 17, faz-se uma série de verificações sobre o resultado da requisição, como o _status_ da resposta (linha 18) e se o conteúdo retornado está de acordo com o esperado (linhas 21 a 35).

Um detalhe importante sobre os testes unitários é que nesse tipo de teste simulamos integrações com módulos e componentes externos; não há conexões ou chamadas reais. Observe que, no código de exemplo mostrado, não há uma chamada “real” à rota, mas uma simulação de chamada. O objetivo é garantir que a execução dos testes unitários não dependa da execução de outros sistemas e/ou componentes externos. Quem for executar esses testes não irá precisar conhecer e saber manipular essas integrações.

#### Testes de Integração

Quando o objetivo é verificar de fato o comportamento de um sistema quando integrado a uma aplicação externa real, utilizaremos os **testes de integração.** Nesse tipo de teste, temos um **escopo maior de atuação e testamos a interação entre as diferentes partes da API e suas dependências externas**, como bancos de dados, serviços _web_ ou outras APIs. Esses testes garantem que os componentes da API se comuniquem corretamente e que as integrações externas estejam funcionando conforme o esperado.

Como ilustração simples, podemos pensar no caso do teste de uma rota que faz chamadas ao banco de dados.

Imagine que essa rota solicita a atualização de dados de cadastro de um cliente.

**No teste de integração, teremos um caso de teste que irá simular a chamada à rota, passando como parâmetros uma coleção correta de dados, e, em seguida, serão feitas a verificação e a validação automatizadas do estado do banco, para verificar se de fato a atualização solicitada foi executada.**

O código a seguir ilustra esse cenário de teste de integração entre uma aplicação web com o seu banco.

![[stb2 1.png]]

Nesse exemplo, muito similar ao exemplo anterior, foi utilizada a **biblioteca pymysql para interagir com um banco de dados MySQL.** No método setUp(), é criado um banco de dados test_db, que será destruído pelo método tearDown() após a execução de cada caso de teste – no caso, temos apenas um caso de teste no método test_update_route().

Dentro do método test_update_route(), primeiro está sendo criado um usuário de teste no banco de dados com um _e-mail_ e endereço iniciais (linhas 34-37). Em seguida, na linha 40, é recuperado o id do usuário de teste inserido para realizar a atualização.

Entre as linhas 47 e 52, é feita a requisição de atualização definindo os novos valores de _e-mail_ e endereço. Nas linhas seguintes, são feitas as verificações no banco de dados para validar se de fato a atualização foi corretamente feita pela API.

Esse tipo de teste tem geralmente **alto custo** de desenvolvimento, mas **alto valor de entrega**. Com ele, podemos identificar com muita antecedência conflitos entre componentes e antecipar correções, minimizando impactos e evitando interrupções de serviço. Ele não precisa ser executado somente quando há código novo. É indicado que os testes de integração sejam executados a cada nova atualização de código ou de qualquer componente externo que se relacione com o sistema.

#### Testes de aceitação

**Quando queremos verificar se a API atende aos requisitos e aos comportamentos esperados pelo usuário final, fazemos testes de aceitação,** também conhecidos como testes funcionais ou testes de aceitação do usuário. Esses testes são escritos do ponto de vista do usuário e **testam os fluxos de uso principais da API** para garantir que ela funcione corretamente em cenários reais de uso. Esses cenários reais são geralmente escritos junto com cliente ou com seus representantes.

Para ilustrar um caso de teste de aceitação, no código apresentado a seguir temos um teste de aceitação de uma rota de _login_ de uma API; **quando o usuário é validado com sucesso, ela retorna um _token_.**

![[stb3 2.png]]

No código, de forma muito similar aos outros apresentados aqui, dentro da classe de teste temos **dois métodos de teste: test_successful_login e test_failed_login.** O primeiro método verifica se **é possível fazer _login_** com sucesso, fornecendo um _e-mail_ e senha válidos. O segundo método verifica se **uma mensagem de erro é retornada** quando são fornecidas credenciais inválidas.

Dentro de cada método de teste, é realizada uma requisição POST para a rota de _login_ utilizando o cliente de teste self.client. Em seguida, verificam-se o código de _status_ da resposta e o conteúdo da resposta para garantir que as respostas estejam corretas.

#### Testes de carga

Já os testes de carga e desempenho **avaliam a capacidade da API de lidar com cargas de trabalho intensas e medem seu desempenho sob condições de alto tráfego.** Eles ajudam a identificar gargalos de desempenho, tempos de resposta lentos e limites de escalabilidade, permitindo otimizações e ajustes adequados.

Para um projeto de API desenvolvido em Python, temos a opção de ferramentas como a [Locust](https://locust.io/), que permite simular múltiplos usuários acessando a API simultaneamente. A configuração de um teste de carga utilizando essa ferramenta é simples. O código a seguir apresenta o código de configuração de uma API que implementa apenas uma rota de _login_.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb4 2.png]]

No código apresentado, é criada uma classe MyUser que herda da classe HttpUser do Locust. **A classe MyUser define um usuário que fará _login_ na API.** O método _login_ da classe representa uma ação de _login_ de um usuário válido. Entre as linhas 11 e 14, estamos estabelecendo os cenários de sucesso e falha. Na Técnica aplicada, vamos voltar a falar dessa ferramenta com um exemplo prático.

![[pos-graduacao/2º Acervo de imagens (Disc. 1)/stb6 1.png]]

#### Teste de segurança

Por fim, os testes de segurança **avaliam a resistência da API a ameaças de segurança**, como injeção de código, ataques de negação de serviço, autenticação inadequada, entre outras. Eles garantem que a API esteja protegida contra vulnerabilidades conhecidas e cumpra as melhores práticas de segurança.

Um exemplo simples de segurança é o **teste de autenticação e autorização**, que é ilustrado no código apresentado a seguir. Nesse teste, o objetivo é verificar se a API está devidamente protegida contra acessos não autorizados e se as regras de autenticação e autorização estão sendo aplicadas corretamente. Isso envolve **garantir que apenas usuários autenticados e autorizados tenham acesso aos recursos protegidos.**

![[stb6 2 1.png]]

No código apresentado, dentro da classe de teste, temos dois métodos de teste: **test_unauthenticated_access_to_protected_route e test_authenticated_access_to_protected_route.** O primeiro método verifica se o acesso não autenticado à rota protegida retorna o código de _status_ 401 (não autorizado). O segundo método de teste simula o acesso autenticado à rota protegida fornecendo um _token_ de autenticação válido no campo Authorization do cabeçalho da requisição. Em seguida, verifica se o código de _status_ da resposta é 200 (OK) e se a mensagem de sucesso é retornada.

Esse código poderia ser facilmente adaptado adicionando mais casos de teste para verificar diferentes cenários de autenticação e autorização, como tentativas de acesso com _tokens_ inválidos, acesso a recursos protegidos por diferentes papéis de usuário, entre outros.

### Qual teste utilizar?

É importante combinar diferentes tipos de testes ao desenvolver uma API, pois cada um aborda aspectos específicos e oferece diferentes níveis de garantia de qualidade. **A escolha dos testes a serem aplicados depende das necessidades e requisitos do projeto, bem como das melhores práticas de desenvolvimento e qualidade de _software_.**

Na Técnica Aplicada, vamos dar foco aos testes e vamos explorar cada um dos tipos de testes apresentados nesta aula. Vamos mostrar como podem ser simples e importantes o uso e a construção de testes.

### Código testado, falta agora a publicação

A publicação de uma API é o processo de **tornar a API acessível aos usuários e clientes** para que possam interagir com ela. Existem várias formas de publicar uma API REST, e a escolha da abordagem depende de vários fatores, como os requisitos do projeto, o ambiente de hospedagem e as necessidades de escalabilidade.

Seguindo uma abordagem mais tradicional, é possível hospedar a API em um servidor dedicado, em uma máquina virtual ou em um provedor de hospedagem. Nessa abordagem, você instala o servidor _web_ (por exemplo, [Nginx](https://www.nginx.com/)) e implanta a API como um aplicativo nesse servidor. Isso requer a configuração e o gerenciamento do ambiente de hospedagem, incluindo a instalação de dependências e a configuração adequada do servidor.

Uma opção mais simplificada é utilizar uma plataforma de nuvem que fornece serviços gerenciados para hospedar e executar a API. Exemplos populares incluem o [Google Cloud Platform](https://cloud.google.com/?hl=pt-br) (GCP), o [Microsoft Azure](https://azure.microsoft.com/) e o [Amazon Web Services](https://aws.amazon.com/pt/) (AWS). Essas plataformas fornecem serviços de hospedagem gerenciados, como o Google App Engine, o Azure App Service e o AWS Elastic Beanstalk, que cuidam da infraestrutura subjacente, da escalabilidade e do gerenciamento.

Outra opção bem popular é o uso de contêineres, como **Docker**, e orquestradores de contêineres, como **Kubernetes ou Docker Swarm**. Você pode empacotar sua API REST em um contêiner e implantá-lo em um ambiente de orquestração que gerencia a execução e o dimensionamento dos contêineres. Isso fornece uma implantação consistente, escalabilidade horizontal e gerenciamento simplificado da infraestrutura.

Independentemente da abordagem escolhida para a publicação de uma API REST, é importante considerar aspectos como segurança, desempenho, monitoramento e documentação. Além disso, é fundamental realizar testes rigorosos da API antes da publicação para garantir que ela esteja funcionando corretamente e atenda aos requisitos de negócios. Isso inclui testes de unidade, testes de integração, testes de carga e testes de segurança.

### Conteinerização de uma aplicação

![[Pasted image 20240726154647.png]]

![[Pasted image 20240726154828.png]]

![[Pasted image 20240726155420.png]]

### Gerenciamento de contêineres

Um dos principais desafios no uso do Docker é a complexidade do gerenciamento de contêineres. Embora o Docker facilite a criação e o empacotamento de aplicativos em contêineres isolados, o gerenciamento desses contêineres pode se tornar complicado à medida que o número deles aumenta. É necessário lidar com questões como escalabilidade, balanceamento de carga, monitoramento e atualização de contêineres, o que pode exigir habilidades adicionais e uma compreensão profunda da infraestrutura.

Para facilitar esse gerenciamento, sugiram tecnologias como o Kubernetes, que têm como objetivo facilitar a orquestração e o gerenciamento de contêineres em escala, oferecendo um ambiente robusto para implantar, escalar e manter aplicativos em contêineres, independentemente do tamanho e da complexidade da aplicação que está no contêiner.

Com o [Kubernetes](https://kubernetes.io/), é possível automatizar tarefas como o provisionamento de recursos, o balanceamento de carga, a recuperação de falhas e a escalabilidade horizontal. Ele também oferece uma maneira padronizada de lidar com serviços de rede, armazenamento e monitoramento, facilitando a construção de aplicativos distribuídos e altamente disponíveis.

O Kubernetes é considerado a plataforma de orquestração de contêineres mais popular e amplamente adotada atualmente. Ele ganhou grande popularidade e se tornou o padrão de fato para gerenciamento de contêineres em escala. No entanto, apresentamos uma breve listagem de outras tecnologias que, assim como o Kubernetes, têm como objetivo auxiliar no provisionamento de aplicações com conteinerização:  
  

- [Docker Swarm](https://docs.docker.com/engine/swarm/): o Docker Swarm é uma ferramenta nativa do Docker para orquestração de contêineres.

- Apache Mesos: o Apache Mesos pode ser usado para executar aplicativos em contêineres, juntamente com outras cargas de trabalho, como tarefas de processamento de dados em lote ou em tempo real.

- [Amazon Elastic Container Service](https://aws.amazon.com/pt/ecs/) (ECS): o Amazon ECS é um serviço de orquestração de contêineres fornecido pela Amazon Web Services (AWS). Ele permite executar e gerenciar aplicativos em contêineres na nuvem da AWS.

- [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine?hl=pt-br) (GKE): o Google Kubernetes Engine é um serviço gerenciado do Google Cloud Platform (GCP) para execução de contêineres no Kubernetes. O GKE facilita a configuração e a operação de _clusters_ Kubernetes, permitindo que as equipes se concentrem no desenvolvimento de aplicativos.

- [HashiCorp Nomad](https://www.hashicorp.com/products/nomad): o HashiCorp Nomad é uma plataforma de orquestração de cargas de trabalho que suporta não apenas contêineres, mas também outros tipos de tarefas, como aplicativos executáveis, tarefas de lote e cargas de trabalho de máquinas virtuais.

O Kubernetes é a opção mais popular e amplamente adotada, oferecendo recursos avançados, uma comunidade ativa e um ecossistema abrangente. No entanto, a escolha de uma tecnologia de orquestração de contêineres depende dos requisitos específicos do seu ambiente e dos objetivos do seu projeto. Ao tomar essa decisão, é importante considerar fatores como escalabilidade, complexidade, ecossistema de ferramentas e serviços, suporte da comunidade e compatibilidade com a infraestrutura existente.



Em um texto publicado na _Harvard Business Review_, intitulado “APIs não são apenas para empresas de tecnologia”, os autores comentam que as APIs são “blocos de montar” para a transformação digital. Ver APIs como blocos de montar é um ponto de vista que ressalta a ideia de venda de serviços pontuais. Por exemplo, o Google tem um gigantesco portfólio de APIs disponíveis para contratação; uma delas é a API do Cloud Vision, disponível na versão REST e gRPC. Essa API fornece um serviço de reconhecimento de entidades em imagens.

Supondo um projeto de sistema web que tem como objetivo organizar fotos de acordo com o conteúdo presente nelas, poderíamos utilizar essa API para fazer a extração de entidades para auxiliar na indexação. Agora, supondo que, além disso, seja interessante também identificar geograficamente o ponto onde a foto foi tirada a partir das coordenadas salvas no metadado da foto, poderíamos utilizar outra API apenas para identificar em um mapa o local. Se eu quiser agora gerar um _post_ para ser compartilhado em uma rede social, posso utilizar a API de uma rede social para fazer esse compartilhamento, e assim por diante. Com isso, temos um sistema cuja qualidade vai depender fortemente também da qualidade dos serviços que utiliza.

De acordo com o [estudo divulgado pela Postman em 2022](https://voyager.postman.com/doc/postman-state-of-the-api-2022.pdf), é crescente o esforço dedicado por empresas no desenvolvimento de APIs. Esse mesmo relatório também traz alguns alertas. São vários os obstáculos listados relacionados à produção e ao consumo de serviços via APIs. Entre os mais citados estão a falta de documentação, a falta de pessoas especializadas e o gerenciamento de APIs quando um sistema faz uso exagerado delas.

Diante desses obstáculos, quais as principais estratégias você acredita que poderiam aumentar o grau de confiança do usuário/cliente de uma API? Quão difícil ou custosa ela seria?

### Referências:

LOCUST. **Locust documentation**. Disponível em:[https://docs.locust.io/en/stable/](https://docs.locust.io/en/stable/). Acesso em: 22 maio 2023

NGINX. **Nginx documentation**. Disponível em: [https://nginx.org/en/docs/](https://nginx.org/en/docs/). Acesso em: 22 maio 2023.

POSTMAN. **2022 State of the API Report**. Disponível em:[https://voyager.postman.com/doc/postman-state-of-the-api-2022.pdf](https://voyager.postman.com/doc/postman-state-of-the-api-2022.pdf). Acesso em: 22 maio 2023.

SHKLAR, L.; ROSEN, R. **Web application architecture**: principles, protocols and practices. 2. ed. [_s.l._]: Wiley, 2009.
# Arquitetura de Microsserviços (Disciplina 2)
## Introdução à Arquitetura de Microsserviços (Aula 1)

### O que é arquitetura de _software?_

Arquitetura de _software_ é um termo difícil de se definir. Em um artigo para o _IEEE Software_, Martin Fowler coletou a seguinte definição de Ralph Johnson:

“Na maioria dos projetos de _software_ de sucesso, os desenvolvedores mais experientes trabalhando naquele projeto têm um entendimento compartilhado do projeto do sistema. Esse entendimento compartilhado é chamado de 'arquitetura'.  
Esse entendimento inclui como o sistema é dividido em componentes e como os componentes interagem por meio de interfaces. Esses componentes geralmente são compostos por componentes menores, mas a arquitetura inclui somente os componentes e interfaces que são entendidos por todos os desenvolvedores.”

É uma boa definição. No entanto, existem alguns pontos imprecisos. Por exemplo, o que é um “componente”? E por que os componentes menores não estão incluídos na arquitetura?

De fato, é difícil definir arquitetura de _software_ de forma precisa. De qualquer forma, é fácil intuir o que seja a arquitetura de um sistema e defini-la da maneira mais precisa possível. De maneira geral, gosto de imaginar a arquitetura como:  
  
Uma visão geral do sistema a partir de um _zoom-out_ que permite enxergar sua estrutura: os componentes maiores que o compõem e como esses componentes se comunicam.

“Componente” refere-se a um conjunto de módulos, e “módulo” refere-se a um agregado de funções e dados (em uma linguagem orientada a objetos, o módulo é uma classe com seus métodos – funções – e dados – atributos; em uma linguagem não orientada a objetos, pode ser um arquivo de código-fonte com funções e dados relacionados).

A meu ver, o termo **_arquitetura_** em **arquitetura de microsserviços** refere-se tanto à maneira como estruturamos o código do sistema quanto a aspectos de infraestrutura. Por exemplo, como veremos em breve, uma das características desejáveis nos microsserviços é que eles possam ser **implantados** independentemente. Isso se refere mais a uma estratégia de implantação (_deploy_) – e, portanto, uma característica de infraestrutura – do que à estrutura do código em si, porém essa estratégia também afeta a maneira como iremos estruturar o código.

Usando minha definição de **componente** apresentada, podemos entender cada microsserviço como um **componente** do sistema que implementa uma fatia do negócio. Esse componente contém um conjunto de módulos necessários para a sua implementação.

### O que são microsserviços?

Os microsserviços são serviços **modelados em torno de um domínio de negócios** que podem ser **lançados e implantados ​​independentemente**. Eles são um tipo de arquitetura orientada a serviços, embora tenham 'opiniões fortes' sobre como os limites de cada serviço devem ser traçados e nos quais a **capacidade de implantação independente é fundamental**. Eles são **agnósticos à tecnologia**, o que é uma das vantagens que oferecem.

![[Pasted image 20240729102121.png]]

![[Pasted image 20240729102605.png]]

Podemos ter por exemplo de um microsserviço para lidar com o frete de produtos vendidos.

Informalmente falando, podemos dizer que uma arquitetura de microsserviços é implementada como uma porção de _fatias_ do sistema, que podem ser desenvolvidas, testadas e implantadas independentemente.

Pense em um sistema grande que, em vez de estar implementado com todas as funcionalidades juntas em uma base de código única e com apenas um grande executável, agora é fatiado em vários serviços pequenos com seus executáveis próprios servidos distribuidamente em algum tipo de rede, comunicando-se uns com os outros.

Do lado de fora, um único microsserviço é tratado como um componente caixa-preta. Ele hospeda a funcionalidade de negócios em um ou mais _endpoints_ de rede (por exemplo, uma fila ou uma API REST, conforme mostrado na figura a seguir), sobre quaisquer protocolos apropriados. Os consumidores, sejam eles outros microsserviços ou outros tipos de programas que consomem algo produzido pelo serviço, acessam a funcionalidade oferecida pelo serviço por meio desses _endpoints_. Os detalhes internos da implementação (como a tecnologia em que o serviço é escrito ou a forma como os dados são armazenados) são **totalmente ocultos do mundo externo**.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03.png]]

Isso significa que as arquiteturas de microsserviços **evitam o uso de bancos de dados compartilhados na maioria das circunstâncias**. Em vez disso, **cada microsserviço encapsula seu próprio banco de dados, quando este é necessário**.

Os microsserviços adotam o conceito de **ocultação de informações**. Ocultar informações significa ocultar o máximo possível de informações dentro de um componente e expor o mínimo possível por meio de interfaces externas. Isso permite uma separação clara entre o que pode mudar facilmente e o que é mais difícil de mudar. A implementação ocultada do mundo externo pode ser alterada livremente, desde que as interfaces de rede expostas pelo microsserviço não sejam alteradas de maneira incompatível com versões anteriores. Mudanças dentro de um microsserviço não deveriam afetar outros microsserviços que consomem informações produzidas a partir dele. Isso é o que permite que ele seja independentemente lançado e implantado (talvez a característica mais importante dos microsserviços). Ter limites de serviço claros e estáveis ​​que não mudam quando a implementação interna muda resulta em sistemas com **baixo acoplamento** e **alta coesão**

### Principais conceitos relacionados com os microsserviços

Algumas ideias principais devem ser compreendidas ao explorar os microsserviços. Dado que alguns aspectos são frequentemente ignorados, é vital explorar esses conceitos mais a fundo para garantir que você entenda o que faz funcionar bem uma arquitetura de microsserviços. Os principais conceitos que eu gostaria que você entendesse nesse sentido estão relacionados com:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/07.png]]

1 - Implantação Independente:
	Microsserviços devem ser isoladamente implantados. Ex: Um acoplamento muito forte entre um par de microsserviços, impedindo dos mesmos serem tratados de forma isolada. Junto a implantação independente, é proporcionada a escala de microsserviço de maneira individualizada, como por exemplo: Um microsserviço com uma carga de requisições muito mais alta que outras, com a implantação independente, podemos escalar somente esse microsserviço, independente dos outros.

2 - Modelagem sobre um domínio de negócios:
	Os microsserviços devem equivaler a uma fatia do domínio de negócio (nicho de negócio), técnicas como _Domain-Driven Design_ (DDD), que focam a modelagem do sistema no domínio, podem ajudar a estruturar melhor o código dos microsserviços, para eles representarem o domínio real no qual operam.

3 - Gerenciamento do próprio estado:
	Cada microsserviço deve possuir e gerenciar seu próprio estado, portanto, devem possuir seu próprio banco de dados. Se um microsserviço requer algum dado de propriedade de outro microsserviço, ele deve requisitar o dado, não acessar diretamente ao banco deste. Cada serviço deve ser pensado como uma funcionalidade de negócios de ponta-a-ponta, que quando apropriado, encapsula sua própria interface com o usuário, lógica de negócio, e dados.

4 - Tamanho do microsserviço:
	Não existe uma regra sobre tamanho, porém, o microsserviço deve ter um tamanho tal que permita que seja facilmente entendido. Quando um microsserviço se torna muito complexo, é sinal que deva ser divido em um ou mais serviços.

5 - Flexibilidade:
	A arquitetura de microsserviços permite que haja mais opções, por exemplo, como os serviços são independentemente desenvolvidos e implantados, é possível desenvolver diferentes microsserviços, utilizando diferentes stacks tecnológicas, como: Python e Flask, NodeJS, ou Go. Um podendo usar um banco de dados NoSQL como o MongoDB, ou um banco relacional como o MySQL.

6 - Alinhamento de arquitetura com organização:
	Organizações que modelam sistemas estão restritas a produzir modelagens que são cópias das estruturas de comunicação dessas organizações. Ou seja, as arquiteturas, em grande parte, tendem a espelhar a estrutura dos times que as desenvolvem.

### O monolito

Vimos um pouco sobre a definição e as características dos microsserviços. Porém, é importante perceber que a arquitetura de microsserviços é frequentemente discutida como **uma alternativa à arquitetura monolítica**. Dessa maneira, é importante entender o que queremos dizer com monolitos quando os comparamos com os microsserviços.

De maneira geral, quando falamos de monolitos neste curso, estamos nos referindo a **uma unidade de implantação** (_deploy_). Quando toda a funcionalidade do sistema deve ser implantada em uma única unidade, consideramos se tratar de um monolito.

Entretanto, múltiplos tipos de sistema se encaixam nessa definição. Em particular, temos frequentemente (1) o monolito de processo único, (2) o monolito modular e (3) o monolito distribuído. Analise com atenção:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/01.png]]

#### Monolito de Processo Único:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/02.png]]

O exemplo mais comum de monolito, é um sistema no qual todo o código é implantado como um único processo. Neste caso, em geral, não há muito cuidado com a modularização dos componentes dentro do monolito, o que significa que o código é altamente acoplado e tem baixa coesão. Quando se trata de um sistema pequeno, não há problemas sérios em se adotar tal tipo de arquitetura. De fato, David Heinemeier Hansson, o criador do Ruby on Rails, argumenta que tal arquitetura faz sentido para organizações menores. No entanto, à medida que a organização cresce, o monolito pode potencialmente crescer com ela, o que nos leva ao monolito modular.

#### Monolito Modular:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 1.png]]

Como um subconjunto do monolito de processo único, o monolito modular é uma variação na qual o processo único é composto de componentes separados e bem modularizados. Cada componente pode ser trabalhado independente, mas todos ainda precisam ser combinados para a implantação, como mostrado na figura. O conceito de dividir o software em componentes não é algo novo; o software modular tem suas raízes em trabalhos realizados em torno da programação estruturada na década de 1970 e até mesmo antes disso. No entanto, ainda não se vê as organizações suficientemente engajadas nessa abordagem de forma adequada.

Para muitas empresas e sistemas, o monolito modular é uma excelente escolha. Se os limites dos componentes são bem definidos, podemos ter alto grau de trabalho em paralelo. No monolito modular também evitamos muitos dos desafios de uma arquitetura de microsserviços mais distribuída ao adotar-se uma topologia de implantação muito mais simples.

#### Monolito Distribuído:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/04.png]]

Um monolito distribuído é um sistema que consiste em vários serviços, mas, por alguma razão, todo o sistema precisa ser implantado conjuntamente. Um monolito distribuído pode se enquadrar na definição de uma arquitetura orientada a serviços (SOA), mas, com muita frequência, não consegue cumprir as promessas da SOA. Assim, um monolito distribuído tem todas as vantagens suficientes de nenhum dos dois. Aqui estamos no pior dos dois mundos: com as desvantagens dos monolitos e as desvantagens dos microsserviços, sem benefício algum.

Os monolitos distribuídos geralmente surgem de um ambiente em que não houve ênfase suficiente em conceitos como ocultação de informação e coesão das funcionalidades do domínio. Em vez disso, arquiteturas altamente acopladas fazem com que mudanças se propaguem através das fronteiras de serviços, e mudanças aparentemente inocentes que parecem locais acabam quebrando outras partes do sistema.

#### Vantagens dos monolitos:

Simplicidade da topologia de implantação, evita muitos problemas comuns em sistemas distribuídos, que por sua vez, simplifica fluxos de trabalho de desenvolvimento, monitoramento, solução de problemas e testes. A reutilização de código em um sistema de monolito é mais simples do que em um sistema distribuído, podendo somente utilizar o código disponível ao invés de copiar código, dividir bibliotecas, ou criar serviços compartilhados. 

### Tecnologias de apoio

No campo de microsserviços existem vários tipos de tecnologia que podem ser utilizados para apoiar o seu uso.

Por sua vez, é preciso tomar cuidado para não adotar uma quantidade excessiva de ferramentas tecnológicas ao se implementar uma arquitetura de microsserviços, o que pode mais atrapalhar do que ajudar. Porém, algumas delas podem ser consideradas essenciais.

Em particular, ferramentas para a captação de _logs_ e rastreamentos distribuídos são muito importantes para coletar e agregar registros de todos os serviços em um único local centralizado para que possam ser analisados e até mesmo se tornar parte de um mecanismo de alerta ativo. Esta é uma atividade crucial, tendo em vista que um dos problemas de se ter vários processos distribuídos rodando em vez de um monolito é a perda da capacidade de monitoração das atividades que são realizadas ao rodar o sistema. Existem várias ferramentas nessa linha, e uma das mais populares é o Humio. Outra opção é usar os próprios serviços simples de registro oferecidos pelos principais provedores de nuvem. Estes podem ser suficientes para começar.

Outra tecnologia muito utilizada para facilitar a execução de instâncias de serviços independentes são os contêineres (o Docker é a ferramenta mais comumente adotada nesse espaço). Eles fornecem uma maneira leve de se provisionar a execução isolada para instâncias de serviço, resultando em tempos de inicialização mais rápidos para novas instâncias de contêiner, além de serem muito mais eficientes em termos de custos para muitas arquiteturas. Depois de começar a trabalhar com contêineres, você perceberá que precisa de algo para gerenciá-los em muitas máquinas.

Plataformas de orquestração de contêineres, como o Kubernetes, permitem distribuir instâncias de forma a fornecer a robustez e a _performance_ de que seu serviço precisa, permitindo também o uso eficiente das máquinas subjacentes.

Mas não se sinta pressionado a adotar o Kubernetes, ou até mesmo contêineres, logo de início. Eles oferecem vantagens significativas em relação às técnicas de implantação mais tradicionais, mas sua adoção é difícil de justificar se você tiver apenas alguns microsserviços. Quando a sobrecarga de gerenciar a implantação começar a se tornar uma dor de cabeça significativa, comece a considerar a conteinerização de seu serviço e o uso do Kubernetes. Mas, se você acabar fazendo isso, faça o melhor para garantir o uso de um serviço que facilite a execução do _cluster_ do Kubernetes para você, talvez usando um serviço gerenciado em um provedor de nuvem pública. Executar seu próprio _cluster_ pode ser uma quantidade excessiva de trabalho.

Com os microsserviços, estamos procurando nos afastar dos bancos de dados monolíticos, mas ainda precisamos encontrar maneiras de compartilhar dados entre os serviços. Produtos que permitem a fácil transmissão e processamento de dados, que muitas vezes podem vir em grandes volumes, tornaram-se populares para quem usa arquiteturas de microsserviços. Para muitos, o Apache Kafka se tornou a escolha padrão para transmitir dados em um ambiente de microsserviços, e por uma boa razão.

Recursos como persistência de mensagens, compactação e a capacidade de dimensionar para lidar com grandes volumes de mensagens podem ser muito úteis.

O Kafka começou a adicionar recursos de processamento de fluxo na forma de KSQLDB, mas você também pode usá-lo com soluções dedicadas de processamento de fluxo, como o Apache Flink. O Debezium é uma ferramenta de código aberto desenvolvida para ajudar a transmitir dados de fontes de dados existentes sobre o Kafka, ajudando a garantir que as fontes de dados tradicionais possam se tornar parte de uma arquitetura baseada em fluxo.

À medida que sua arquitetura de microsserviços cresce, cada vez mais trabalho será empurrado para o espaço operacional.

No entanto, os provedores de nuvem pública, como Google Cloud, Microsoft Azure e Amazon Web Services (AWS), oferecem uma grande variedade de serviços gerenciados e opções de implantação para gerenciar sua aplicação. Isso inclui desde instâncias de banco de dados ou _clusters_ Kubernetes gerenciados até corretores de mensagens ou sistemas de arquivos distribuídos.

Ao usar esses serviços gerenciados, você transfere uma grande parte do trabalho para um terceiro, que é capaz de lidar melhor com essas tarefas. Além disso, os produtos _serverless_ oferecidos pelos provedores de nuvem pública são uma ótima opção, permitindo que você trabalhe em um nível mais alto de abstração. Eles incluem soluções de armazenamento, bancos de dados e plataformas _Function as a Service_ (FaaS), que permitem que você implante seu código e deixe a plataforma subjacente lidar com a criação de instâncias de código sob demanda, sem se preocupar com quantos servidores serão necessários.

### Vantagens e desvantagens da arquitetura de microsserviços

#### Vantages:
![[Pasted image 20240729150548.png]]

1 - Heterogeneidade de tecnologia:
	Podemos decidir usar de diferentes tecnologias dentro de um sistema, permitindo escolhermos a melhor ferramenta para cada trabalho. Por exemplo:
![[Pasted image 20240729151224.png]]
	Outro ponto é a facilitação do upgrade de tecnologias; Por exemplo: Ao invés de fazer o upgrade da versão da JVM de todo um sistema baseado em Java Springboot, podemos escolher alguns microsserviços para realização de upgrade, facilitando gerenciamento de riscos na alteração e possibilitando que essa modificação seja incremental.

2 - Robustez:
	Em uma arquitetura de microsserviço bem implementada, um serviço pode falhar e ainda assim o sistema continua funcionando como um todo.

3 - Escala:
	Com serviços pequenos, é possível escalar somente o que necessita de escala, permitindo outras partes do sistema rodarem em hardware menos poderoso ou com menos instâncias.
![[Pasted image 20240729151908.png]]

4 - Facilidade de implantação:
	Em um microsserviço, é possível alterar somente um microsserviço e implantá-lo independentemente do resto do sistema, e se ocorrer um problema, pode-se isolá-lo, facilitando a recuperação.

5 - Alinhamento organizacional:
	A divisão em microsserviços focados em cada área de negócio ajuda a alinhar melhor a arquitetura com a organização, diminuindo a frequência de problemas como conflitos em várias pessoas trabalhando em um mesmo sistema compartilhado.

6 - Facilidade de composição:
	Oportunidade de re-uso de funcionalidades.

#### Desvantagens:
1 - Quantidade exacerbada de microsserviços:
	Se a quantidade de microsserviços for elevada, pode-se tornar difícil rodar todos os microsserviços do sistema na máquina local do desenvolvedor.

2 - Complexidade de tecnologias:
	Quanto maior o número de microsserviços diversos, maior a quantidade de tecnologias de deverão ser dominadas pelos desenvolvedores.

3 - Custo:
	Por ter muitas partes soltas rodando de forma independente, são requeridos mais recursos como processos, computadores, rede, armazenamento, o que acarreta em maior custo para manter.

4 - Complexidade de acesso aos dados:
	Pela quebra de um banco de dados em vários, o acesso aos dados é dificultado, logo, o monitoramento e a resolução de problemas, assim como a segurança, o teste, a latência e consistência de dados, são aspectos que também são dificultados ao se adotar uma arquitetura de microsserviço.

Embora exista uma tendência, em alguns setores, de fazer dos microsserviços a abordagem padrão para _software_, é importante refletir antes de adotá-los devido aos desafios envolvidos. É fundamental avaliar suas necessidades e habilidades, bem como entender o que deseja alcançar antes de decidir se os microsserviços são adequados para você. É importante lembrar que eles são apenas uma das muitas abordagens arquitetônicas disponíveis e que seu contexto específico deve ser considerado ao decidir seguir por esse caminho.

Dada a importância na definição de limites estáveis entre os microsserviços – falaremos sobre isso logo mais, quando tratarmos de como projetar microsserviços utilizando conceitos do _domain-driven design_ –, em geral pode-se afirmar que uma arquitetura de microsserviços será uma escolha ruim para produtos novos ou _startups_. Talvez o mais apropriado seja esperar até que o modelo de domínio esteja mais estável para que os limites entre os serviços sejam mais bem estabelecidos. É claro que isso vai depender muito do contexto, e podemos considerar também que muitas tecnologias utilizadas em conjunto com microsserviços já estão muito mais maduras do que no início. Além disso, muitos profissionais já adquiriram bastante experiência com esse tipo de arquitetura, o que certamente não era verdade há alguns anos.

Um dos principais motivos pelos quais as organizações adotam a arquitetura de microsserviços é permitir que vários desenvolvedores trabalhem colaborativamente sem interferir nas tarefas uns dos outros (é muito comum a expressão 'pisar nos pés uns dos outros', aludindo ao fato de que uma base de código única, monolítica, começa a produzir atrito entre os diferentes times de desenvolvimento trabalhando nela).

Ao estabelecer limites adequados entre arquitetura e organização, o número de desenvolvedores independentes pode aumentar, reduzindo, assim, os conflitos na entrega. Por sua vez, a arquitetura de microsserviços pode não ser prática para uma _startup_ com uma força de trabalho limitada a cinco pessoas, por exemplo. No entanto, uma empresa mais madura e em crescimento, com cem funcionários, pode descobrir que alinhar seus esforços de desenvolvimento de produtos com uma arquitetura de microsserviços permite gerenciar seu crescimento de maneira mais tranquila.

### Como projetar microsserviços

Microsserviços são essencialmente um tipo de decomposição modular que envolve interação entre modelos baseada em rede, criando desafios adicionais. Assim, felizmente existe uma ampla base de conhecimento existente sobre modularização de _software_ e programação estruturada que podemos aproveitar para nos ajudar a definir os limites entre os microsserviços. Nesse sentido, exploraremos três conceitos cruciais que mencionamos anteriormente. Compreender esses conceitos é vital para determinar o que constitui uma fronteira eficaz de microsserviço.  
  
Os três conceitos são **ocultação de informação**, **coesão** e **acoplamento**.

#### Ocultação de informação

David Parnas introduziu o conceito de ocultação de informações para determinar a abordagem ideal na definição de limites dos módulos/componentes. Basicamente, a ocultação de informações visa a esconder detalhes complexos dentro de um limite de módulo/componente ou microsserviço. Parnas analisou os possíveis benefícios nos módulos quando se faz uso dessa ideia, como a diminuição no tempo de desenvolvimento, a compreensibilidade e a flexibilidade.

Quando apoiamos o desenvolvimento de módulos de maneira independente, permitimos que mais trabalho possa ser feito em paralelo, reduzindo também o impacto de se adicionar mais desenvolvedores a um projeto. A ocultação de informação também permite que os módulos sejam analisados e entendidos em isolamento, o que facilita compreender o que o sistema realiza como um todo. Além disso, os módulos podem ser modificados independentemente uns dos outros, permitindo que a funcionalidade do sistema seja alterada sem a necessidade de mudar outros módulos. Outra vantagem é permitir que os módulos sejam combinados de maneiras diferentes para entregar novos tipos de funcionalidade.

Essas vantagens não aparecem “magicamente” somente pelo fato de dividir um sistema em componentes (ou, em nosso caso, em microsserviços). A maneira como os componentes se comunicam – como os limites entre eles são definidos – também é chave para atingir uma situação na qual esses benefícios aparecem.

De acordo com Parnas:

"**As conexões entre os componentes são as premissas de funcionamento que os componentes assumem uns sobre os outros. Ao reduzir o número de suposições que um módulo (ou microsserviço) faz sobre outro, impactamos diretamente as conexões entre eles. Quando mantemos o número de suposições pequeno, fica mais fácil garantir que podemos modificar um módulo sem afetar outros.**"

#### Coesão

Coesão se refere ao grau no qual os elementos dentro de um componente ou módulo estão inter-relacionados e compartilham um objetivo comum. Seja uma classe, um pacote ou um microsserviço, o princípio permanece o mesmo:

“**Código que muda junto permanece junto.**”

Um módulo com alta coesão é composto por componentes que estão intimamente ligados e servem a um propósito comum. Por exemplo, todos os métodos dentro de uma classe _Usuário_ devem refletir o comportamento do usuário. Por sua vez, um módulo com baixa coesão contém elementos díspares que não estão diretamente relacionados.

Por exemplo, uma classe _Usuário_ que inclui um método para validar endereços de _e-mail_ não é muito coesa. Embora a classe _Usuário_ seja responsável por armazenar o endereço de _e-mail_, não é de sua responsabilidade validar ou enviar _e-mails_.

Nosso objetivo é identificar limites dentro do nosso domínio que promovam funcionalidade consolidada e minimizem a comunicação entre os limites. Quando um comportamento relacionado fica espalhado pelo sistema, isso indica coesão fraca. Em arquiteturas de microsserviços, nosso objetivo é alcançar alta coesão.

#### Acoplamento

O baixo acoplamento entre serviços é crucial em uma arquitetura de microsserviços. Ele garante que uma alteração em um serviço não exija alterações em outros, permitindo a implantação independente. O acoplamento forte, por sua vez, resulta de estilos de integração que unem os serviços, exigindo que modificações em um serviço sejam refletidas em seus consumidores.

Para manter o baixo acoplamento, um serviço deve ter conhecimento apenas do mínimo necessário para colaborar com outros serviços. Isso também significa reduzir o número de diferentes tipos de chamadas entre os serviços. Além de possíveis problemas de desempenho, muita comunicação também pode levar a alto acoplamento.

O acoplamento, no entanto, assume várias formas, e equívocos sobre sua natureza em arquiteturas baseadas em serviços são comuns. Em particular, no contexto de microsserviços, podemos ter quatro tipos de acoplamento: acoplamento de domínio, acoplamento de passagem, acoplamento comum e acoplamento de conteúdo. Esses tipos de acoplamento estão listados em ordem de mais fraco para mais forte. Isso quer dizer que o acoplamento de domínio é o mais fraco, enquanto o acoplamento de conteúdo é o mais forte.

O **acoplamento de domínio** descreve uma situação em que um microsserviço precisa interagir com outro microsserviço, porque o primeiro microsserviço precisa usar a funcionalidade que o outro fornece. Por exemplo, conforme ilustrado na figura a seguir, em determinado sistema podemos ter três microsserviços: um que processa pedidos (processador de pedidos), um que gerencia o armazenamento de produtos (armazém) e um que gerencia o pagamento (pagamento). O microsserviço processador de pedidos precisa chamar o microsserviço de armazém para reservar estoque. Ele também interage com o microsserviço de pagamento para que seja recebido um pagamento. O microsserviço de processamento de pedidos é, portanto, dependente e acoplado aos microsserviços de armazém e pagamento. Esse acoplamento não aparece em relação aos microsserviços de armazém e pagamento, já que eles não interagem. Em uma arquitetura de microsserviços, esse tipo de acoplamento é praticamente impossível de se evitar completamente.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 1 1.png]]

**Acoplamento de passagem** descreve uma situação na qual um microsserviço passa dados a outro microsserviço somente porque esses dados serão requeridos por outro microsserviço que será chamado mais para frente na cadeia de interação entre os microsserviços. Por exemplo, conforme ilustrado na figura a seguir, imagine que o nosso microsserviço de processamento de pedidos faz uma requisição ao armazém para que seja preparado um pedido para envio. Porém, em vez de enviar somente as informações de que ele precisa para informar ao armazém sobre o pedido a ser preparado, ele também inclui na requisição um **manifesto de carga** com as informações de frete que serão utilizadas pelo microsserviço de frete no envio do produto. Repare que o armazém não utiliza essa informação diretamente; ele somente a **repassa** ao microsserviço de frete.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 2.png]]

No **acoplamento comum**, dois microsserviços compartilham um conjunto de dados. Esse tipo de acoplamento acontece, por exemplo, quando dois microsserviços utilizam o mesmo banco de dados (ou o mesmo sistema de arquivos, ou memória compartilhada). O principal problema desse tipo de acoplamento é que, quando a estrutura dos dados compartilhados muda, isso afeta mais de um microsserviço de uma vez só. Um exemplo, ilustrado na figura a seguir, poderia ser quando mais de um microsserviço – como o processador de pedidos e o armazém – utiliza um mesmo banco com dados estáticos com informações sobre países. Esse exemplo pode ser considerado um acoplamento até benigno, porque dados estáticos não tendem a mudar muito. No entanto, o acoplamento comum pode se tornar um problema mais grave quando os dados mudam mais frequentemente ou mais de um microsserviço lê e escreve dados em uma mesma base de dados.

![[Pasted image 20240729185705.png]]

O **acoplamento de conteúdo** acontece quando um serviço chamador acessa dados internos de um microsserviço chamado e muda o seu estado interno. Por exemplo, como ilustrado na figura a seguir, imagine um sistema que inclui um serviço de pedido que é responsável por gerenciar as mudanças de estado permitidas para os pedidos. O processador de pedidos envia solicitações ao serviço de pedido, delegando não apenas as alterações de estado exatas que serão feitas, mas também a responsabilidade por decidir quais transições de estado são permitidas. No entanto, suponha que o serviço de armazém **atualiza diretamente** a tabela de armazenamento de dados do pedido, ignorando qualquer funcionalidade no serviço de pedido que possa verificar mudanças permitidas. Temos que confiar no serviço de armazém para ter um conjunto consistente de regras para garantir que apenas alterações válidas sejam realizadas. Isso representa uma possível duplicação de lógica na melhor das hipóteses. Na pior das hipóteses, o processo de validação do serviço de armazém para mudanças permitidas pode ser diferente do serviço de pedido, **levando a pedidos em estados inconsistentes e incomuns**.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 3.png]]

Ao permitir que uma parte externa acesse diretamente seu banco de dados, o banco de dados se torna efetivamente parte desse contrato externo, embora seja difícil definir facilmente o que pode ou não ser alterado. Você perde a capacidade de definir o que é compartilhado (e, portanto, não pode ser facilmente alterado) e o que está oculto. A ocultação de informações é comprometida. Em suma, evite o acoplamento de conteúdo.

#### _Domain-driven design_ no projeto de microsserviços

Como comentado anteriormente, um microsserviço é um serviço projetado sobre um domínio de negócios. Dessa forma, uma ótima ferramenta que pode ser usada para o projeto de microsserviços é o **_domain-driven design_** (DDD). O DDD foi introduzido por Eric Evans e apresenta um conjunto de ideias importantes que nos ajudam a melhor representar o domínio do problema dentro dos nossos programas. Em particular, os conceitos de **linguagem ubíqua, agregados** e **contextos delimitados** podem ajudar muito no projeto de uma arquitetura de microsserviços.

A **linguagem ubíqua** é a prática de usar a mesma terminologia utilizada pelos usuários do sistema em nosso código. O objetivo é estabelecer uma linguagem comum entre a equipe de desenvolvimento e os usuários finais – na verdade, entre todos os interessados do sistema –, o que pode facilitar a comunicação e a modelagem de um domínio do mundo real. Como um exemplo do que não fazer, Sam Newman descreve uma situação quando trabalhava para um grande banco global na área de liquidez corporativa. Confira:

A proprietária do produto era experiente e falava em termos que faziam sentido para seus clientes, como _haircuts e end-of-day sweeps_. No entanto, a base de código não usava essa linguagem porque havia sido tomada a decisão de usar um modelo de dados padrão, referido como 'o modelo bancário da IBM'. Esse modelo usava o conceito de um 'arranjo' para representar qualquer operação bancária, desde a realização de um empréstimo até a compra de uma ação ou a solicitação de um cartão de crédito. Infelizmente, essa padronização poluiu muito a base de código, porque ela não compreendia os conceitos reais do sistema que estava sendo construído. Em vez de construir um sistema especificamente para gerenciar a liquidez corporativa, estávamos criando um aplicativo bancário genérico que não capturava a terminologia e as nuances específicas necessárias para o propósito pretendido. Como resultado, os analistas de negócio precisavam explicar um mesmo conceito diversas vezes, porque não havia uma terminologia comum utilizada entre os clientes e a equipe de desenvolvimento. Como no _software_ tudo foi implementado utilizando o conceito de 'arranjo', era difícil encaixar as operações do domínio de liquidez corporativa no sistema. Dessa forma, é muito desejável que seja estabelecida uma **linguagem ubíqua** no projeto de uma arquitetura de microsserviços (na verdade, isso é desejável para qualquer arquitetura), porque isso facilita a comunicação entre todos os envolvidos no uso e desenvolvimento do _software_.

Em DDD, um **agregado** é um conceito importante, porém um tanto confuso, com muitas definições diferentes por aí. Será apenas uma coleção arbitrária de objetos? A menor unidade que deve ser recuperada de um banco de dados? Parece-me que uma boa maneira de entender essa ideia é primeiro considerar um agregado como uma representação de um **conceito real de domínio** – pense em algo como um **pedido**, uma **fatura**, um **aluguel**, um **item de estoque**, e assim por diante. Os agregados geralmente têm um **ciclo de vida**, o que faz com que possam ser implementados como uma máquina de estado. Por exemplo, um agregado de **Pedido** pode conter vários itens (imagine um pedido em uma loja de móveis que inclui **três sofás e uma cadeira** – cada par quantidade x produto é um **item do pedido**). Veja: esses **itens** só têm sentido quando considerados como parte do agregado geral do **Pedido** e, portanto, não poderiam ser considerados como um agregado em si, mas fariam parte do agregado **Pedido**.

Em geral, queremos tratar os agregados como unidades independentes, deixando o código que lida com as suas transições de estado – no caso do pedido, por exemplo, de **pedido realizado a pedido enviado** – ser implementado junto com o próprio estado. Portanto, um agregado deve ser gerenciado por um microsserviço, embora um único microsserviço possa gerenciar vários agregados. Em geral, porém, você deve pensar em um agregado como algo que tem estado, identidade e um ciclo de vida que será gerenciado como parte do sistema. Agregados geralmente se referem a conceitos do mundo real.

Um único microsserviço lidará com o ciclo de vida e o armazenamento de dados de um ou mais agregados. Se a funcionalidade em outro serviço quiser alterar um desses agregados, ele precisará solicitar diretamente uma alteração ou fazer com que o próprio agregado reaja a outros eventos no sistema para iniciar suas próprias transições de estado, talvez registrando-se como interessado em eventos emitidos por outros microsserviços. O principal a entender aqui é que, se uma parte externa solicitar uma transição de estado em um agregado, o agregado poderá negar-se a mudar de estado. Idealmente, devemos implementar os agregados de forma que as transições de estado ilegais sejam impossíveis.

Em DDD, outro conceito importante refere-se aos **contextos delimitados**. Um contexto delimitado geralmente representa um limite organizacional de mais alto nível, envolvendo possivelmente múltiplos agregados. Dentro do escopo desse limite, responsabilidades explícitas precisam ser realizadas. Imagine uma empresa na qual o depósito – ou armazém – é um ramo de atividades.

O depósito compõe atividades como gerenciar pedidos despachados (e retornos ocasionais), receber novos estoques, participar de corridas de empilhadeiras, e assim por diante. Em outra parte da empresa, o departamento financeiro talvez seja menos divertido, mas ainda tem uma função importante dentro da organização e abarca atividades como lidar com a folha de pagamento, o pagamento de remessas, e assim por diante. O sistema de _software_ que implementa o domínio dessa empresa poderia conter dois contextos delimitados: um que se refere ao **depósito** e outro que se refere ao **financeiro**.

Uma característica importante dos contextos delimitados é que eles ocultam detalhes de implementação do mundo exterior. Preocupações internas como os tipos de empilhadeiras utilizadas são de pouco interesse para qualquer pessoa que não seja o pessoal do depósito. Essas preocupações internas devem ser escondidas do mundo exterior, que não precisa saber e nem deveria se preocupar com elas.

Do ponto de vista de implementação, os contextos limitados contêm um ou mais agregados (no exemplo, o **Depósito** e o **Financeiro** poderiam conter múltiplos agregados). Alguns agregados podem ser expostos para fora do contexto delimitado; outros podem estar escondidos internamente. Assim como os agregados, os contextos delimitados podem ter relacionamentos com outros contextos delimitados – quando mapeados para serviços, essas dependências se tornam dependências entre serviços.

Tanto um **agregado** quanto um **contexto delimitado** oferecem unidades de coesão com interfaces bem definidas com o sistema mais amplo. O agregado é uma máquina de estado independente que se concentra em um único conceito de domínio em nosso sistema, e o contexto delimitado representa uma coleção de agregados associados, novamente com uma interface explícita para o mundo mais amplo.  
  

Ambos podem, portanto, funcionar bem como limites de serviço, ou seja, **um microsserviço poderia implementar tanto um contexto delimitado de um domínio quanto apenas um agregado.**

No começo de um projeto, como já comentado, é melhor **reduzir o número de serviços implementados**. Como resultado, você provavelmente deve implementar serviços que abranjam contextos delimitados inteiros. No entanto, à medida que você se adapta e decide dividir esses serviços em serviços menores, é preciso lembrar que os agregados não devem ser quebrados: mais uma vez, um microsserviço pode gerenciar um ou mais agregados, mas não queremos que um agregado seja gerenciado por mais de um microsserviço. A quebra de um agregado certamente afetaria a coesão de um serviço e introduziria dependências indesejadas entre os serviços.

### Conclusão

Finalmente chegamos ao fim desta primeira aula. Achei por bem expandir essas ideias iniciais, pois, com elas bem formadas em nossa cabeça, o restante acontece de modo muito mais natural.

Resumindo algumas das principais ideias desta aula:  
  

- Um microsserviço é um serviço modelado em torno de um domínio de negócios que pode ser lançado e implantado ​​independentemente.

- Talvez uma das ideias mais importantes de uma arquitetura de microsserviços é a de que deve ser possível implantar cada microsserviço de maneira independente.

- Você só deve adotar uma arquitetura de microsserviços se tiver boas razões para isso. Em minha opinião (e na do Sam Newman e de outros autores também), a escolha padrão de arquitetura deveria ser a de um monolito modular.

- Como a arquitetura de microsserviços compõe componentes modulares, todas as ideias desenvolvidas no campo de projeto de _software_ também deveriam ser aplicadas aqui. Em particular, os conceitos de **ocultamento de informação, coesão e acoplamento** são muito importantes ao modelar seus microsserviços.

- O _domain-driven design_ é uma ótima ferramenta para se modelar microsserviços. Em particular, devemos tomar cuidado para adotar uma linguagem ubíqua quando modelarmos uma arquitetura de microsserviços. Além disso, é importante que cada microsserviço implemente um contexto delimitado ou um agregado. Quebrar agregados em múltiplos microsserviços é uma má ideia, pois diminui a coesão do sistema e introduz acoplamentos indesejados.

### Referências:

EVANS, E. **Domain-driven design**: tackling complexity in the heart of software. [_s.l._]: Addison-Wesley Professional, 2003.

FOWLER, M. Who needs an architect? **IEEE Software**, v. 20, n. 5, p. 11–13, 2003.

HANSSON, D. The magestic monolith. **Signal V Noise**, 1999-2023. Disponível em: [https://m.signalvnoise.com/the-majestic-monolith/](https://m.signalvnoise.com/the-majestic-monolith/). Acesso em: 25 maio 2023.

LEMOS, O. **Arquitetura limpa na prática**. [_s.l.: s.n._], 2021.

LEWIS, J.; FOWLER, M. Microservices: a definition of this new architectural term. **Martin Fowler**, 2014. Disponível em: [https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html). Acesso em: 25 maio 2023.

MARTIN, R.; FEATHERS, M.; OTTINGER, T. **Clean code**: a handbook of agile software craftsmanship. [_s.l._]: Prentice Hall, 2008.

MICROSSERVIÇOS: o mínimo que você precisa saber. [_S. l.: s. n._], 2020. 1 vídeo (13 min). Publicado pelo canal Otavio Lemos. Disponível em: [https://www.youtube.com/watch?v=eN8dFfTrEtQ&t=201s](https://www.youtube.com/watch?v=eN8dFfTrEtQ&t=201s). Acesso em: 25 maio 2023.

NEWMAN, S. **Building microservices**: designing fine-grained systems. 2. ed. [_s.l._]: O'Reilly, 2021.

PARNAS, D. L. On the criteria to be used in decomposing systems into modules. **Communications of the ACM**, v. 15, n. 12, p. 1053-1058, 1972.
## Implementando Uma Arquitetura de Microsserviços (Aula 2)

### Comunicação entre microsserviços

Acertar a comunicação entre microsserviços é difícil para muitas pessoas. Isso se dá devido, em grande parte, ao fato de que elas gravitam em direção a uma **abordagem tecnológica escolhida a** **_priori_**, sem primeiro considerar os diferentes tipos de comunicação que podem fazer sentido em cada lugar da aplicação. De modo geral, existem mecanismos de comunicação **síncronos bloqueantes** e **assíncronos não bloqueantes**. Existem, também, de maneira geral, três estilos diferentes de colaboração _request-response_ (requisição-resposta), dirigidos a eventos e com uso de dados compartilhados. O diagrama da figura a seguir mostra esses diferentes tipos de colaboração com escolhas comuns de implementação:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/01 1.png]]

Síncrono Bloqueante:
	Um microsserviço faz uma chamada para outro microsserviço e bloqueia a operação, aguardando resposta.

Assíncrono Não-Bloqueante:
	O microsserviço que emite uma chamada é capaz de continuar o processamento, independentemente de a chama ser recebida ou não.

Request-Response:
	Um microsserviço envia uma requisição para outro microsserviço, solicitando que algo seja feito. ele espera receber uma resposta informando o resultado (note que esse tipo de comunicação pode ser feito tanto síncrona quanto assincronamente).

Dirigido à Eventos:
	Os microsserviços emitem eventos que correspondem a fatos que ocorrem no sistema. Esses eventos são consumidos por outros microsserviços, que reagem de acordo com algum tratamento implementado (por exemplo, quando um pedido é realizado no microsserviço de "Pedidos" o microsserviço de "Produtos" precisa atualizar o estoque). O microsserviço que emite o evento não tem conhecimento de quais microsserviços consomem os eventos que ele emite (no exemplo, o microsserviço de "Pedidos" apenas emite o evento "_pedido realizado_").

Dados Compartilhados:
	Frequentemente, não é considerado um estilo de comunicação, mas os microsserviços colaboram por meio de uma fonte de dados compartilhada.

Como é possível observar no diagrama, podemos ter um estilo de colaboração _request-response_ síncrono bloqueante, ou seja, em que o microsserviço faz a requisição e bloqueia a operação, aguardando a resposta; ou assíncrono não bloqueante, ou seja, em que o microsserviço faz a requisição e não bloqueia a operação, recebendo a resposta em algum tempo no futuro (pode ser que outra parte da aplicação lide com a resposta).



**Estilos de colaboração em microsserviços e sistemas distribuídos**

Como material complementar, você pode assistir ao vídeo do meu canal do YouTube, em que falo sobre o assunto.

[Clique aqui](https://youtu.be/cFft8IJ3M9Y) para acessar o vídeo.


Em geral, o estilo de comunicação _request-response_ é implementado utilizando o padrão arquitetural REST (Representational State Transfer) com o protocolo HTTP (Hypertext Transfer Protocol). Porém, como alternativa, mais recentemente surgiu o GraphQL, uma linguagem de consulta criada pelo Facebook em 2012 e lançada publicamente em 2015. A principal diferença entre o GraphQL e o REST é que o primeiro permite incluir consultas na requisição, o que pode facilitar o acesso a subconjuntos de dados na comunicação. Os dados retornados com REST são sempre predefinidos, ou seja, se for necessário construir uma requisição que acessa um subconjunto – ou superconjunto – de dados, é necessário criar outro _endpoint_ específico para essa comunicação. Além disso, como o GraphQL permite que o cliente defina consultas nos dados, isso também pode evitar a realização de múltiplas requisições para recuperar a mesma informação. Além disso, pode impactar a performance, favorecendo uma otimização de requisições, o que é muito interessante para clientes mais restritos, como _apps_ rodando em um celular. Mesmo assim, o padrão REST sobre HTTP continua sendo a implementação mais popular do estilo _request-response_.  
  
  
Uma das vantagens do REST, comparado ao GraphQL, é sua simplicidade.

  
RPC (Remote Procedure Call, ou Chamada Remota a Procedimento) refere-se à técnica de realizar uma chamada local e fazer com que ela seja executada em algum serviço remoto. Ou seja, para o programador, ele aparentemente só está realizando uma chamada a uma função local – no código, é como uma chamada local mesmo, mas essa chamada acionará uma requisição a um serviço remoto.  
  

Existem diferentes tipos de implementação de RPC e a maioria exige um esquema explícito de dados, como SOAP (Simple Object Access Protocol, ou Protocolo Simples de Acesso a Objetos) ou gRPC (Google Remote Procedure Call). No exemplo de código mais complexo que veremos mais à frente, nesta aula, RPCs são usadas para a comunicação entre serviços.

#### _Brokers_ de mensagem

Um mecanismo amplamente utilizado na comunicação assíncrona entre microsserviços são os _brokers_ de mensagem. Os _brokers_ de mensagem são intermediários, também conhecidos como _middleware_, que atuam como facilitadores na comunicação entre processos.

Em uma arquitetura de microsserviços, uma mensagem é um conceito genérico que representa o conteúdo transmitido por um _broker_ de mensagem. Essa mensagem pode conter uma solicitação – uma _request_ –, uma resposta – uma _response_ – ou um evento. Em vez de ocorrer uma comunicação direta entre os microsserviços, o serviço envia a mensagem para o _broker_ de mensagem, incluindo informações sobre como a mensagem deve ser entregue.

Os _brokers_ de mensagem podem ser baseados em **filas** ou **tópicos**. As filas são comumente utilizadas para comunicação ponto a ponto, em que um produtor **coloca** uma mensagem em uma fila específica e um consumidor **lê** a mensagem dessa fila. Já os tópicos permitem que vários consumidores se inscrevam em um tópico, recebendo, assim, cópias das mensagens relacionadas a ele.

Uma das principais diferenças entre um _broker_ baseado em fila e um baseado em tópico é que, quando uma mensagem é enviada utilizando uma fila, existe conhecimento de **para quem** ela está sendo enviada. No caso do tópico, essa informação é escondida do produtor: ele não sabe quem – e se, de fato, alguém – receberá a mensagem.

### Fluxo de trabalhos

Até agora, em nossa exploração, focamos principalmente a comunicação entre pares de microsserviços. No entanto, quando se trata de permitir que vários microsserviços trabalhem juntos, como na implementação de um processo de negócios, a tarefa de modelar e implementar esses fluxos de trabalho colaborativos em sistemas distribuídos pode ser desafiante.

Na computação, uma _**transação**_ se refere a um conjunto de ações tratadas como uma única unidade. Ao fazer várias alterações dentro de uma operação, é importante verificar sua conclusão e lidar com possíveis erros.

Isso geralmente envolve o uso de uma transação de banco de dados, em que são realizadas modificações de estado, como remoção, inserção ou alteração de dados. Em bancos de dados relacionais, essas transações podem abranger várias tabelas.

A questão é que, muitas vezes, uma operação envolve mais de uma alteração e essas alterações devem ser realizadas em conjunto. Por exemplo: no contexto da transferência de dinheiro entre contas bancárias, uma transação de banco de dados garante a integridade da operação.

Sem uma transação, pode ocorrer um problema em que o dinheiro é debitado de uma conta, mas não creditado em outra, levando a um estado inconsistente. Ao utilizar uma transação, tanto as operações de débito quanto as de crédito ocorrem de forma atômica, garantindo que ambas as alterações sejam feitas com sucesso, ou nenhuma, evitando tais inconsistências. 

Outro exemplo, no mesmo domínio em que é necessário utilizar uma transação e um esquema de locks, é quando pode haver saques de uma mesma conta em diferentes locais (por exemplo: em um conta conjunta, uma pessoa faz um saque em um caixa eletrônico enquanto outra faz em outro, ao mesmo tempo).

Imagine que o saque é feito seguindo o algoritmo do seguinte fluxograma:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/04 1.png]]

Sem uma transação, as retiradas simultâneas podem substituir as alterações umas das outras, levando a débitos incorretos. Por exemplo, se as duas requisições de saques são praticamente simultâneas e ocorrem segundo a seguinte figura, os dois saques de $100 são realizados sem problemas, mesmo havendo um saldo de apenas $100 antes das requisições (isso porque a atualização do saldo só ocorre depois do passo “Altera o saldo”, ou seja, quando se verifica o saldo; como a alteração ainda não foi feita, o saldo aparece como suficiente).

Ao utilizar uma transação, os saques são realizados de forma atômica, garantindo a consistência dos dados e evitando a perda de atualizações, conforme apresentado na figura a seguir:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/04 2.png]]

As transações de banco de dados geralmente se referem a transações ACID (atomicidade, consistência, isolamento e durabilidade). Essas propriedades garantem a confiabilidade e a integridade do sistema de armazenamento de dados. Aqui está um detalhamento do que cada propriedade implica:

**Atomicidade**: Garante que todas as operações dentro de uma transação sejam concluídas com sucesso ou nenhuma delas entre em vigor. Se alguma alteração falhar, toda a transação será revertida, deixando o banco de dados inalterado.

**Consistência**: Garante que o banco de dados permaneça em um estado válido e consistente após a execução de uma transação, obedecendo a regras e restrições predefinidas. 

**Isolamento**: Permite que várias transações operem simultaneamente sem haver interferência entre elas. Alterações temporárias feitas em uma transação são isoladas de outras transações até que as alterações sejam confirmadas.

**Durabilidade**: Garante que, uma vez que uma transação seja confirmada e concluída, suas alterações sejam permanentemente armazenadas e protegidas contra falhas ou travamentos do sistema.


Um microsserviço pode realizar transações ACID em seu próprio banco de dados local. Entretanto, algumas operações podem envolver alterações em bancos de um conjunto de microsserviços. É aí que entra a dificuldade em manter a consistência dos dados, uma vez que temos um conjunto de bancos de dados envolvidos na operação, e não somente um microsserviço realizando alterações locais em seu próprio conjunto de dados.

Uma das maneiras de contornar esse problema é utilizar **transações distribuídas** que usam algoritmos como o de _commit_ de duas fases (2_PC – two-phase-commit_). Não vou entrar em detalhes de como se poderia implementar uma transação distribuída porque, em geral, para o contexto de microsserviços, isso é uma má idéia. Porém, explicando rapidamente, ela envolve uma fase de preparação em que o coordenador verifica se cada microsserviço participante pode realizar a sua parte da operação, seguida por uma fase de _commit_ em que a transação é finalizada. Se todos os microsserviços estiverem preparados para o _commit_, a transação prosseguirá, mas, se algum microsserviço encontrar um problema, a transação será abortada.

O uso de _commits_ de duas fases e transações distribuídas no contexto de microsserviços apresenta os seguintes desafios: maior complexidade, impacto no desempenho, limitações de escalabilidade, acoplamento entre serviços, ponto único de falha, riscos de impasse distribuído – _deadlocks_ – e problemas de consistência.

Esses fatores podem prejudicar a escalabilidade, a capacidade de resposta e a resiliência do sistema. Consequentemente, muitas organizações exploram abordagens alternativas, como transações de compensação, arquiteturas orientadas a eventos ou eventuais padrões de consistência para enfrentar esses desafios e fornecer soluções mais flexíveis e escaláveis ​​para microsserviços.

Uma das soluções mais populares e recomendadas por especialistas, como Sam Newman, é o padrão SAGA. Ele visa lidar com transações complexas e de longa duração, dividindo-as em uma série de etapas ou estágios menores e fracamente acoplados, conhecidos como “sagas”.

No padrão SAGA, cada microsserviço envolvido na transação é responsável por suas operações transacionais locais e mantém seu próprio banco de dados. Em vez de uma única transação atômica abrangendo vários serviços, uma saga coordena uma sequência de transações locais, cada uma dentro de seu próprio limite de microsserviço.

Entenda como o padrão SAGA normalmente funciona no infográfico a seguir:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb7.png]]

A seguir, temos um exemplo de implementação do padrão SAGA. Nesse contexto, a **realização dos pedidos** é ilustrada como uma saga única, em que cada fase do processo corresponde a uma ação executada por um serviço distinto. Dentro de cada serviço, todas as alterações de estado podem ser gerenciadas em transações ACID locais. Por exemplo: ao verificar e reservar estoque por meio do serviço Armazém, internamente esse serviço pode criar uma entrada em sua tabela local de Reservas para registrar a reserva. Essa modificação seria processada em uma transação de banco de dados convencional. A figura mostra, ainda, a situação em que a última operação da saga no serviço Armazém falha, por conta da falta de estoque para a realização do pedido. Repare que, nesse ponto, é necessário realizar transações compensatórias em outros serviços para reverter toda a operação: debitar os pontos do sistema de Fidelidade, devolver o dinheiro do cliente no serviço de Pagamentos e remover a reserva de estoque do Armazém. Isso é comparável a um _rollback_ realizado em um banco de dados, mas, nesse caso, exige alterações nos vários serviços participantes (isso é chamado de **_rollback_** **de saga**).

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb8.png]]

### _Build_, implantação e teste de sistemas baseados em microsserviços

Em nossas discussões anteriores, focamos aspectos de _design_ de microsserviços. Agora, vamos nos aprofundar nas mudanças necessárias no **processo de desenvolvimento** para adequação a esse estilo arquitetônico. Antes de examinar a implantação e o teste de microsserviços nas seções a seguir, primeiro precisamos entender o que acontece quando um desenvolvedor está pronto para dar _commit_ de suas alterações em um dado microsserviço.

#### Integração contínua

A integração contínua (CI – _continuous integration_) é uma prática bem estabelecida que garante a frequente integração e sincronização de código entre desenvolvedores. A integração contínua consiste em realizar frequentemente o _merge_ das alterações de código em um repositório compartilhado, e validá-las automaticamente por meio de compilações e testes automatizados.

Ela envolve um servidor CI que detecta _commits_ de código, realiza verificações como compilação e testes, e cria artefatos para validação posterior. Esses artefatos são armazenados em um repositório para permitir a reutilização e confirmar se os artefatos implantados correspondem aos testados.

A CI oferece vários benefícios, incluindo _feedback_ rápido sobre a qualidade do código, criação automatizada de artefatos, rastreabilidade entre artefatos e código e capacidade de controlar a versão da configuração da infraestrutura juntamente com o código do microsserviço.  
  
O sucesso da CI é atribuído a sua capacidade de fornecer transparência, reprodutibilidade e colaboração eficiente no desenvolvimento de _software_.
  
O debate sobre esquemas de _branching_ de código-fonte para o desenvolvimento de _software_ é controverso. _Branching_ é o mecanismo utilizado quando se deseja ramificar do tronco principal de código no desenvolvimento de um projeto, para se implementar, por exemplo, um novo comportamento no sistema. Ele é realizado utilizando principalmente a ferramenta _git_ de versionamento de código (o comando geralmente utilizado para isso é o _gitbranch_). Embora esse tipo de ramificação permita o desenvolvimento isolado de alguma parte do sistema, atrasa a integração e resulta em _merges_ complexos. Não é difícil visualizar que a utilização de _branches_ que demoram a ser incorporadas ao tronco principal pode atrapalhar a integração contínua. Dessa forma, uma abordagem alternativa à criação de _branches_ e sua posterior incorporação ao tronco é o _trunk-based development_ (TBD). No TBD, todos trabalham e _commitam_ código direto no mesmo tronco, sem a criação de _branches_, utilizando, por exemplo, _feature flags_ para ocultar trabalhos incompletos.

As vantagens da integração e validação frequentes superam as desvantagens, tornando o _trunk-based development_ um esquema de _branching_ muito desejável. Além disso, a implementação de _feature flags_ pode, também, ser vantajosa para a entrega progressiva de _software_. Ainda que não se use o _trunk-based development_, acredito – e estudos têm demonstrado isso cada vez mais definitivamente, em particular os do projeto DORA, delineados no livro _Accelerate_ – que, quanto antes e mais frequentemente se faz o _merge_ de alguma _branch_, melhor para o andamento do projeto (ou seja, se de fato for necessário abrir _branches_, o ideal é que elas tenham vida curta; por exemplo, no máximo, um dia).

Uma outra opção menos **radical** de esquema de _branching_ é o _Ship_ – _Show_ – _Ask_, descrito por Rouan Wilsenach (2021). Nesse esquema, para cada alteração nova implementada, pode-se escolher se quer fazer o _merge_ diretamente (_ship_), fazer o _merge_ e mostrar a alteração pós-merge (_show_), ou pedir para que o código seja revisado _antes_ do _merge_ (_ask_). Muitos esquemas utilizados – como o GitFlow – somente utilizam a terceira opção, exigindo que se crie uma _branch_, que é submetida para revisão de código antes de todo e qualquer _merge_ (por meio de, principalmente, _pull requests_, as famosas PRs).


#### _Pipelines_ de _build_

As _pipelines_ de _build_ envolvem a divisão do processo de _build_ em vários estágios para melhorar a eficiência e fornecer valioso _feedback_ no processo.

Essa abordagem é particularmente útil ao lidar com diferentes tipos de testes, como testes rápidos e de escopo pequeno _versus_ testes lentos e de escopo grande (por exemplo, testes de integração que envolvam banco de dados).

Ao separar os testes em estágios distintos em uma _pipeline_ de _build_, torna-se possível priorizar testes rápidos para um _feedback_ mais rápido. Se os testes rápidos falharem, não há necessidade de prosseguir com os testes mais lentos.

O conceito de _pipeline_ de _build_ permite monitorar o progresso da alteração de _software_ à medida que ela passa por cada estágio, fornecendo informações sobre sua qualidade. Ao longo da _pipeline_, um artefato implantável é usado, representando o _software_ alterado a ser implantado. Esse artefato, no contexto de um microsserviço, passa por cada estágio, incutindo cada vez mais confiança de que funcionará corretamente em produção.

Na figura a seguir, é exemplificada uma _pipeline_ de _build_ em que um microsserviço de nossa aplicação é compilado e verificado com testes rápidos e o artefato gerado a partir da compilação passa pelos próximos estágios da _pipeline_, com verificações cada vez mais rigorosas, até que ele seja implantado em produção. Se alguma das verificações falha, o microsserviço alterado não é implantado em produção. Ferramentas como o GitHub Actions podem ser utilizadas para automatizar a _pipeline_ de _build_.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb9.png]]

#### Entrega contínua e implantação contínua

Dado que temos uma _pipeline_ de _build_ que roda cada vez que integramos alguma implementação nova de nosso microsserviço, se nesse processo há **implantação automática das alterações em produção**, então estamos realizando o que é chamado de implantação contínua (_continuous deploy_). Se, por outro lado, não fazemos a implantação automática, mas a cada alteração deixamos o nosso microsserviço em um estado que nos permita fazer a implantação quando quisermos, então estamos falando de entrega contínua (_continuous delivery_). Com a junção das integrações frequentes – a integração contínua – com a prática de sempre deixarmos nosso sistema pronto para a implementação – a _continuous delivery_ –, temos o que é comumente conhecido, em nossa indústria, como CI/CD.  


É importante que fique claro que não é possível realizar CI/CD sem uma boa base de testes automatizados, pois é essa base que vai garantir a possibilidade de se integrar e implantar frequentemente com confiança.


#### Implantação de microsserviços

A implantação de um sistema monolítico é relativamente simples, já que, simplificadamente, estamos falando de apenas **um processo rodando em algum servidor**.

Em primeiro lugar, deve ficar claro que a maneira como modelamos nossos microsserviços até agora mostra somente uma visão **lógica** de como esses serviços são divididos e se comunicam entre si. Entretanto, quando de fato falamos na implantação dos microsserviços, estamos falando de uma visão **física** e que, de maneira geral, diverge bastante da visão lógica mais simples.

Por exemplo, ao considerar a topologia de implantação dos dois microsserviços representados na figura a seguir, percebemos que não se trata simplesmente de um serviço se comunicando com outro. Inicialmente, é muito provável que várias instâncias de cada serviço sejam implantadas. Ter várias instâncias de serviço permite um melhor manuseio de carga e aumenta a resiliência do sistema, fornecendo a capacidade de se manter tolerante à falha de uma única instância.

Assim, poderíamos ter uma ou mais instâncias do serviço Fatura se comunicando com uma ou mais instâncias do serviço Pedido. As especificidades de como a comunicação entre essas instâncias é gerenciada dependem do mecanismo de comunicação escolhido. Supondo o uso de uma API baseada em HTTP nesse cenário, um balanceador de carga seria suficiente para rotear solicitações para diferentes instâncias de serviço, conforme ilustrado na mesma figura.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 4.png]]

E o banco de dados, como fica? Como deixamos claro na primeira aula, é importante que cada microsserviço gerencie seu próprio estado em uma base de dados própria. Mas isso não significa que haverá um banco para cada **instância** de microsserviço. De maneira geral, por exemplo, para recuperar informações sobre um determinado pedido, independentemente da instância do serviço de Pedido que é acessado, é necessário haver um certo nível de estado compartilhado entre diferentes instâncias do mesmo serviço lógico. Fluxo disponível na figura abaixo:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/03 5.png]]

Existem muitas outras questões relacionadas com a implantação de microsserviços, porém cairiam fora do escopo de nossa aula. Entretanto, julgo importante o seguinte conjunto de princípios essenciais ao se considerar a implantação de uma arquitetura de microsserviços:

![[Pasted image 20240731111812.png]]

**Execução Isolada**:
	Execute as instâncias dos microsserviços isoladamente, garantindo que tenham recursos de computação dedicados. Certifique-se de que a execução de uma instância de microsserviço não afete outras instâncias próximas.

**Foco Na Automação**:
	Foque em automação à medida que o número de microsserviços cresce. Escolha a tecnologia que permite um alto nível de automação. Torne a automação uma parte fundamental da sua cultura organizacional.

**Infraestrutura Como Código**:
	Represente a configuração da infraestrutura por meio de código para facilitar a automação e o compartilhamento de informações. Armazene esse código no controle de versão para facilitar a recriação de ambientes.

**Implantação Com Tempo de Inatividade Zero**:
	Habilite a implantação contínua de novas versões de microsserviços sem qualquer interrupção para os usuários (humanos e outros microsserviços). Procure disponibilidade de serviço ininterrupta durante o processo de implantação.

**Gerenciamento De Estado Desejado**:
	Utilize uma plataforma que mantém os microsserviços em um estado definido. Inicie novas instâncias conforme necessário, em resposta a interrupções ou aumento de tráfego.


#### Teste em uma arquitetura de microsserviços

Existem tantos aspectos e detalhes importantes no teste de _software_ na área de microsserviços que seria necessário dedicar uma aula somente para isso. Entretanto, como não temos esse recurso e nosso foco é dirigido aos microsserviços, e como você provavelmente estudará ou já estudou esse assunto em outra disciplina, focarei apenas em aspectos do teste que são mais importantes do ponto de vista de uma arquitetura de microsserviços.

Todas as granularidades de teste continuam sendo importantes quando se desenvolve uma arquitetura de microsserviços:

![[Pasted image 20240731114319.png]]

![[Pasted image 20240731114342.png]]

![[Pasted image 20240731114354.png]]

Entretanto, no contexto de uma arquitetura de microsserviços, aparece um novo tipo de teste muito eficaz e importante: o **teste baseado em contratos** (que pode, inclusive, substituir, pelo menos em parte, os testes de integração entre microsserviços e os testes ponta a ponta).

O exemplo de teste citado acima ocorreu recentemente no sistema do Nubank. No artigo a seguir, você pode ler mais a respeito.

[Clique aqui](https://building.nubank.com.br/why-we-killed-our-end-to-end-test-suite/) para fazer a leitura.

Os testes de contrato nos permitem definir as interações esperadas entre nossos serviços com base em seus requisitos de entrada e saída. Por exemplo, o serviço de cobrança requer o nome e o sobrenome do cliente para gerar uma fatura. Podemos descrever a interação entre o faturamento e os serviços ao cliente usando o seguinte **contrato**: o serviço fornece o _endpoint_ GET /customers/{id} e espera um **UUID** válido como entrada. Como consumidor desse _endpoint_, o serviço de cobrança espera receber dois atributos: first_name e last_name, sendo que ambos devem ser _strings_ não vazias.

Quaisquer alterações inesperadas nessas suposições, como o atendimento ao cliente tornando o atributo **last_name** opcional (permitindo que ele fique vazio), violaria o contrato. Essas quebras de contrato podem afetar adversamente o comportamento dos processos de negócios durante o tempo de execução e podem ser detectadas por ferramentas de teste de contrato.

Os testes de contrato envolvem uma equipe responsável por um microsserviço que depende de um serviço externo. Esses testes são projetados para descrever o comportamento esperado do serviço externo, em vez de focar o teste do próprio microsserviço.


Vamos a um exemplo: se a equipe desenvolvendo o serviço A sabe que ele necessita e vai chamar o serviço B, ela escreve testes com expectativas de como o serviço B deve se comportar. A partir daí, a equipe que desenvolve o serviço B inclui esses testes que vieram da equipe A em seu conjunto de testes, para que as expectativas da equipe A sejam mantidas pelo serviço B. Observe que esses testes são executados exclusivamente a partir de um único produtor (B, nesse caso), isoladamente. Isso garante um _feedback_ mais rápido e confiável em comparação com os testes ponta a ponta que eles poderiam substituir.


### Monitoramento e observabilidade

Como demonstrado até agora, a decomposição de nosso sistema em microsserviços menores e de granulação fina gera inúmeras vantagens. No entanto, como também discutimos extensivamente, apresenta complexidades consideráveis. Entre essas complexidades, nenhuma é mais aparente do que tentar compreender o comportamento de nossos sistemas em um ambiente de produção.  
  
  
Torna-se evidente, desde o início, que as ferramentas e técnicas que eram eficazes para aplicativos monolíticos de processo único relativamente mais simples não funcionam tão eficientemente no contexto de uma arquitetura de microsserviços.
  
  
Esse assunto também demandaria muito conteúdo para cobri-lo adequadamente. Aqui, vamos apenas indicar alguns caminhos sobre como conseguir atingir um adequado monitoramento de um sistema baseado em microsserviços em direção à observabilidade. Em particular, podemos destacar as seguintes abordagens:

![[Pasted image 20240731115954.png]]

![[Pasted image 20240731120025.png]]

![[Pasted image 20240731120127.png]]

![[Pasted image 20240731120238.png]]

![[Pasted image 20240731120259.png]]

Essas são apenas algumas direções a serem consideradas na busca pela observabilidade de sistemas baseados em microsserviços. Cada aplicação terá suas particularidades, mas investir em estratégias e ferramentas adequadas pode ajudar a enfrentar os desafios inerentes a essa arquitetura e garantir a eficácia operacional do sistema. Algumas ferramentas específicas que poderiam ajudar a implantar as abordagens citadas incluem:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/01 2.png]]

**Prometheus**:
	Uma poderosa ferramenta de monitoramento e alerta que coleta métricas de serviços e infraestrutura. Oferece recursos avançados de consultas e visualização de dados.

**Grafana**:
	Uma plataforma de visualização de métricas e criação de painéis interativos. Com o Grafana, é possível criar _dashboards_ personalizados para monitorar o desempenho e a saúde dos microsserviços.

**Jaeger**:
	Uma ferramenta de rastreamento distribuído que permite rastrear solicitações em ambientes complexos de microsserviços. Com o Jaeger, é possível visualizar o fluxo de uma solicitação em diferentes componentes e identificar gargalos ou problemas de latência.

**ELK Stack**:
	Uma combinação popular de ferramentas para centralização e análise de _logs_. O Elasticsearch é usado para armazenar e pesquisar _logs_; o Logstash, para processamento e enriquecimento de _logs_; e o Kibana para visualização e análise de dados.

**OpenTelemetry**:
	Um conjunto de APIs e bibliotecas que facilitam a instrumentação de microsserviços para coleta de métricas, rastreamento e correlação de solicitações entre diferentes componentes.


Essas são apenas algumas das muitas ferramentas disponíveis no mercado que podem ser úteis para alcançar a observabilidade em sistemas baseados em microsserviços. A escolha das ferramentas mais adequadas dependerá das necessidades específicas do sistema e dos recursos disponíveis. De qualquer maneira, precisamos lembrar que a **observabilidade** se refere ao grau de compreensão que se pode alcançar em relação ao comportamento do sistema por meio de entradas externas. Embora _logs_, eventos e métricas possam contribuir para alcançar a observabilidade, é essencial priorizar que o sistema seja compreensível em vez de depender apenas de várias ferramentas.

### Segurança, resiliência e escalabilidade

Segurança é outro tema que demandaria um curso completo para cobrir o conteúdo adequadamente. Mais uma vez, resumirei alguns assuntos importantes para tratar desse tema no contexto de microsserviços. Em particular, gostaria de focar princípios essenciais de segurança que podem ser mais genericamente aplicáveis em quaisquer sistemas, principalmente aqueles baseados em microsserviços.

Os princípios que gostaria de delinear são: princípio do privilégio mínimo; defesa em profundidade; automação; e inclusão de segurança no processo de entrega. Esses princípios são essenciais para garantir a proteção adequada dos sistemas. Conheça-os detalhadamente:

![[Pasted image 20240731121302.png]]

![[Pasted image 20240731121333.png]]

![[Pasted image 20240731121358.png]]

![[Pasted image 20240731121422.png]]

Esses princípios formam a base para estabelecer uma postura de segurança robusta em sistemas, especialmente em ambientes de microsserviços. Ao aplicá-los adequadamente, é possível criar sistemas mais resilientes e protegidos contra ameaças e violações de segurança.

A resiliência em uma arquitetura de microsserviços é a capacidade do sistema de se adaptar e se recuperar de falhas ou interrupções, mantendo um desempenho aceitável. Um aspecto importante a ser considerado é o teorema CAP, que estabelece que é impossível para um sistema distribuído fornecer simultaneamente consistência, disponibilidade e tolerância à partição. Nesse contexto, é comum adotar uma abordagem que **priorize a disponibilidade** e a **tolerância à partição**, sacrificando a consistência eventualmente.

Um padrão muito utilizado para lidar com falhas em microsserviços é o **_circuit breaker_**. Ele atua como um intermediário entre as chamadas aos serviços e é capaz de detectar falhas de forma rápida. Quando uma falha é detectada, o _circuit breaker_ interrompe temporariamente as chamadas subsequentes, evitando que a falha se propague e sobrecarregue ainda mais o sistema.

Além disso, o _circuit breaker_ também permite a implementação de estratégias de _fallback_, redirecionando as chamadas para uma funcionalidade alternativa ou retornando um valor-padrão, garantindo que o sistema permaneça operacional mesmo quando um serviço específico estiver inacessível.

A escalabilidade em uma arquitetura de microsserviços envolve a capacidade de lidar com o aumento da carga de trabalho e das demandas. Existem vários tipos de escalabilidade que podem ser empregados, incluindo os seguintes:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/01 3.png]]

**Dimensionamento Vertical**:
	Envolve atualizar ou adicionar mais recursos a uma única máquina, como aumentar a potência da CPU, a memória ou a capacidade de armazenamento. Permite lidar com cargas de trabalho maiores em um único servidor (repare que esse tipo de escalonamento pode, inclusive, ser feito com uma arquitetura monolítica).

**Duplicação Horizontal**:
	Refere-se à adição de mais instâncias do mesmo componente, como a implantação de vários microsserviços idênticos ou a adição de mais servidores. Permite distribuir a carga de trabalho em vários recursos e aumenta a capacidade do sistema.

**Partição De Dados**:
	Envolve dividir os dados com base em atributos específicos, como grupos de clientes ou regiões geográficas. Ao particionar os dados, a carga de trabalho é distribuída em vários sistemas de armazenamento, permitindo melhor desempenho e escalabilidade.

**Decomposição Funcional**:
	Essa abordagem envolve a divisão do sistema em microsserviços menores e independentes com base em diferentes componentes funcionais. Cada microsserviço se concentra em um recurso de negócios específico, permitindo escalabilidade por meio do dimensionamento independente de componentes individuais.

Em suma, **o monitoramento e a observabilidade** permitem acompanhar o desempenho dos serviços e coletar métricas e _logs_ para diagnóstico e solução de problemas; a **segurança** abrange medidas para proteger os microsserviços contra ameaças e garantir a confidencialidade, integridade e disponibilidade dos dados; a **resiliência** refere-se à capacidade do sistema de se adaptar a falhas e interrupções, utilizando técnicas como o padrão _circuit breaker_. Já a **escalabilidade** envolve a capacidade de lidar com o aumento de demanda, seja por meio de escalabilidade vertical, horizontal, particionamento de dados ou decomposição funcional. Esses elementos são fundamentais para garantir a eficiência, estabilidade e confiabilidade dos sistemas baseados em microsserviços.

### Conclusão

Cobrimos muitas coisas relacionadas com a implementação de microsserviços, fazendo um _tour_ em dois exemplos de sistemas baseados em microsserviços usando Python. Também cobrimos uma gama de outros assuntos, desde o gerenciamento do _workflow_ em uma aplicação com microsserviço (incluindo o padrão SAGA) até o _build_, com implantação e teste (com os efetivos testes baseados em contrato), segurança (com alguns princípios essenciais), escalabilidade, observabilidade e resiliência de sistemas baseados em microsserviços (com o famoso padrão _circuit breaker_), entre outros. Espero que você tenha aprendido bastante.

### Aplicação

**1. Defina um Microsserviço**: Comece definindo um microsserviço simples. Pode ser um serviço de cadastro de usuários, um serviço de gerenciamento de pedidos etc. Para implementar, utilize a stack definida para o curso.

**2. Implemente a Automação**: Implemente a automação do processo deimplantação de seu microsserviço. Isso pode incluir a automação de testes, a automação de implantação etc. Você pode usar ferramentas como Github Actions, Jenkins, CircleCI, ou outras ferramentas de CI/CD de sua escolha.

**3. Implemente a Defesa em Profundidade**: Adicione (ou pelo menos projete) várias camadas de segurança ao seu microsserviço. Isso pode incluir a autenticação de usuários, a autorização de acesso a recursos e rotas, as validações de entrada etc. Você pode escolher um aspecto de segurança, como por exemplo a autenticação, para implementar neste exercício. Procure usar serviços como o Auth0, que contém uma assinatura inicial grátis, para a autenticação, em vez de implementá-la você mesmo (pois isso envolveria guardar, por exemplo, a senha dos seus usuários no seu banco de dados).

**4. Teste seu Microsserviço**: Finalmente, teste seu microsserviço para garantir que ele esteja funcionando corretamente e que todas as medidas de segurança estejam em vigor.

Este exercício irá ajudá-lo a entender como aplicar os princípios de segurança e automação em uma arquitetura de microsserviços na prática. Lembre-se, a segurança é um aspecto crucial de qualquer sistema de _software_, e é ainda mais importante em uma arquitetura de microsserviços devido à sua natureza distribuída.

**OBSERVAÇÃO**: Você não precisa implementar todos os aspectos descritos, se não for capaz; você pode somente pensar, investigar e descrever como trataria cada um deles com base no conteúdo desta aula.
### Referências:

DOCKER. Docker Documentation. 2023. Disponível em: <[https://docs.docker.com/](https://docs.docker.com/)>. Acesso em: 1 jun. 2023.

FOWLER, M. Microservices. 2014. Disponível em: <[https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html)>. Acesso em: 1 jun. 2023.

KUBERNETES. Kubernetes Documentation. 2023. Disponível em: <[https://kubernetes.io/docs/home/](https://kubernetes.io/docs/home/)>. Acesso em: 1 jun. 2023.

LINKEDIN LEARNING. Microservices Fundamentals. 2023. Disponível em: <[https://www.linkedin.com/learning/microservices-fundamentals](https://www.linkedin.com/learning/microservices-fundamentals)>. Acesso em: 1 jun. 2023.

NEWMAN, S. Building Microservices: Designing Fine-Grained Systems. 2. ed. [S.l.]: O'Reilly Media, 2021.

PERCIVAL, H.; GREGORY, B. Architecture Patterns with Python: Enabling Test-Driven Development, Domain-Driven Design, and Event-Driven Microservices. 1. ed. [S.l.]: Capa comum, 2020.

RED HAT. Microservices architecture: advantages and drawbacks. 2023. Disponível em: <[https://www.redhat.com/en/topics/microservices/advantages-and-drawbacks](https://www.redhat.com/en/topics/microservices/advantages-and-drawbacks)>. Acesso em: 1 jun. 2023.

UDEMY. Microservices with Spring Boot and Spring Cloud. 2023. Disponível em: <[https://www.udemy.com/course/microservices-with-spring-boot-and-spring-cloud/](https://www.udemy.com/course/microservices-with-spring-boot-and-spring-cloud/)>. Acesso em: 1 jun. 2023.

WILSENACH, Rouan. Ship / Show / Ask. 2021. Sisponível em: <[https://martinfowler.com/articles/ship-show-ask.html](https://martinfowler.com/articles/ship-show-ask.html)>. Acesso em: 26 jun. 2023.
## Aspecto Humano na Arquitetura de Microsserviços (Aula 3)

Vamos ver um pouco do aspecto humano quando trabalhamos com uma arquitetura de microsserviços. Repare que a adoção de uma arquitetura, ainda mais uma tão impactante como a de microsserviços, não afeta somente o _software_ desenvolvido — ela influencia também a forma como as pessoas se organizam ao desenvolver o sistema e, até mesmo, como o utilizam. Em particular, vamos ver três fatores aqui: interfaces com o usuário; estruturas organizacionais; e o arquiteto evolutivo.

### Interfaces com o usuário

O mundo das interfaces de usuário ainda precisa ser discutido em detalhes. Embora alguns desenvolvedores possam oferecer interfaces de programação de aplicativos (APIs) “secas” a seus clientes, muitos visam a criar interfaces visualmente atraentes e funcionais, que melhorem a experiência do usuário. A interface do usuário serve como ponte para integrar vários microsserviços em um sistema coerente para os clientes.

Nos primórdios da computação, os aplicativos _desktop_ dominavam o cenário. Esforços foram feitos para melhorar a usabilidade do _software_ por meio de _frameworks_ como Motif e Swing.

Embora esses aplicativos lidassem principalmente com o gerenciamento de arquivos locais, alguns tinham componentes do lado do servidor.

A transição para interfaces baseadas na _web_ introduziu o conceito de UIs “finas”, com mais ênfase na lógica do lado do servidor. Inicialmente, os programas do lado do servidor renderizavam páginas inteiras, que eram enviadas para navegadores clientes com funcionalidade limitada. As interações do usuário eram tratadas por meio de solicitações do lado do servidor acionadas ao clicar em _links_ ou enviar formulários.

Com o tempo, o JavaScript ganhou popularidade por adicionar comportamento dinâmico a interfaces nos navegadores, diminuindo as diferenças entre aplicativos da _web_ e _desktop_.

O surgimento de aplicativos móveis diversificou ainda mais a entrega de interfaces gráficas com o usuário, resultando em uma infinidade de plataformas e tecnologias disponíveis hoje. Essa variedade apresenta aos desenvolvedores inúmeras opções para criar interfaces de usuário eficazes, apoiadas por microsserviços no servidor.

Nos últimos anos, houve uma mudança no pensamento das organizações em relação às interfaces _web_ e _mobile_. Elas agora procuram abordar as experiências digitais de uma maneira mais holística. Em vez de tratar _web_ e _mobile_ separadamente, as organizações estão considerando como os clientes podem utilizar melhor seus serviços e como isso afeta a arquitetura do sistema. Esse entendimento levou à adoção de APIs granulares, como microsserviços, para acomodar diversas interações com clientes (afinal, essas APIs granulares permitem uma interação com o sistema muito mais customizável).

Ao aproveitar os recursos expostos pelos microsserviços de diferentes maneiras, as organizações podem personalizar experiências exclusivas para clientes em aplicativos de _desktop_, dispositivos móveis, dispositivos vestíveis e, até mesmo, locais físicos, como lojas físicas. As interfaces do usuário servem como pontos de integração, em que esses recursos são combinados para oferecer uma experiência coesa ao usuário.

Para enfrentar esse desafio, precisamos abordá-lo sob duas perspectivas.

**O Aspecto Organizacional**:
	Em primeiro lugar, precisamos determinar a propriedade e as responsabilidades dentro da organização para fornecer interfaces de usuário.

**O Aspecto de Implementação**:
	Em segundo lugar, podemos explorar um conjunto de padrões que podem ser empregados para implementar essas interfaces de forma eficaz.

O modelo de responsabilidade mais utilizado na indústria atualmente é ter um time especializado em _front-end_ que cuida de todas as interfaces gráficas de um sistema. Apesar de haver algumas vantagens em se particionar o sistema dessa forma, alguns autores — em particular, Sam Newman — defendem a ideia de que o melhor é optar por equipes multidisciplinares divididas por subdomínio de negócio, e não por conhecimento técnico.

A figura abaixo mostra um exemplo desse tipo de divisão em uma aplicação de comercialização de música, quando é realizada uma alteração para possibilitar que o cliente escolha o seu gênero de música favorito.

![[stb2 2.png]]

Cada equipe — a responsável pelo estoque, a responsável pelo fluxo de compra e a responsável pelo perfil do cliente — tem integrantes especialistas em cada uma das camadas do sistema: interface gráfica (_front-end_), lógica de negócios e dados.

Repare que, quando dividimos os times dessa forma, uma única equipe pode realizar todas as modificações necessárias para implementar a funcionalidade nova de ponta a ponta, sem a necessidade de envolver mais de um time (como no caso de termos uma equipe de _front-end_ dedicada).

### Desafios técnicos

Ao longo dos anos, o desenvolvimento da interface do usuário apresentou evoluções fascinantes, passando de interfaces baseadas em terminais de tela verde para aplicativos de _desktop_ avançados, depois para interfaces da _web_ e agora abrangendo experiências móveis nativas.

De certa forma, fechamos o círculo, pois os aplicativos clientes modernos exibem complexidade e sofisticação que rivalizam com os aplicativos de _desktop_ do passado. Embora certos controles de interface do usuário, como botões, caixas de seleção e formulários, tenham se mantido constantes, a tecnologia subjacente usada para criar interfaces gráficas de usuário evoluiu.

No entanto, tecnologias mais recentes, como **aplicativos de página única** (a famosa _single page application_ — SPA), apresentam desafios na decomposição de interfaces, e a crescente variedade de dispositivos aumenta a complexidade das soluções.

Em última análise, o objetivo é fornecer aos usuários uma experiência de _software_ homogênea, seja por meio de um navegador ou um aplicativo móvel, e integrar a funcionalidade da interface do usuário de forma eficaz, superando os desafios apresentados por aplicativos de página única, dispositivos móveis e outros fatores

A seguir, vamos ver alguns padrões de implementação de interface gráfica com sistemas baseados em microsserviços. 

#### Padrão: _front-end_ monolítico

O padrão _front-end monolítico_ ilustra uma abordagem arquitetônica em que a interface do usuário (UI) gerencia todo o estado e o comportamento, enquanto utiliza microsserviços de apoio para recuperar dados ou executar as operações necessárias.

A figura abaixo fornece um exemplo desse padrão. Nesse cenário, em uma aplicação de comércio de músicas, a interface do usuário solicita dados do microsserviço Álbum para exibir informações sobre um álbum e sua lista de faixas. Além disso, a interface do usuário obtém informações sobre as ofertas especiais mais recentes, consultando o microsserviço de Promoções. Os microsserviços retornam dados em formato JSON (JavaScript Object Notation, um formato muito comum de comunicação na _web_), que a interface do usuário utiliza para atualizar as informações exibidas. Abaixo uma visualização do fluxo:

![[03 8.png]]

O padrão de _front-end_ monolítico é comumente usado no desenvolvimento de aplicativos de página única (SPAs), principalmente quando há uma equipe dedicada de _front-end_ envolvida. Os microsserviços nesse padrão se concentram no compartilhamento de informações em um formato facilmente interpretável pela interface do usuário, geralmente usando JSON para interfaces baseadas na _web_. A interface do usuário é responsável por criar componentes de interface, gerenciar a sincronização de estado com o _back-end_ e manipular dados textuais recebidos de microsserviços.

No entanto, essa abordagem tem suas desvantagens. Veja quais são elas:

![[Pasted image 20240731163531.png]]

![[Pasted image 20240731163544.png]]

![[Pasted image 20240731163631.png]]

![[Pasted image 20240731163731.png]]

![[Pasted image 20240731163819.png]]

#### Padrão: micro _front-ends_

A abordagem de micro _front-end_ é um padrão organizacional que permite que diferentes seções de um _front-end_ sejam desenvolvidas e implantadas de forma independente. É definido como um estilo de arquitetura em que aplicativos de _front-end_ entregues separadamente são combinados para criar um sistema unificado. Esse padrão se torna crucial para as equipes que buscam ter a responsabilidade de ponta a ponta dos microsserviços de _back-end_ e da interface do usuário correspondente. Enquanto os microsserviços oferecem implementabilidade independente para a funcionalidade de _back-end_, os micro _front-ends_ fornecem o mesmo para essa camada da aplicação.

A ascensão de micro _front-ends_ pode ser atribuída aos desafios impostos por interfaces de usuário _web_ monolíticas e pesadas em JavaScript, particularmente em aplicativos de página única. Com micro _front-ends_, várias equipes podem trabalhar e modificar seções distintas do _front-end_.

No contexto da primeira figura mostrada nesta aula, em que as equipes são divididas por subdomínio, e não por tecnologia, as equipes responsáveis ​​por estoques, fluxo de compras e perfis de clientes podem fazer alterações em suas respectivas funcionalidades de _front-end_ de forma autônoma, sem impactar outras equipes.

Quando se trata de _front-ends_ baseados na _web_, existem duas técnicas de decomposição principais que podem facilitar a implementação do padrão de micro _front-end_. Analise-as:

**Decomposição Baseada em Página**:
	A primeira técnica, a decomposição baseada em página, divide o front-end em páginas da web separadas, cada um funcionando de forma independente.

**Decomposição Baseada em Widget**:
	Por outro lado, a decomposição baseada em widget, envolve a integração de vários componentes front-end em uma tela unificada.


A figura a seguir mostra um esquema de como funciona a decomposição baseada em página.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb6.png]]

Com a decomposição baseada em _widgets_, uma tela de uma interface gráfica contém _widgets_ (componentes gráficos) que podem ser alterados independentemente.

Na figura a seguir, é mostrado um exemplo de uma empresa fictícia chamada MusicCorp que vende música _on-line_. Dois _widgets_ apresentam a funcionalidade de UI (1) para o carrinho de compras e (2) para as recomendações.

![[stb7 3.png]]

#### Padrão: _gateway_ agregador

Essencialmente, um _gateway_ de agregação atua como um _hub_ centralizado, conectando interfaces de usuário externas com os microsserviços chamados. Ele filtra e combina com eficiência as chamadas feitas por todas as interfaces de usuário. Ao habilitar a agregação, a interface do usuário pode evitar fazer várias chamadas para recuperar as informações necessárias, reduzindo assim o desperdício de dados recuperados, mas não utilizados.

Um exemplo prático pode ser imaginar que, em uma dada aplicação, queremos apresentar os pedidos recentes de um cliente em uma tela. A tela deve fornecer uma visão geral dos detalhes do cliente e apresentar uma lista cronológica de seus pedidos. Cada entrada de pedido deve incluir informações essenciais, como data, _status_ e preço do pedido, permitindo uma visão resumida do histórico de compras. Se o _front-end_ fosse requisitar as informações diretamente aos microsserviços, ele deveria fazer uma chamada ao microsserviço Cliente, que retornaria TODAS as informações do cliente, e depois uma chamada ao microsserviço Pedido, que retornaria com os cinco últimos pedidos daquele cliente. Note que não precisamos de todas as informações do cliente para essa tela, mas somente de algumas; além disso, o _front-end_ precisa fazer duas chamadas aos microsserviços. Para essa situação, poderíamos incluir um _gateway_ agregador, ao qual o _front-end_ pode fazer somente uma chamada, requisitando somente as informações necessárias. O _gateway_ seria responsável por, de fato, chamar os microsserviços e _agregar_ as informações necessárias, como ilustrado na figura abaixo.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb8 1.png]]

### Padrão: _back-end_ para _front-end_ (BFF — _back-end for front-end_)

A principal diferença entre um BFF (_back-end_ for _front-end_) e um _gateway_ de agregação central está em sua finalidade.

![[Pasted image 20240731165138.png]]

![[Pasted image 20240731165348.png]]

Na figura a seguir, observamos um exemplo em que as interfaces de compras na _web_ e no celular têm BFFs dedicados para melhorar a funcionalidade. Entenda:

![[stb10 3.png]]

### O arquiteto evolutivo

Como estamos falando de pessoas e do desenvolvimento de arquiteturas com microsserviços, um assunto muito importante nesse contexto é o papel do arquiteto de _software_. No âmbito dos microsserviços, esse papel é crucial, porém, muitas vezes, malcompreendido.

A indústria de _software_ é relativamente jovem e não se encaixa perfeitamente na compreensão da sociedade, levando ao empréstimo de termos como “engenheiro” e “arquiteto” de outras profissões. Isso pode levar a equívocos sobre o papel de um arquiteto de _software_. É importante notar que os arquitetos de _software_ não são criadores de planos detalhados, que não levam em conta o futuro imprevisível e a dificuldade de implementar planos; essa descrição, algumas vezes, se encaixa no domínio da construção civil, mas não no domínio de _software_.

O arquiteto é responsável por garantir uma visão técnica coesa para um sistema, atendendo às necessidades tanto dos clientes quanto dos desenvolvedores. Seja trabalhando com uma única equipe ou coordenando várias equipes em uma organização, o papel do arquiteto de _software_ é fundamental para garantir a qualidade dos sistemas e das condições de trabalho e a capacidade de uma organização de se adaptar às mudanças.

A arquitetura de _software_ deve se concentrar em entender o sistema como um todo e garantir uma visão arquitetônica adequada, que possa se adaptar às mudanças. O conceito de 'arquitetura' no desenvolvimento de _software_ trata dos aspectos importantes de um sistema que são difíceis de mudar. É uma **construção social** (no sentido de envolver vários interessados) que depende do consenso do grupo sobre quais partes do _software_ são importantes.

Para se adaptar às necessidades sempre **mutantes** dos usuários e da indústria, os arquitetos de _software_ devem frequentemente adaptar suas ideias. Em vez de visar à criação de um produto final perfeito, eles devem se concentrar em criar uma estrutura que permita que os sistemas certos surjam e evoluam à medida que aprendemos mais. Esse papel pode ser comparado ao de um planejador urbano, que define direções amplas e permite a tomada de decisões locais dentro de certas restrições. Essa abordagem reconhece que o _software_, como uma cidade, precisa mudar e evoluir ao longo do tempo.

### Estabelecendo limites do sistema

Expandindo a metáfora do arquiteto como um planejador de cidade, quais seriam nossas zonas? Estas seriam as fronteiras de microsserviços, ou talvez dos grupos de microsserviços. Como arquitetos, nosso foco deve ser menos no que acontece dentro de uma zona e mais nas interações entre as zonas. Isso implica dedicar tempo para entender como nossos microsserviços se comunicam entre si e garantir que podemos monitorar efetivamente a saúde geral do nosso sistema. Em termos de arquitetura, é assim que criamos nosso próprio espaço universal — ao definirmos limites específicos, indicamos aos nossos colegas que estão construindo o sistema onde as mudanças podem ser implementadas mais livremente, sem interromper um aspecto fundamental de nossa arquitetura.

Em um cenário simples, como mostrado na figura a seguir, o microsserviço de Recomendações recupera informações dos microsserviços de Promoções e Vendas. Como já discutimos extensivamente, podemos modificar livremente a funcionalidade oculta dentro desses três microsserviços, sem o risco de quebrar o sistema geral. Pode-se fazer quaisquer mudanças em Vendas ou Promoções, desde que se continue a cumprir as expectativas que o microsserviço de Recomendações tem sobre suas interações com esses microsserviços chamados.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb11.png]]

Podemos criar espaço para mudanças também em níveis de maior escopo. Na figura a seguir, vemos que os microsserviços da figura anterior, na verdade, existem em uma zona de _marketing_ que se relaciona com a responsabilidade de uma equipe específica. Podemos definir um comportamento esperado em termos de como a funcionalidade de _marketing_ como um todo interage com o sistema maior. Dentro da zona de _marketing_, podemos fazer quaisquer mudanças que desejarmos, desde que a compatibilidade com o sistema maior seja mantida.

Voltando à ideia de entender quais coisas são difíceis de mudar, as estruturas organizacionais geralmente se enquadram nessa categoria; dessa forma, as estruturas de equipe existentes podem nos ajudar a definir essas zonas. Coordenar mudanças dentro de uma equipe entre microsserviços pertencentes a essa equipe será mais fácil do que mudar as interações que são expostas a outras equipes. Isso se alinha bem com o conceito de uma API de equipe.

Um arquiteto pode ajudar a facilitar a criação de uma API de equipe, garantindo que os microsserviços da equipe e as práticas de trabalho se encaixem na organização como um todo. Agora, veja a figura mencionada:

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb12.png]]

### Uma construção social

Então você, como arquiteto, pensou sobre a visão geral, sobre as restrições e sobre o que precisa fazer; você acha que entende o que será difícil de mudar e os espaços onde precisa tornar a mudança possível. E agora? Bem, a arquitetura é o que acontece, e não o que você acha que deveria acontecer — essa é a diferença entre visão e realidade. Os arquitetos do ambiente construído precisam trabalhar com as pessoas que estão construindo o edifício para ajudá-las a entender qual é a visão, mas também para mudar o plano quando a realidade desafia essa visão.

Pode ser que o que você acha que é possível fundamentalmente não seja. Se um arquiteto não estiver, de certa forma, integrado às pessoas que estão criando o sistema, ele será incapaz de comunicar a visão às pessoas que estão fazendo o trabalho — nem mesmo o arquiteto vai entender onde essa visão não é mais adequada. A equipe de construção pode encontrar coisas no terreno que não foram previstas, ou talvez uma escassez de suprimentos possa causar uma reavaliação em termos do _design_.

A arquitetura é o que acontece, e não o que é planejado. Se, como arquiteto, você se afasta do processo de colocar essa visão em prática, então você não é um arquiteto — você é um sonhador. A arquitetura que vai surgir pode ou não ter alguma relação com o que você deseja. Ela vai acontecer com ou sem você.

Implementar uma arquitetura requer o trabalho de muitas pessoas e uma série de decisões, grandes e pequenas.

“No início, a arquitetura de um sistema intensivo de _software_ é uma declaração de visão. No final, a arquitetura de todo esse sistema é um reflexo das bilhões e bilhões de pequenas e grandes decisões de _design_, intencionais e acidentais, feitas ao longo do caminho.” Grady Booch (2020).

Isso significa que, mesmo que você tenha um indivíduo dedicado que é responsável pela arquitetura, há muitas pessoas responsáveis por colocar essa visão em prática. Implementar uma arquitetura de sucesso será um esforço de equipe.

Um ótimo exemplo disso vem da Comcast, que compartilhou suas experiências de como descentralizou a tomada de decisões por meio do uso de uma guilda de arquitetura. Dado o seu tamanho, a Comcast decidiu aproveitar as experiências de vários grupos influentes da indústria, em que a tomada de decisão coletiva é fundamental. Jon Moore, arquiteto-chefe de _software_ da empresa, relatou o seguinte (MOORE, 2019):

“Na Comcast, percebemos que esse problema era muito semelhante ao modo como os órgãos de padrões abertos funcionam: conseguir que vários grupos autônomos cheguem a um acordo sobre abordagens técnicas. Projetamos uma guilda de arquitetura interna explicitamente modelada a partir de uma organização de padrões muito bem-sucedida, a Internet Engineering Task Force (IETF), que define muitos protocolos importantes da Internet.”

### Habitabilidade

Outra ideia que se origina da arquitetura e tem importância no desenvolvimento de _software_ é a noção de **habitabilidade**. Esse termo tem a ver com a ideia de que **o dever de um arquiteto é criar um ambiente de trabalho propício**. Se considerarmos a arquitetura como a estrutura do sistema, definindo como os aspectos inflexíveis se interconectam, pode haver instâncias em que a imposição de limites será necessária. No entanto, se isso não for feito corretamente, o sistema pode se tornar desafiador e propenso a erros.

“A habitabilidade refere-se à qualidade do código-fonte que permite aos programadores que se envolvem com o código posteriormente em seu ciclo de vida compreender sua estrutura e propósito e modificá-lo com conforto e confiança.” Richard Gabriel (1996).

Um ecossistema de desenvolvimento de _software_ contemporâneo compreende mais do que apenas código — inclui também as tecnologias que empregamos e as metodologias de trabalho que seguimos. Frequentemente, testemunhamos desenvolvedores expressando frustração com a tecnologia que eles são obrigados a usar — geralmente uma tecnologia escolhida por indivíduos que, na verdade, não a usam.

Quanto mais colaborativa você tornar a evolução de sua arquitetura e a seleção de suas ferramentas e de sua tecnologia, maior a probabilidade de criar um ambiente habitável, em que os desenvolvedores dos sistemas se sintam satisfeitos e produtivos.

Para garantir que os sistemas que desenvolvemos sejam habitáveis ​​para nossos desenvolvedores, nossos arquitetos e tomadores de decisão devem compreender as consequências de suas escolhas. Isso requer, no mínimo, gastar tempo com a equipe e, idealmente, codificar junto com eles.

Para aqueles que praticam a programação em pares, é fácil para um arquiteto ingressar temporariamente em uma equipe como membro de um par. A participação em atividades de programação conjunta — _mob programming_ — também pode ser benéfica, embora um arquiteto envolvido em tal atividade de grupo deva estar ciente de como sua presença pode alterar a dinâmica do grupo.

É crucial se envolver em tarefas regulares para realmente entender como é o trabalho “normal” do dia a dia.

Não se pode deixar de enfatizar a importância de os arquitetos passarem tempo com as equipes que constroem o sistema. Isso é muito mais eficaz do que uma simples troca de mensagens ou apenas revisar o código. A frequência dessa interação depende muito do tamanho da equipe com a qual você está trabalhando.

No entanto, essa deve ser uma atividade regular. Por exemplo, se você estiver trabalhando com quatro equipes, convém dedicar um turno por mês com cada equipe, auxiliando-as em suas tarefas de entrega. Isso vai ajudar a promover a conscientização e aprimorar a comunicação com as equipes com as quais você está colaborando.

### Uma abordagem baseada em princípios

O processo de tomada de decisões no _design_ de sistemas é repleto de _trade-offs_.

![[Pasted image 20240731174942.png]]

![[Pasted image 20240731174958.png]]

![[Pasted image 20240731175005.png]]

![[Pasted image 20240731175014.png]]

Essa tomada de decisão pode ser facilitada por meio do enquadramento das nossas escolhas dentro de um conjunto de princípios e práticas definidos, que devem se alinhar com os objetivos estratégicos da organização. Veja em detalhes a seguir:

**Objetivos Estratégicos**:
	São as metas de alto nível da empresa. Metas como expandir para novos mercados ou possibilitar o autoatendimento do cliente podem nao envolver diretamente a tecnologia, mas devem ser consideradas ao se alinhar a estratégia tecnológica.

**Princípios**:
	São diretrizes criadas para alinhar ações com objetivos mais amplos. Um exemplo é o Twelve Factors do Heroku, um conjunto de princípios de desgin centrado no objetivo de ajudar a criar aplicações que funcionem bem na plataforma Heroku. Esses princípios também podem ser úteis em outros contextos.

**Práticas**:
	São os meios pelos quais os princípios são implementados. São orientações específicas sobre a realização de tarefas e costumam ser específicas para uma dada tecnologia.

Às vezes, o que pode ser um princípio para um pode ser uma prática para outro, e isso é aceitável. O ponto principal é que há valor em ter ideias gerais que orientem a evolução do sistema e diretrizes detalhadas sobre a implementação dessas ideias. Um exemplo real desses elementos trabalhando juntos foi apresentado por Evan Bottcher. Ele criou um diagrama representando a interação de objetivos, princípios e práticas, destacando que as práticas podem mudar com mais frequência do que os princípios. O diagrama é apresentado a seguir.

![[pos-graduacao/2º Acervo de imagens (Disc. 2)/stb15.png]]

Nesta seção, identificamos as principais responsabilidades de um arquiteto evolutivo. Vamos relembrá-las:

![[Pasted image 20240731175536.png]]

![[Pasted image 20240731175550.png]]

![[Pasted image 20240731175600.png]]

![[Pasted image 20240731175617.png]]

![[Pasted image 20240731175629.png]]

![[Pasted image 20240731175637.png]]

Um arquiteto evolutivo deve equilibrar essas responsabilidades, entendendo que as forças sempre vão pressionar por mudanças. A rigidez no pensamento é contraproducente. Embora esse conselho se aplique a todos os arquitetos de sistemas, os microsserviços exigem mais tomadas de decisão, necessitando de um melhor equilíbrio desses compromissos.

Recomendamos a leitura dos livros a seguir, que podem ajudar os arquitetos a fazerem a ponte entre o pensamento estratégico e a entrega prática.

**_Building evolutionary architectures_**

FORD, N.; PARSONS, R.; KUA, P.; SADALAGE, P. **Building evolutionary architectures**: support constant change. 2. ed. Sebastopol: O'Reilly Media, 2022.

**_The software architect elevator_**

HOHPE, G. **The software architect elevator**: redefining the architect's role in the digital enterprise. Sebastopol: O'Reilly Media, 2020.

### Conclusão

Uma arquitetura de microsserviços também impacta fortemente as pessoas que trabalham no sistema. Em particular, vimos como a interface gráfica pode ser influenciada por essa arquitetura, como ela pode modificar a estrutura organizacional e também como o papel do arquiteto de _software_ deve ser adaptado para esse contexto.

Como você percebeu, a arquitetura de microsserviços envolve muitos aspectos da engenharia de _software_. Espero que você tenha conseguido absorver muitas ideias que o ajudarão a entender o desenvolvimento de arquiteturas de microsserviços e, em muitos pontos, o desenvolvimento de _software_ em geral!

### Aplicação

1. **Estudo de caso**: selecione uma organização que utiliza a arquitetura de microsserviços — pode ser uma empresa conhecida, como a Netflix ou a Amazon, ou uma empresa local que você conheça.

2. **Análise da estrutura organizacional**: analise a estrutura organizacional da empresa. Como as equipes são organizadas? Elas são divididas por funções específicas ou são multidisciplinares?

3. **Impacto da arquitetura de microsserviços**: avalie como a adoção da arquitetura de microsserviços influenciou a forma como as pessoas se organizam para desenvolver o sistema e como o utilizam. Você pode fazer isso por meio de pesquisas ou entrevistas com membros da equipe, se possível.

4. **Relatório**: escreva um relatório detalhando suas descobertas. Inclua uma discussão sobre como a arquitetura de microsserviços pode impactar as estruturas organizacionais e como isso foi evidenciado em seu estudo de caso.

### Referências:

BOOCH, G. (@Grady_Booch, Twitter, 4 set. 2020, 6:12 a.m. Disponível em: <[https://twitter.com/Grady_Booch/status/1301810379161440256?s=20](https://twitter.com/Grady_Booch/status/1301810379161440256?s=20)>. Acesso em: 30 jun. 2023.

FORD, N.; PARSONS, R.; KUA, P.; SADALAGE, P. **Building evolutionary architectures:** support constant change. 2. ed. Sebastopol: O'Reilly Media, 2022.

GABRIEL, R. **Patterns of software**: Tales from the software community. Nova York: Oxford University Press, 1996.

HOHPE, G. **The software architect elevator**: redefining the architect's role in the digital enterprise. Sebastopol: O'Reilly Media, 2020.

MOORE, J. **Architecture with 800 of my closest friends**: the evolution of Comcast’s architecture guild. InfoQ, 14 mai. 2019. Disponível em: <[https://www.infoq.com/articles/architecture-guild-800-friends/](https://www.infoq.com/articles/architecture-guild-800-friends/)>. Acesso em: 30 jun. 2023

NEWMAN, S. **Building microservices**: designing fine-grained systems. 2. ed. Sebastopol: O'Reilly Media, 2021

# Arquitetura em Nuvem e DevOps (Disciplina 3)

## Introdução e DevOps: Primeira Maneira (Fluxo) (Aula 1)

O objetivo da primeira maneira na abordagem DevOps, em que a base é o _Lean_, é acelerar o fluxo da esquerda para a direita. Para que seja possível entregar valor ao cliente de forma continuada e com qualidade (que é uma obrigação e não mais um diferencial), é importante fazer uma boa gestão do fluxo para identificar o melhor caminho para a automação, gerando valor a cada etapa da melhoria contínua.

Nos últimos anos, o valor agregado para a garantia da qualidade do produto ao longo do ciclo de vida do projeto (as famosas atividades de remoção de defeitos) tem sido primordial para o alcance da qualidade e da redução de desperdícios para entregar nossas _features_ ou _releases_ no tempo adequado ao negócio.

Muitas organizações acreditam que as atividades de qualidade, além de terem alto custo, “provocam” atrasos nas entregas para os clientes. Esses discursos podem e devem ser rebatidos, pois é sabido que: “_o custo do retrabalho é muito maior do que fazer certo de primeira”; “a qualidade e revisões de código evitam que erros ocorram lá na frente”; “o custo de remoção de defeito é sempre muito maior_”; etc.

O mundo mudou e cada vez mais, tarefas repetitivas estão sendo realizadas por robôs e serviços inteligentes. Como consequência desse movimento, as empresas terão em seu quadro de funcionários, em algum momento do futuro, essencialmente decisores e especialistas em algoritmos.

Só sobreviverão as organizações que souberem escolher tecnologias, abordagens e processos que absorvam as constantes mudanças onde a necessidade de informação pode mudar a cada segundo, e onde um erro pode resultar em milhões perdidos ou na falência de um negócio.

Por tudo isso, não é possível mais renunciar à qualidade. A automação (DevOps) contribui não só para o aumento da qualidade, mas para a aceleração de tarefas repetitivas e manuais.  
  

O mais importante não é automatizar tudo de primeira, mas automatizar o que vai ter mais **percepção de valor** e seguir em pequenos incrementos de melhoria contínua, guiados por uma boa gestão do fluxo.

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb01.png]]

Como, então, conseguimos alta qualidade em um prazo competitivo?  
Com uma jornada de **melhoria contínua**, com muita automação e colaboração. O triângulo “prazo, escopo e custo”, tão conhecido por todos, parece fazer cada vez mais sentido atualmente.

Quando falamos em agilidade e primeira maneira do DevOps, temos que reduzir o prazo sem renunciar à qualidade. O que nos sobra é priorizar o escopo (descartando aquilo que não tem valor e é desnecessário – olha o _Lean_ aí), cuidar das pessoas e automatizar o máximo possível (com o apoio de ferramentas especialistas) as tarefas repetitivas e/ou essenciais para aumentar a qualidade do produto.

Estes quatro pilares (**pessoas, ferramentas, cultura** e **colaboração**) estão no DevOps, que deriva da junção das palavras “desenvolvimento” e “operações”, como sendo um conjunto de práticas conhecidas da engenharia de _software_ que tem o intuito de unificar o desenvolvimento e a operação de _software_, por meio de transparência, colaboração entre pessoas e muita automação.

### _Overview_ do DevOps

O objetivo do DevOps é tornar os processos mais simples, integrar desenvolvedores e profissionais de infraestruturas, unir equipes e aumentar as entregas aos clientes, agregando velocidade e qualidade a elas. Acompanhe a imagem a seguir:

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb02.png]]

Com base na colaboração dessas equipes e em um conjunto de ferramentas, a tecnologia e as abordagens ágeis permitem às _equipes_ criar uma cultura de colaboração para fugir dos desperdícios e impedimentos automatizando processos: 50% automação e 50% colaboração.

O termo DevOps vem da junção das palavras inglesas _development_ e _operations_, que significam “desenvolvimento” e “operações”, respectivamente. É uma abordagem para a construção e implantação de um produto que busca unir essas duas áreas (que tradicionalmente são separadas), automatizando os processos operacionais em todas as fases do ciclo de vida do produto, não só durante o desenvolvimento.

**DevOps na vida real**

O desafio de implementar o DevOps não é somente selecionar uma tecnologia, mas motivar o setor de tecnologia a se reinventar. Uma mudança cultural e de _mindset_, em que deve haver contínuo apoio motivacional às equipes envolvidas, com respostas claras e comprometimento de todos com as mudanças necessárias à adoção do DevOps. Assista ao vídeo para se aprofundar mais no assunto.

[Clique aqui.](https://www.youtube.com/embed/KbvfV01tSig?start=620)

De acordo com o Guia Ágil (2020), a agilidade pode ser aplicada a qualquer processo de _software_, seja para adaptar tarefas e fazer melhorias, seja para guiar o planejamento. O objetivo principal deve estar em **manter a simplicidade**, enfatizando a estratégia da entrega incremental e evolutiva.

### O que é _mindset_ ágil mesmo?

Dweck (2017) destaca o significado de _mindset_, uma palavra inglesa que significa “pensamento”, “atitude mental”, “moldes mentais”. É a forma de pensar e como a mente está organizada. Mais ainda: como o pensamento se organiza e encara as situações da vivência diária. Já a palavra ágil se refere ao que é eficaz e rápido, diligente, trabalhador, que acha solução rápida e consegue se resolver com facilidade. Que junção poderosa a dessas duas palavras, não acha?

Para apoiar a implantação da Jornada DevOps, existe um princípio chamado de “princípio das três maneiras”. Vamos falar sobre cada um deles, nesta e nas próximas aulas.

**Jornada DevOps**

Para se obterem mais detalhes sobre esse assunto, sugerimos a leitura do livro _Jornada DevOps_, 2ª edição, em que cada maneira desse princípio é abordada profundamente em capítulos colaborativos, com muitos cases e experiências práticas.

Acompanhe a imagem a seguir:

![[stb03 3.png]]

O livro _The DevOps handbook_ (KIM; DEBOIS; WILLIS; HUMBLE, 2016) relaciona as boas práticas de DevOps a três principais objetivos (ou maneiras), para facilitar sua implantação e entendimento.

![[Pasted image 20240802124236.png]]
![[Pasted image 20240802124253.png]]
![[Pasted image 20240802124327.png]]

![[Pasted image 20240802150055.png]]

### CALMS

Segundo o livro _Jornada DevOps_ (MUNIZ et al., 2020, p. 11), “o acrônimo CALMS é muito conhecido para representar a cultura DevOps e foi criado em 2010 como CAMS por John Willis e Damon Edwards. Posteriormente, esse termo foi aperfeiçoado por Jez Humble com a inclusão do _L_ para destacar a importância do _Lean_ para melhoria contínua e processos enxutos”.

O acrônimo CALMS foi criado com base nas seguintes palavras: **colaboração, automação,** **_lean_**, **medição e compartilhamento** (**_sharing_**), e é frequentemente usado na análise de uma organização e, em paralelo, em diversas aplicações.

Implantar o DevOps ou o DevOps CALMS significa não só automatizar, mas também convocar todos os interessados para colaborar. São eles: **negócios, operações, qualidade, segurança** e **desenvolvimento**, que coletivamente fazem a entrega, implantação e integração dos processos automatizados que fazem sentido para os clientes (entrega de valor).

Como será que devemos adotar o CALMS nas organizações? A seguir, vamos ver quais são os passos, de forma macro, que devem ser dados até chegarmos na cultura DevOps CALMS:

![[Pasted image 20240802125007.png]]
![[Pasted image 20240802125019.png]]
![[Pasted image 20240802125030.png]]
![[Pasted image 20240802125051.png]]
![[Pasted image 20240802125116.png]]

### DevOps: primeira maneira

A primeira maneira tem como objetivo acelerar o fluxo do desenvolvimento (esquerda) para operações e clientes (direita) com o uso de diversas técnicas/ferramentas/abordagens, como detalhado na imagem:

![[stb06 3.png]]

Aqui, o objetivo está na **entrega de valor para o cliente**, levando em consideração o fluxo de toda a organização e não os fluxos de cada departamento, desde a concepção (início da solicitação do cliente) até o valor a ser entregue. Com esse mapeamento, é possível identificar, ao longo desse fluxo, desperdícios e oportunidades de automação, para que, cada vez mais, se tenha um _lead time_ (tempo de entrega ao cliente) competitivo e sem perder a qualidade.

A seguir, temos alguns princípios e práticas que apoiam o alcance desse primeiro objetivo da Jornada DevOps:

**Focar o que realmente importa**:
	Limitar o trabalho em execução utilizando o conceito do método Kanban (WIP – _work in progress_). Com essa prática, é possível focar o que realmente importa, garantindo mais qualidade, pois o time está mais focado em uma única tarefa/projeto do que em diversas(os) que nunca conclui. Terminar mais tarefas do que começar novas.

**Tornar o trabalho visível**:
	Por meio da gestão visual, é possível aumentar o fluxo de trabalho e favorecer o autogerenciamento. Todos conseguem visualizar o que precisa ser feito, qual a prioridade e para quando, ou até mesmo se alguém precisa de ajuda (impedimentos).

**Automatizar processos manuais repetitivos**:
	Automatizando processos manuais repetitivos com tarefas automatizadas, que antes eram manuais, é possível liberar as pessoas envolvidas para atuarem em atividades de mais valor para o cliente. Vale automatizar tudo o que for possível, sejam testes, _deploys_, levantamento de ambientes e máquinas virtuais ou artefatos de conformidade (quando a organização precisa atender normas/legislações).

**Identificar e remover desperdícios**:
	Sejam eles em código, infra e/ou processos – muitas vezes, temos em nosso fluxo de trabalho passos desnecessários, que, se identificados e removidos, podem agilizar ainda mais o fluxo.

**Preocupar-se com a qualidade**:
	Preocupar-se com a qualidade desde o início do fluxo de trabalho, para evitar que erros aconteçam e gerem atrasos e gargalos, ou até pior: realizar a entrega sem qualidade.

**Realizar entregas contínuas de pequenos lotes de trabalho**:
	Realizar entregas contínuas de pequenos lotes de trabalho, tornando implantações complexas em atividades simples, tranquilas e com alta qualidade.

### O que é _pipeline_ de implantação?

_Pipeline_ de implantação é o processo de automação do fluxo de valor que leva o _software_ do controle de versão até o ambiente de produção, passando pela integração contínua. Seu objetivo principal é fornecer _feedback_ rápido a todos no fluxo de valor sobre o _status_ das mudanças (principalmente para a equipe Dev). Por isso, colabora com a correção imediata quando algum problema ocorre.

![[Pasted image 20240802151640.png]]

![[Pasted image 20240802151923.png]]

![[Pasted image 20240802152546.png]]

#### Infraestrutura como código (IaC)

Não só o código está versionado, mas as configurações e ambientes (infraestrutura) passam a estar “dentro” do controle de versão. A criação desses ambientes passa a ser automatizada e sob demanda (_self service_) em todos os ambientes, evitando trabalho manual. Todos os estágios do fluxo de valor têm ambientes iguais ou semelhantes aos de produção, evitando erros de infraestrutura. Deve-se derrubar o conceito de “infraestrutura imutável”, em que é melhor recriar todo o ambiente de produção de forma rápida, em vez de realizar alterações em um ambiente já criado.

##### Arquitetura em nuvem (IaaS, SaaS e PaaS)

**IaaS (Infrastructure as a Service) - É a arquitetura mais simples**:
	1º - Oferece infraestrutura de TI automatizada e escalonável - armazenamento, hospedagem e redes - de seus próprios servidores globais, cobrando apenas pelo que o usuário consome.
	2° - Não precisa adquirir licença de software ou servidores e recursos podem ser alocados conforme a necessidade.
	3º - O mercado é dominado pela Amazon (AWS - 38% do mercado), Microsoft (8%) e Google (14%).

**PaaS (Platform as a service) - É uma arquitetura mais difícil de ser definida**:
	1º - Oferece os conceitos básicos de IaaS.
	2° - Além disso, oferece ferramentas e recursos para desenvolver e gerenciar aplicativos com segurança, sem precisar se preocupar com a infraestrutura: sistema operacional, compilação e testes.
	3º - Exemplo: os servidores que hospedam sites são exemplos de PaaS.
	4º - A solução Azure para desenvolvimento de software: Azure DevOps + Azure Services.

**SaaS (Software as a service) - É uma arquitetura já conhecida e mais fácil de entender**:
	1º - O software como serviço (SaaS) é o local onde um software é hospedado por terceiros e acessado pela web, geralmente bastando um login.
	2° - Normalmente, oferece um plano de assinatura, para que seja possível utilizar a solução necessária para algum negócio específico.
	3º - É interessante para o uso de aplicativos específicos, mas, dependendo do negócio e do contrato, o cliente pode ficar dependente da solução e não poder trocar facilmente o serviço por outro fornecedor.

Assim, podemos sintetizar a arquitetura em nuvem como:

![[Pasted image 20240802154143.png]]

##### Vantagens do PaaS

Segundo a Microsoft e a Red Hat, em seus próprios _sites_, existem diversas vantagens no uso de PaaS:  
  
- Ao fornecer infraestrutura como serviço, o PaaS tem as mesmas vantagens que o IaaS e mais alguns recursos adicionais, como:
![[stb10 4.png]]

- Reduz o tempo de codificação e facilita a gestão de capacidade, pois nessa plataforma existem componentes de aplicativos pré-codificados, como: fluxo de trabalho, serviços de diretório, recursos de segurança, pesquisa, etc.

- Desenvolvimento simplificado para diversas plataformas, incluindo aplicativos móveis. Nesse sentido, alguns provedores fornecem opções de desenvolvimento para diversas plataformas, como computadores, dispositivos móveis e navegadores, tornando aplicativos de plataforma cruzada mais rápidos e fáceis de serem desenvolvidos. **Lógico que existe o contraponto da dependência tecnológica da plataforma, por isso o custo x benefício precisa ser sempre analisado.**

- Um modelo pago, conforme o uso, permite que pessoas ou organizações usem um _software_ de desenvolvimento e **ferramentas** de análise e _business intelligence_ sem a necessidade de comprar o produto por completo, levando, em alguns casos, a economia de licenças. De qualquer forma, antes de tomar essa decisão, **faça as contas**. Um arquiteto _cloud_ deve estar sempre com uma calculadora, pois, em alguns cenários, versões _on-premise_ e híbridas podem ser mais vantajosas.

- Como o ambiente de desenvolvimento é acessado pela internet, equipes de desenvolvimento podem trabalhar em conjunto sem problemas, mesmo quando existem times geograficamente distribuídos.

- A estrutura PaaS fornece todas as funcionalidades para o suporte ao ciclo de vida completo de um aplicativo _web_. Por exemplo: compilação, teste, implantação, gerenciamento e atualização no mesmo ambiente integrado.

##### O conceito de _serverless_

Muitos entendem que o conceito de _serverless_ significa somente a ausência de servidores físicos, mas não é bem assim:  

- Ainda existem servidores, apesar do nome.

- O desenvolvedor não se preocupa em configurar ou conhecer outros aspectos da infra em que sua aplicação vai rodar.

- Podem ser divididos em: _backend_ as a _service_ (BaaS) e _function as a service_ (FaaS).

- Você paga pelo uso (cada vez que a função é executada). De novo: é preciso sempre analisar o custo x benefício dessa modalidade de nuvem.

- _Frameworks serverless_.

**Os principais frameworks do mercado são:**  
  
1. **Node.js**: o _serverless_ é um _framework web_ e _open source_.

	- Inicialmente, era destinado exclusivamente para a criação de aplicações para o AWS Lambda, plataforma da Amazon Web Services de _serverless cloud computing_.
	- Agora, está compatibilizado com outros fornecedores de _cloud_: Microsoft Azure, IBM BlueMix, Google Cloud e Oracle Cloud, entre outros.  
    

**Cuidado: ao usar, não se esqueça de que é diferente de um desenvolvimento para _cloud_ tradicional.**

2. **Up**: também é um _framework open source_.

	- Não tem funcionalidades.
	- Adapta seu código para rodar na arquitetura _serverless_. 

**Cuidado: seu código não poderá utilizar as funcionalidades especiais dos provedores _serverless_.**

Quando você usa FaaS, compartilha o tempo de execução com outras pessoas. Por exemplo: quando sua “função” é escrita em JavaScript, essa parte do código será executada no mesmo servidor node.js que as “funções” de outros usuários desse FaaS (isso pode ser diferente para alguns fornecedores). Ao usar o BaaS, você compartilha o mesmo BaaS.

![[stb11 4.png]]

Os exemplos práticos facilitam o entendimento e materializam conceitos teóricos.

#### Testes automatizados, _branching e releases_ de baixo risco

Devemos priorizar os testes unitários que têm execução mais rápida do que os testes de aceite e integração. Além da economia de tempo, outro grande benefício é que os desenvolvedores recebem _feedback_ de imediato no teste unitário, ficando mais eficiente a correção na origem.

![[stb12 2.png]]

##### Estratégia de _branching_

A estratégia de _branching_ é fundamental para que tenhamos mais colaboração e facilidade não só na integração contínua, mas também na construção dos gatilhos da _pipeline_ de implantação ou entrega contínua.

Na tabela a seguir, temos duas das mais comuns estratégias e suas vantagens e desvantagens:

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb13.png]]

##### Categorias de liberação (_release_)

É importante que o time planeje a _release_, ou a implantação de um pacote, e defina, junto com a operação, formas de reversão do _deploy_ (plano de contingência), caso se detecte algum problema. Exemplos de reversão são: _release_ canário (implantar a versão anterior) ou alternância de recursos/_feature toggle_ (incluir na aplicação uma função de ligar/desligar a funcionalidade sem precisar voltar à versão anterior à implantação).  
  
Em caso de maturidade em testes automatizados com alta cobertura, é possível seguir com o _fix forward_, consertar o código imediatamente e implantar seguindo as regras da _pipeline_ para entrega contínua.

As categorias de _releases_ podem ser feitas de duas formas:

- **Com base no ambiente:**
	Há dois ou mais ambientes, sendo que apenas um fica ativo para os clientes (ex.: balanceadores) – azul-verde (_blue-green_) e canário (_canary_).
![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb14.png]]

- **Com base no aplicativo:**
	Novas funcionalidades de forma seletiva, usando configurações simples (não é preciso fazer _deploy_).
	Alternância de recursos (_feature toogles_) e lançamento escuro.


##### O que é “alternância de recursos” (_feature toggle_)

- Habilita e desabilita recursos da aplicação, de acordo com critérios definidos (ex.: funcionário e localidade).

- Usa instrução condicional por meio de parâmetros ou configuração, sem necessidade de _deploy_.

- Permite **lançamento escuro**:
	Implantação de recursos na produção para avaliar resultados, sem o usuário perceber.

##### Conceito de arquitetura de baixo risco

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb15.png]]

A arquitetura de baixo risco, como o próprio nome indica, permite que implantações possam ser realizadas de forma frequente, pela facilidade, quando um erro é descoberto. Por exemplo: voltar a uma versão anterior ou seguir com os ajustes necessários.

#### Testes automatizados

![[Pasted image 20240802162324.png]]

![[Pasted image 20240802162335.png]]

![[Pasted image 20240802162806.png]]

![[Pasted image 20240802163013.png]]

![[Pasted image 20240802163137.png]]

![[Pasted image 20240802163150.png]]

#### _Release_ de baixo risco

![[Pasted image 20240802163509.png]]

![[Pasted image 20240802163546.png]]

![[Pasted image 20240802163617.png]]

![[Pasted image 20240802163806.png]]

![[Pasted image 20240802163835.png]]

![[Pasted image 20240802164035.png]]

![[Pasted image 20240802164108.png]]

![[Pasted image 20240802164149.png]]

![[Pasted image 20240802164157.png]]

![[Pasted image 20240802164225.png]]

### Referências:

DWECK, C. S. **Mindset**: the new psychology of success. London: Robinson, 2017.

EDMONDSON, A. C. Strategies for learning from failure. **Harvard Business Review**, Apr. 2011.

EDMONDSON, A. C. The competitive imperative of learning. **Harvard Business Review**, July-Aug. 2008.

KIM, G.; DEBOIS, P.; WILLIS, J.; HUMBLE, J. **The DevOps handbook**: how to create worldclass agility, reliability, and security in technology organizations. Portland: IT Revolution Press, 2016.

MICROSOFT. O que é PaaS? **Microsoft**, [20--?]. Disponível em: [https://azure.microsoft.com/pt-br/resources/cloud-computing-dictionary/what-is-paas/](https://azure.microsoft.com/pt-br/resources/cloud-computing-dictionary/what-is-paas/). Acesso em: 21 mar. 2023.

MUNIZ, A.; IRIGOYEN, A. **Jornada ágil e digital**. Rio de Janeiro: Brasport, 2019.

MUNIZ, A.; IRIGOYEN, A.; GAMA, F.; CARRASCO, J.; COSTA, M.; ENOMOTO, N.; IRIGOYEN, R. **Jornada Azure DevOps**. Rio de Janeiro: Brasport, 2022.

MUNIZ, A.; SANTOS, R.; IRIGOYEN, A.; MOUTINHO, R. **Jornada DevOps**. Rio de Janeiro: Brasport, 2019.

PRESSMAN, R. S. Engenharia de software. 5. ed. Rio de Janeiro: McGraw-Hill, 2011.

RED HAT. IaaS x PaaS x SaaS. **Red Hat**, 2022. Disponível em:[https://www.redhat.com/pt-br/topics/cloud-computing/iaas-vs-paas-vs-saas](https://www.redhat.com/pt-br/topics/cloud-computing/iaas-vs-paas-vs-saas). Acesso em: 21 mar. 2023.

TEMPOS MODERNOS. Direção: Charlie Chaplin. Estados Unidos: United Artists, 1936. Disponível em: [https://archive.org/details/modern-times-1936](https://archive.org/details/modern-times-1936) (87 min).

## Segunda Maneira - Rápido Feedback (Aula 2)

O principal objetivo da segunda maneira na abordagem DevOps é implantar abordagens que permitam a obtenção de um rápido _feedback_. Nesse sentido, para que seja possível entregar qualidade ao cliente, é imprescindível que os erros sejam encontrados e ajustados rapidamente, de preferência no início do ciclo de desenvolvimento. As diversas técnicas/abordagens e boas práticas que destacaremos a seguir nos ajudam a “errar e consertar mais rápido ainda”.

A segunda maneira da Jornada DevOps tem como objetivo o rápido _feedback_, conforme ilustrado a seguir, em todos os estágios do fluxo de um produto, acelerando as descobertas que só teríamos ao final do fluxo (mais à direita) para o início do fluxo (mais à esquerda). Nesse sentido, quanto mais rápido o _feedback_, mais rápido sabemos se acertamos e erramos e mais rápido ainda podemos ajustar problemas e erros.

Estes são alguns dos insumos fundamentais para um fluxo cada vez mais contínuo e automatizado:  

- conhecimento de desenvolvimento do time;
- aprendizado de segurança;
- entendimento dos conceitos da disciplina de operação;
- priorização da própria qualidade do processo e do _software_;
- experiência do cliente;
- criação de ambiente de forma automatizada e rápida.

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/stb01 1.png]]

A segunda maneira aborda boas práticas já conhecidas em disciplinas anteriores de engenharia de _software_, mas com o foco em automatizar o máximo possível com a colaboração do time. A segunda maneira permite que as empresas se adaptem rapidamente às mudanças do mercado, contribuindo para o atendimento às demandas dos clientes de forma mais rápida e eficaz.

![[Pasted image 20240805180804.png]]

![[Pasted image 20240805181039.png]]

![[Pasted image 20240805181003.png]]

![[Pasted image 20240805181151.png]]

![[Pasted image 20240805181402.png]]

![[Pasted image 20240805181447.png]]

A seguir, listamos alguns princípios e práticas que apoiam o alcance desse segundo objetivo da Jornada DevOps.

#### Telemetria

É a coleta remota e automática de dados para monitorar a saúde das aplicações e de seus ambientes. A telemetria apoia, também, a análise do risco de liberação de versões em desenvolvimento/homologação e/ou produção com o _feedback_ de eventos, métricas e registros em toda a cadeia do fluxo.

Esse monitoramento deve ser proativo, para que seja possível detectar vulnerabilidades nesses diversos ambientes como _feedback_ para o desenvolvimento, e não só para a área de operações (a situação mais comum em grandes empresas).

A seguir, a figura ilustra um exemplo de _framework_ de monitoramento, que tem métricas de diversos tipos: aplicativo, atividades de negócio e sistema operacional.

![[stb02 1 1.png]]

Para que seja possível um rápido _feedback_, é fundamental que tenhamos o conceito de **telemetria _self-service_**, ou seja, indicadores disponíveis para todos os envolvidos no fluxo (incluindo o cliente), democratizando esse tipo de _feedback_. A cultura de métrica deve ser incluída no dia a dia de todas as equipes.

#### Visão clara do fluxo e o trabalho diário de desenvolvedores e operação

Juntos, todos são responsáveis pela melhoria contínua e condução proativa de verificações. Quando estudamos abordagens ágeis, normalmente o método _kanban_ é mencionado ou, algumas vezes, até mesmo aprofundado. Apesar de existirem alguns _experts_ em _kanban_ que não o consideram uma abordagem ágil, é claro (e isso todos concordam) que esse método foi popularizado pela agilidade e pelo Manifesto Ágil, principalmente pelo _scrum_ não só usar o quadro _kanban_, mas muitos dos seus conceitos. Nesse sentido, quando se inicia o método _kanban_, o primeiro passo é estabelecer/definir uma visão clara do fluxo de trabalho, que é essencial para que seja possível aplicar os diversos conceitos, práticas e métricas propostas pelo método.

Através do fluxo de valor, que é representado e fica visível no quadro _kanban_, é possível identificar gargalos, calcular o _lead time_ e o _cycle time_ e ainda analisar o gráfico do diagrama do fluxo cumulativo (CFD).

O _lead time_ (que é o tempo que se leva para entregar um serviço/produto ao cliente desde a sua solicitação) é usado no DevOps para que seja possível priorizar automações que diminuam cada vez mais esse ciclo sem que a qualidade seja perdida. No DevOps, a qualidade é sempre prioridade do time. Da mesma forma, a métrica _cycle time_ ou tempo de ciclo (que é o tempo que se leva desde que foi estabelecido o compromisso com o time para entregar determinada solicitação do cliente até a entrega propriamente dita) é utilizada para que o time priorize qual etapa deste pode ser automatizada para diminuir esse tempo e aumentar o _feedback_ sobre o processo e o trabalho dos diversos times envolvidos no fluxo de valor.

#### Gemba

_Gemba_ é um conceito que vem do _lean_ e significa “**ir e ver**” com os seus próprios olhos o que está acontecendo para propor melhorias e/ou ajustes. Por exemplo, se o problema é na utilização do aplicativo do cliente, gere empatia e vá até o cliente para entender qual é a dificuldade real. Essa atitude se aplica a todas as etapas do fluxo e a todos os participantes do fluxo.

A empatia está muito ligada a essa prática. Ficar reclamando, por exemplo, que o formulário de gestão de mudanças (GMUD) é burocrático não resolve o problema. Muitas vezes, ir à área e entender o problema e o motivo dessa GMUD pode agilizar o _feedback_ e melhorias conjuntas (automatizando as etapas da GMUD e reduzindo os riscos na operação).

#### Corda de _andon_

O DevOps, cuja base é a agilidade e o _lean_, não cria conceitos teóricos ou metodologias, mas usa ferramentas para que seja possível automatizar etapas da engenharia de _software_ e aumentar a colaboração através das abordagens ágeis. Diante desse conceito, uma importante prática do _lean_ destacada no DevOps é a corda de _andon_. Usada na Toyota, significa a junção de todos do time para resolver (e não com o foco de procurar culpados) sempre que um problema é detectado ao longo do fluxo. Essa prática não só favorece a resolução de problemas críticos como também potencializa o sentimento de pertencimento e de que todos são os donos da solução, além de que o time sempre pensa melhor do que só uma pessoa.

#### Listas de revisão de segurança

É um papel exercido pelo Site Reliability Engineering – SRE, criado pela Google. Na indicação de leitura a seguir, você terá mais informações sobre SRE.

Conheça mais sobre SRE com a rápida leitura de “O que é engenharia de confiabilidade do _site_ (SRE)?”.

[Clique aqui.](https://sre.google/)

#### Plantão 24 x7 compartilhado

É importante deixar claro que, mesmo que tenhamos uma boa cobertura de testes automatizados, isso não garante zero erro em produção; aliás, nada garante. Mesmo que seja comum no mercado envolver somente a área de sustentação durante a implantação em produção, é importante que todos os participantes do fluxo de valor compartilhem as responsabilidades para resolver os incidentes em produção. Essa prática gera empatia, aprendizado e sensação de pertencimento do mesmo time.

![[stb03 1 1.png]]

#### Testes A/B

Entendendo que DevOps é um conjunto de boas práticas existentes no mercado, testes A/B são uma dessas técnicas. Usar a técnica praticada pelo _marketing_ favorece o rápido _feedback_ e o desenvolvimento de pequenos lotes, ou até mesmo o não desenvolvimento (código), e a utilização de formulários e pesquisas para entender se realmente é algo que o cliente quer que seja ser desenvolvido, evitando, assim, desperdícios de tempo e de recursos (incluindo desperdício de código).

Mais detalhadamente, essa técnica é usada em _marketing_ para avaliar o resultado imediato e entender a experiência do usuário (UX), sendo bastante útil quando desejamos experimentar novos recursos e tomar decisões com base em fatos e dados. Os testes A/B podem ser aplicados através de formulários, pesquisas, entrevistas ou qualquer outro meio que permita coletar os dados de _feedback_ do cliente sobre uma funcionalidade ou futura funcionalidade de um aplicativo.

#### Desenvolvimento por hipóteses

O uso de hipóteses, em substituição à palavra “requisitos”, é importante para confirmar se novas funcionalidades serão realmente adotadas pelos clientes. Trabalhar com hipóteses nos “livra” do peso de desenvolver algo que de fato vai ser usado pelo usuário.

Quando pensamos em hipóteses, direcionamos os nossos esforços para obter um rápido _feedback_ sobre o que realmente importa para o cliente, e não uma interpretação do que achamos que o cliente vai usar. Isso facilita a definição do MVP (produto mínimo viável) e de funcionalidades mais enxutas para que seja possível obter um rápido _feedback_.

#### Revisão de código (_pull request_)

Uma das formas mais comuns de revisão de código é o _pull request_ (PR), em que o desenvolvedor solicita revisão de forma colaborativa após concluir uma mudança no código. Esse processo é muito usado no GitHub, no GitLab e/ou no Azure DevOps.

![[Pasted image 20240806112722.png]]
![[Pasted image 20240806112749.png]]
![[Pasted image 20240806112818.png]]
![[Pasted image 20240806112845.png]]
![[Pasted image 20240806112920.png]]
![[Pasted image 20240806112943.png]]
![[Pasted image 20240806113018.png]]
![[Pasted image 20240806113038.png]]

_Pull request_ é o termo usado pelo mercado, popularizado pelo GIT inicialmente, para a boa prática de engenharia de _software_ de revisão de código por pares (ou por um especialista). 

#### PRs e estratégia de _branching_ e técnicas de revisão (programação em pares)

_Pull requests_, juntamente com as estratégias de _branching_ e técnicas de revisão, facilitam a integração, contribuindo para que o código seja entregue com qualidade. 

![[Pasted image 20240806114634.png]]

![[Pasted image 20240806114722.png]]

![[Pasted image 20240806114928.png]]

![[Pasted image 20240806115128.png]]

![[Pasted image 20240806115338.png]]

![[Pasted image 20240806115454.png]]

![[Pasted image 20240806115542.png]]

![[Pasted image 20240806115622.png]]

Rápidos _feedbacks_ só são possíveis quando temos uma boa estratégia de _branching_ e uma revisão de código que aconteça. Aprovar o código só por aprovar sem realmente realizar a revisão não garante um código de qualidade. Todos nós podemos errar. Não abra mão da tranquilidade de ter seu código revisado.

Vale a pena acompanhar esta excelente discussão entre especialistas sobre diversas possibilidades de estratégias de _branching_, inclusive a mais popular (GitFlow). Nesta conversa entre amigos, é possível perceber diversos cenários diferentes nos quais a estratégia pode até ser diferente, mas a cultura e a política são as mais ressaltadas.

[Clique aqui.](https://open.spotify.com/episode/0glbsRgetP7kQcNDIBrdSg?si=4964923802024921&nd=1)

Rápidos _feedbacks_ potencializam aprendizados e aumentam a qualidade do trabalho do time e, principalmente, da solução dada. O pensamento adequado para todas essas boas práticas que vimos até agora é: erre, mas conserte mais rápido ainda.

### Tipos de reversão quando temos problemas na implantação

1. Correção: fix forward
	É uma mudança no código e deve ser executada em ambientes com grande maturidade: com alta cobertura de testes automatizados, implantação rápida e telemetria.

2. Reversão: Rollback
	Usuário não recebe a nova versão em produção, e a versão é disponibilizada de duas formas:
	- Implantar a versão anterior (p. ex., canário).
	- Alternância de recursos (_feature toggle_): mais fácil de reverter e menos arriscada. Você pode materializar essa forma como se fosse uma configuração administrativa no próprio aplicativo que ligasse ou desligasse uma funcionalidade, algo fácil como se fosse ligar o modo avião do telefone celular, por exemplo. Algumas linguagens permitem marcar um código que não está pronto e que não será “executado” em produção.

Lembre-se de que é importante ter opções de reversão disponíveis para que a equipe possa agir rapidamente e minimizar o impacto nos usuários finais.

#### Usar a experiência do usuário (UX) como _feedback_

Usar a experiência do usuário como feedback é uma boa prática da segunda maneira, pois permite:

- Mostrar todas as dificuldades na prática (cliques numerosos, lentidão, transição de várias telas, migração de dados para outros sistemas etc).
- Gerar maior **empatia** e incentivar as equipes.
- Que a **pesquisa contextual** ocorra quando a equipe do produto observa um cliente usar a aplicação em seu ambiente natural.

#### Testes A/B, experimentação e desenvolvimento por hipóteses

Testes A/B, experimentação e desenvolvimento por hipóteses são práticas fundamentais em DevOps para garantir que o _software_ entregue atenda às necessidades dos usuários com vários ciclos de _feedback_.

![[Pasted image 20240806120907.png]]

![[Pasted image 20240806121105.png]]

![[Pasted image 20240806121230.png]]

![[Pasted image 20240806121337.png]]

É impressionante como nem sempre automatizar é a solução de todos os problemas. As práticas que vimos de testes A/B, experimentação e desenvolvimento por hipóteses podem acelerar o _feedback_ sem que sejam criados códigos, ou, quando envolvem codificação, tenham sua quantidade reduzida (uma espécie de MVP), evitando, assim, desperdícios diversos, e o melhor: com entendimento do que realmente o cliente final deseja.

A cultura _lean_ ágil de melhoria contínua e a automação são elementos essenciais do DevOps, pois juntas permitem que as equipes entreguem _software_ de alta qualidade de forma rápida e eficiente, enquanto continuam a melhorar e evoluir continuamente. Porém, algumas questões sobre esse assunto devem ser respondidas com um olhar crítico. Acompanhe no _podcast_ a seguir.

**A cultura _lean_ ágil de melhoria contínua como pilar da automação (DevOps)**
 
**Reflita sobre as questões a seguir:**

- Preciso automatizar tudo de primeira?

- Como trilhar a jornada DevOps de forma evolutiva?

- Como convencer a alta direção sobre os custos da automação?

- Existe uma forma única para iniciar e manter a jornada DevOps?

**Agora, ouça os dois _cases_ nos _podcasts_ a seguir antes de continuar:**

[**_Case_ 1**](https://open.spotify.com/episode/7sD3DPMbVoOWCnHDXLqBZT?si=ebc30fda4e304966)

[**_Case_ 2**](https://open.spotify.com/episode/3pThcMlk6KlzMgio77hI8F?si=l-hwjshcSRm8PQCycHQP-A)


**Por fim, você pode ler um resumo dos _cases_ a seguir:**

Não precisamos automatizar tudo de primeira. A importância da aplicação de conceitos _lean_, base do _scrum_ e do _kanban_, está na possibilidade de fazer a gestão do fluxo e entender as etapas que precisam ser automatizadas primeiro (seja pela identificação de gargalos ou tempo de execução). Quando automatizamos uma etapa, além de ganharmos tempo, ganhamos qualidade. E a cada ciclo de melhoria essa automação pode ser priorizada, sempre de forma evolutiva.

Em cada contexto (que depende de projeto, time, produto, complexidade do negócio, atendimento de legislação), a jornada de automação pode e deve ser diferente. Por isso a importância da transparência e de entender exatamente o seu fluxo e onde a automação pode gerar ganhos reais. Esses ganhos reais podem ser calculados com as métricas existentes de gestão de fluxo no _kanban_ (_throughput_, tempo de entrega, tempo de ciclo, BDC, redução de número de defeitos). Quando falamos em ganhos e mostramos os resultados a cada ciclo evolutivo de melhoria, a alta direção é a parte mais fácil de convencer. Escolha a automação de testes, por exemplo, priorizando os cenários que levam mais tempo ou os cenários que têm maior manutenção ou aqueles que são mais utilizados pelos usuários. Pergunte-se: o que é prioritário (o que gera mais valor) e leva menos tempo para automatizar? Priorize os famosos _quick wins_.

Outros pontos importantes para o sucesso de uma Jornada DevOps são colaboração, políticas explícitas, confiança e coragem. Confiança e coragem do time para falar/mostrar as dificuldades/impedimentos, seguir as políticas, priorizar em toda _sprint_ as melhorias de processo (com ou sem a automação) e realizar uma revisão por pares profunda sem medo de receber críticas ou ser crítico com a qualidade do que está sendo construído. Qualidade é mais importante que velocidade, e, por incrível que pareça, quanto mais qualidade tem o seu código, maior é a agilidade em sua manutenção.

### Referências:

DWECK, C. S. **Mindset**: the new psychology of success. London: Robinson, 2017.

EDMONDSON, Amy C. Strategies for learning from failure. **Harvard Business Review**, abr. 2011.

EDMONDSON, Amy C. The competitive imperative of learning. **Harvard Business Review**, jul-ago. 2008.

KIM, Gene; DEBOIS, Patrick; WILLIS, John; HUMBLE, Jez. **The DevOps handbook**: how to create world-class agility, reliability, and security in technology organizations. Portland: IT Revolution Press, 2016.

MUNIZ, Antonio; IRIGOYEN, Analia. **Jornada ágil e digital**. Rio de Janeiro: Brasport, 2019.

MUNIZ, Antonio; IRIGOYEN, Analia; GAMA, Fabrício; CARRASCO, Joana; COSTA, Marcelo; ENOMOTO, Norberto; IRIGOYEN, Ricardo. **Jornada Azure DevOps**. Rio de Janeiro: Brasport, 2022.

MUNIZ, Antonio; SANTOS, Rodrigo; IRIGOYEN, Analia; MOUTINHO, Rodrigo. **Jornada DevOps**. Rio de Janeiro: Brasport, 2019.

PRESSMAN, R. S. **Engenharia de software**. 5. ed. Rio de Janeiro: McGraw-Hill, 2011.

## Terceira Maneira (Aprendizado): Gestão de Mudanças e DevSecOps (Aula 3)

A terceira maneira tem como objetivo principal criar uma cultura de confiança para que seja possível errar e aprender com os erros. É importante correr riscos para potencializar um aprendizado contínuo.

A terceira maneira é fundamental para que a cultura DevOps esteja presente e preservada nos times. Sem ela, a cultura de automação e colaboração vai se enfraquecendo ao longo do tempo. A automação é uma jornada e identificar onde estão os gargalos e os alvos de automação requer muita colaboração e transparência. Temos que habituar os times em que trabalhamos a melhorar continuamente até a perfeição. Porém, como a perfeição não existe, a melhoria contínua não deve ter fim.

![[stb01 2.png]]

Existem diversos conceitos, princípios e práticas que potencializam o aprendizado e a experimentação, já que não é possível aprender sem experimentar ou se permitir errar. Vamos conhecer os principais?

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/01.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/02.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/03.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/04.png]]

![[pos-graduacao/2º Acervo de imagens (Disc. 3)/05.png]]

![[06.png]]

As práticas de aprendizagem multidisciplinares da terceira maneira demandam cada vez mais profissionais DevOps especialistas-generalistas. Esses profissionais devem conhecer e ter experiência em diversas áreas e se especializar naquelas com que se identificam mais.

#### A importância da terceira maneira e o profissional DevOps

![[Pasted image 20240807144034.png]]
![[Pasted image 20240807144110.png]]
![[Pasted image 20240807144222.png]]
![[Pasted image 20240807144437.png]]
![[Pasted image 20240807144627.png]]

#### O profissional DevOps

![[Pasted image 20240807144951.png]]

### Introdução a segurança e gestão de mudanças

A imagem a seguir representa que objetivos diferentes – desenvolvimento, operações e _compliance_ – podem ser entendidos como um obstáculo ao DevOps.

![[stb03 2 1.png]]

No entanto, é exatamente o contrário: com as automações, temos diversos benefícios. Veja alguns deles:

**Melhor organização e colaboração entre os profissionais**:
	Com a automação, cria-se uma cultura de independência durante a realização das atividades, principalmente as que envolvem Dev e Ops.

**Definição de níveis de acesso adequada**:
	Com a automação, cada profissional tem o perfil adequado, sem a necessidade de acesso direto à máquina de produção ou homologação, evitando confusões e ruídos de comunicação, por exemplo.

**Maior controle de horas e lead-time (tempo total de entrega ao cliente)**:
	Com a automação, as métricas são criadas de forma automática, gerando mais confiabilidade para melhorias e análises de causa-raiz.

**Redução de custos e aumento de produtividade**:
	Com a automação de processos repetitivos, há mais produtividade, qualidade e menos retrabalho. Os times ficam focados e motivados por trabalhar em tarefas que exigem mais criatividade. Além disso, há ferramentas específicas que detectam vulnerabilidades de segurança e falta de qualidade mínima do código (por exemplo, Sonar).

**Gerenciamento mais inteligente**:
	O gestor consegue criar relatórios gerenciais com poucos cliques para acompanhar os processos, facilitando a tomada de decisões em tempo hábil.

Qual auditor ou responsável por segurança da informação ou qualidade não perceberá tantos benefícios e aumento da qualidade e produtividade com evidências e _logs_ automáticos de todas as atividades realizadas com pouca/nenhuma intervenção humana?

Conforme a tabela a seguir, para orquestrar (integrar) todas essas ferramentas, são necessários um bom processo automatizado e muito conhecimento de arquitetura, gestão, qualidade, engenharia de _software_, serviços e inovação.

![[stb05 3.png]]

### Aprendizagem e experimentação

Alvin Toffler, em uma de suas frases mais conhecidas, diz: “Os analfabetos do futuro não serão os que não sabem ler ou escrever, mas os que não sabem aprender, desaprender e reaprender”. Isso resume muito bem a terceira maneira do DevOps. Com a infinidade de ferramentas/tecnologias lançadas diariamente, estamos exercitando nosso aprendizado o tempo todo.

Uma das formas de estimular o aprendizado é utilizar os erros que ocorrem com mais frequência para gerar novos aprendizados. Nesse sentido, para o verdadeiro aprendizado, é necessário combater a teoria da “maçã podre”, que busca “eliminar as pessoas que causaram os erros”.


A seguir, abordaremos as práticas de aprendizagem e experimentação mais difundidas na comunidade DevOps:  
  
- Tipos de macaco do exército símio (_case_ Netflix).
- Reunião _post-mortem_ livre de culpa.
- Dias de jogos.
- Descobertas.

#### _Case_ da Netflix

Conforme detalhado no livro _Jornada DevOps_ (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019): “o time de engenheiros da Netflix criou um processo para injeção de falhas chamado Chaos Monkey, que foi criado em resposta ao movimento de mover a aplicação de uma infraestrutura física para uma infraestrutura física na nuvem provida pela AWS (Amazon Web Services)”.

O Chaos Monkey evoluiu para novos macacos, chamados de “exército símio”. São eles:

**Chaos Gorilla**:
	Simula a falha de uma zona inteira de disponibilidade AWS (Amazon Web Service).

**Chaos Kong**:
	Simula indisponibilidade em regiões inteiras da AWS (ex.: Europa, América do Norte, África, etc.).

**Macaco de Latência**:
	Causa atrasos ou paralisações artificiais; simula a degradação de serviço para verificar se serviços dependentes respondem de forma adequada.

**Macaco Janitor**:
	Procura recursos não utilizados e os desativa.

**Macaco de Conformidade**:
	Localiza e desliga instâncias AWS que não seguem as melhores práticas (ex.: falta de e-mail para alerta).

**Macaco de Segurança**:
	É uma extensão do Macaco de Conformidade para vulnerabilidades.

**Macaco Doutor**:
	Verifica a integridade de cada instância; desliga instâncias não íntegras quando o responsável não resolve a causa-raiz no tempo combinado, por exemplo.

Aumentar a resiliência e o entendimento de que não somos infalíveis e sempre teremos alguma falha e/ou algo a melhorar nos torna mais cautelosos e tolerantes conosco e com os times envolvidos. Isso nos permite focar mais a identificação das causas-raízes e soluções definitivas para os problemas. A resiliência, ou antifragilidade, é o segredo para o aprendizado.

#### Aprendizado com Falhas - Exército Símio

![[Pasted image 20240807150953.png]]
![[Pasted image 20240807151011.png]]
![[Pasted image 20240807151036.png]]
![[Pasted image 20240807151226.png]]
![[Pasted image 20240807151443.png]]

#### Reunião _post-mortem_ livre de culpa

É uma reunião que deve focar o problema, ou seja, o foco não está em descobrir quem fez ou contribuiu, mas no aprendizado constante da equipe e na melhoria dos processos: desde o início da demanda até a descontinuidade do produto, envolvendo todas as áreas da empresa (desenvolvimento, operação, negócio, etc.).

![[Pasted image 20240807152614.png]]
![[Pasted image 20240807152743.png]]
![[Pasted image 20240807152754.png]]
![[Pasted image 20240807152925.png]]
![[Pasted image 20240807153024.png]]
![[Pasted image 20240807153206.png]]
![[Pasted image 20240807153252.png]]

### Dias de jogos

Foram popularizados por Jesse Robbins na Amazon, para garantir a disponibilidade do _site_. Ele ficou conhecido como o “mestre do desastre” e defende que “um serviço não está realmente testado até o estragarmos em produção”.

Dias de Jogos não é só um momento de aprendizado, mas de testar nossa resiliência nos tornando uma organização antifrágil. Conhecer e aprender a resolver nossas vulnerabilidades (antes do cliente) é essencial para que possamos ser cada vez mais proativos e ter produtos com maior qualidade.

#### Aprendizado com Falhas - Dias de Jogos

![[Pasted image 20240807153840.png]]
![[Pasted image 20240807153949.png]]
![[Pasted image 20240807154145.png]]
![[Pasted image 20240807154206.png]]
![[Pasted image 20240807154250.png]]
![[Pasted image 20240807154419.png]]
![[Pasted image 20240807154429.png]]
![[Pasted image 20240807154616.png]]
![[Pasted image 20240807154647.png]]

#### Descobertas

Como divulgar e compartilhar aprendizados (descobertas) entre os times, então?

O livro _Jornada DevOps_ (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019) descreve algumas ações importantes de transformação de melhorias locais em globais. São elas:

##### _Chat_
As conversas com o time são registradas de forma dinâmica, com a colaboração de todos. Além disso, algumas operações no sistema, como o _deploy_, podem ser automatizadas via _chatbots_. Um simples comando pode subir um código em produção, por exemplo.

##### Automatizar atividades em _software_
Em vez de utilizar documentos estáticos, que normalmente não são atualizados, é melhor realizar a documentação no próprio código ou pela IDE. Os engenheiros da General Eletrics, por exemplo, criaram o conceito de ArchOps, em que os diagramas são automatizados e atualizados dinamicamente. Assim, qualquer pessoa do time pode ter uma visão clara das decisões arquiteturais.

##### Código-fonte e configurações em um repositório único
Mesmo usando microsserviços, em que os repositórios são separados, a ideia, aqui, é que todos tenham acesso a todo o código (mesmo que estejam em repositórios diferentes). É importante que todos compreendam o todo (produto completo), e não apenas uma parte específica. Tanto o código-fonte como as configurações de infra devem estar nesse repositório, com os padrões de testes e segurança e as configurações da _pipeline_ de implantação e integração contínua utilizada. Padrões de codificação e tutoriais também podem estar no repositório ou em uma _wiki_, que normalmente é versionada.

##### Testes automatizados como documentação
Quando são criados testes automatizados, documentam-se exemplos (regras de negócios) de como a aplicação deve funcionar (uma fonte rica das entradas e saídas possíveis de cada ponto de comunicação do _software_). A participação de um especialista em qualidade potencializa a completa cobertura e priorização dos testes automatizados.

#### Comunidade de prática (CoP) ou comunidade de excelência (CoE)

As comunidades de prática se resumem às pessoas que se reúnem para discutir o comportamento do sistema/tecnologia/processos e que definem, de fato, esse comportamento, usando ferramentas de discussão/bate-papo e _wikis_ para documentar as principais decisões.

##### Codificar registro não funcional de Ops
Criar mecanismos de monitoramento de requisitos não funcionais dentro do próprio código serve como um tipo de “estetoscópio” da aplicação. Assim como o cardiologista usa aparelhos de medição para estudar a frequência cardíaca, o _software_ deve ter aparelhos de medição do time de operações dentro do código-fonte para monitorar a “saúde” da aplicação. Para isso, utilizam-se requisitos não funcionais (NFR) (codificados) para projetar as operações, como: telemetria completa de produção (verifica, por meio de métricas, se o sistema está se comportando conforme o esperado); capacidade de monitorar dependências (verifica se os serviços que fornecem dados ao sistema estão operacionais, funcionando na capacidade adequada); serviços resilientes que se degradam quando necessário (serviços que podem ser degradados de uma forma planejada, para que a aplicação não caia devido a uma carga excessiva no sistema); e compatibilidade com todas as versões (verifica se o sistema é compatível com outros sistemas a que está integrado). Geralmente, aqui são implementados testes de contrato.

##### Histórias de usuários de Ops usadas em Dev
Para tudo que o time de operação realizar no dia a dia, é necessário criar histórias para “ensaiar” as ações com o time de desenvolvimento. Assim, mantém-se o time todo preparado para imprevistos e trabalhando em conjunto.

##### Escolhas de tecnologia alinhada aos objetivos de negócio
Cada tecnologia tem características/objetivos que influenciam tanto o esforço de aprendizado quanto o próprio desenvolvimento da aplicação e do ambiente para seu uso. Um exemplo disso, segundo o livro _Jornada DevOps_ (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019), são as tecnologias assíncronas, que enviam um _request_ e não têm previsão de retorno da resposta ao sistema quando utilizados os conceitos de _jobs_ e filas. É interessante alinhar esse tipo de estratégia ao negócio, para que se tenha transparência ao usuário final, por exemplo.

##### _Workflows_ e/ou _scripts_ automatizados
Transformar processos que estão documentados em _workflows_ e/ou _scripts_ automatizados é outra forma de transformar um conhecimento local em organizacional, garantindo que o processo seja usado e reutilizado, fornecendo valor agregado para todos os usuários.

##### Testes de _software_
Segundo o livro _Jornada DevOps_ (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019), Gojko Adzic (2011), no livro _Specification by example_, diz que os testes de _software_ servem como uma documentação viva de como o _software_ precisa se comportar. Pelo fato de ser executável, esse tipo de documentação nunca fica desatualizado (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019). Martin Fowler, no artigo “_Specification by example_”, descreve a importância da especificação como documentação útil no desenvolvimento de _software_, além de ser uma forma de estimular a cultura de testes automatizados de ponta a ponta nos times.

### Segurança da informação e gestão de mudanças

O objetivo da segurança (DevSecOps) no DevOps é que a equipe de segurança participe ativamente desde o início do ciclo de desenvolvimento, com foco na automatização dos controles, exercitando a conformidade por demonstração. Dessa forma, evitam-se gargalos de segurança ao final do ciclo de desenvolvimento não autorizando mudanças por problemas no ambiente de produção, que poderiam ter sido alinhados desde o início do desenvolvimento da aplicação.

A imagem a seguir sugere algumas ações que devem ser tomadas ao longo do ciclo:

![[stb07 4.png]]

Conheça algumas dicas do livro _Jornada DevOps_ (MUNIZ; SANTOS; IRIGOYEN; MOUTINHO, 2019) para garantir a segurança ao longo do ciclo de desenvolvimento, implantação e operação do produto:  

1. Teste de código.

2. Revisão de código.

3. Teste de penetração.

4. Servidores de IC como código.

5. Análise estática considerando critérios específicos de segurança, garantindo a remoção de erros antes mesmo da execução do _build_ (Sonar, Veracode, Gauntlet e manual).

6. Evitar que usuários sem autorização acessem o ambiente:
	● Controle das configurações de ambiente.
	● Teste de ataques de injeção de SQL.
	● Uso de credenciais de IC somente leitura.
	● Uso de VM isoladas.

7. Uso de telemetria em ambiente para detectar possíveis falhas:
	● Alterações de componentes e infraestrutura na nuvem.
	● Alterações em configurações diversas (Puppet, Chef, etc.).
	● Alteração de usuários nos grupos privilegiados de _admin_ e InfoSec.
	● Erros _http_ no servidor _web_, como 4xx e 5xx (exs.: 401 – Não autorizado;  
	403 – Permissão negada; 502 – _Bad gateway_).
	● Abertura e fechamento de portas.

8. Uso do Sonar para garantir a segurança. (O Sonar é uma ferramenta de análise de código estática que detecta vulnerabilidades, _code smells_ e cobertura de testes automatizados.)


**_OWASP_**
O OWASP (Open Web Application Security Project) é um projeto aberto de segurança em aplicações _web_ que disponibiliza, gratuitamente, vários artefatos de segurança para aplicações _web_ (artigos, metodologias, documentação e ferramentas). Conheça o projeto [aqui](https://owasp.org/).

Vamos conhecer as 10 principais vulnerabilidades que o Sonar verifica, de acordo com o OWASP:

1. Quebra de controle de acesso.

2. Falhas criptográficas.

3. Injeção.
	a. _Cross-site scripting_ (_script_ entre _sites_) – faz parte dessa categoria na edição de 2021.

4. _Design_ inseguro.

5. Configuração insegura.

6. Componentes desatualizados e vulneráveis.

7. Quebra de identificação e autenticação.

8. Falhas de _software_ e de integridade de dados.

9. Falhas de registro e monitoramento de segurança.

10. Falsificação de solicitação do lado do servidor.

#### DevSecOps

O que é Segurança da Informação? Muitos entendem que a segurança já está contida na sigla DevOps e que não seria necessário destacá-la e formar mais um acrônimo. No entanto, se o time, de alguma forma, entende que é importante fazer isso para promover a cultura, então, vale a pena fazer o destaque. O que é Segurança da Informação e LGPD e o que precisamos saber?

![[Pasted image 20240807160312.png]]
![[Pasted image 20240807160529.png]]
![[Pasted image 20240807160814.png]]
![[Pasted image 20240807161249.png]]
![[Pasted image 20240807161257.png]]
![[Pasted image 20240807161415.png]]

Nós que participamos do Ciclo de Vida do desenvolvimento precisamos conhecer cada vez mais o tema 'segurança' para garantir que estas práticas sejam executadas sempre o mais próximo do início do ciclo de vida. Quanto mais internalizarmos o conceito de ciclo de vida seguro, menos seremos barrados em uma gestão de mudanças ou em vulnerabilidades.

#### DevSecOps - Ciclo de Vida Segura

Quais as boas práticas de SI que devemos nos preocupar ao longo do ciclo de desenvolvimento para que não tenhamos o gargalo de segurança no final do ciclo?

![[Pasted image 20240807161520.png]]
![[Pasted image 20240807162101.png]]
![[Pasted image 20240807162000.png]]

Nada melhor do que conhecer casos práticos relacionados ao tema Segurança para internalizar alguns conceitos importantes.

#### DevSecOps - Segurança na Prática

![[Pasted image 20240807162550.png]]
![[Pasted image 20240807162723.png]]
![[Pasted image 20240807162950.png]]
![[Pasted image 20240807163003.png]]
![[Pasted image 20240807163029.png]]

### Gestão de mudanças

Normalmente, nas empresas, temos os seguintes tipos de mudança:  

- Padrão: baixo risco e pré-aprovada.
- Normal: risco alto e passa pela aprovação de comitê.
- Urgente: risco alto para resolver incidentes críticos em produção e exigência de aprovação da alta direção.

A utilização de práticas DevOps, como uma _pipeline_ de implementação adequada, permite que a grande maioria das mudanças seja classificada como de baixo risco. 

A utilização do DevSecOps tem como objetivo a simplificação da gestão de mudanças.

![[Pasted image 20240807163205.png]]
![[Pasted image 20240807163225.png]]
![[Pasted image 20240807163247.png]]
![[Pasted image 20240807163306.png]]
![[Pasted image 20240807163324.png]]
![[Pasted image 20240807163340.png]]

Pelo que pudemos observar, as evidências (cobradas pelas equipes de governança e auditoria) de uma boa gestão de mudanças não precisam estar em documentos ou formulários extensos. A automação pode e deve ser uma fonte de evidências mais completas, íntegras e confiáveis.

### Referências:

DWECK, C. S. **Mindset**: the new psychology of success. London: Robinson, 2017.

EDMONDSON, A. C. Strategies for learning from failure. **Harvard Business Review**, v. 89, n. 4, p. 48-55, 2011.

EDMONDSON, A. C. The competitive imperative of learning. **Harvard Business Review**, v. 86, n. 7-8, p. 60-67, 2008.

FOWLER, Martin. **Specification by Example**. 2004. Disponível em: [https://martinfowler.com/bliki/SpecificationByExample.html](https://martinfowler.com/bliki/SpecificationByExample.html). Acesso em: 15 mai. 2023.

KIM, G.; DEBOIS, P.; WILLIS, J.; HUMBLE, J. **The DevOps handbook**: how to create world-class agility, reliability, and security in technology organizations. Portland: IT Revolution Press, 2016.

MUNIZ, A.; IRIGOYEN, A. **Jornada ágil e digital**. Rio de Janeiro: Brasport, 2019.

MUNIZ, A.; IRIGOYEN, A.; GAMA, F.; CARRASCO, J.; COSTA, M.; ENOMOTO, N.; IRIGOYEN, R. **Jornada Azure DevOps**. Rio de Janeiro: Brasport, 2022.

MUNIZ, A.; SANTOS, R.; IRIGOYEN, A.; MOUTINHO, R. **Jornada DevOps**. Rio de Janeiro: Brasport, 2019.

PRESSMAN, R. S. **Engenharia de** **_software_**. 5. ed. Rio de Janeiro: McGraw-Hill, 2011.