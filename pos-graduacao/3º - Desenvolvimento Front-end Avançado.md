# Design e Prototipação da Interface do Usuário (Disciplina 1)

##  Design da Usabilidade de Interface (Aula 1)

### Conceitos básicos

#### Ergonomia: _ergon_ (trabalho) + _nomos_ (normas)

Nesta seção, você vai aprender a importância do _design_ para ajudar as pessoas a realizarem seu trabalho, com foco no uso de _websites_ e aplicativos. Para ajudá-lo a compreender essa importância, serão apresentadas as ciências ergonomia e interação humano-computador, bem como sua relação com o _design_. Esse conhecimento é básico e fundamental para este início, pois, para projetar um artefato digital interativo, é preciso compreender como ele pode ajudar nas tarefas do usuário e quais são as consequências de um projeto mal realizado para o bem-estar deste.  

Chapanis (1996) explica que a ergonomia é um corpo de conhecimentos sobre as habilidades, limitações e outras características humanas relevantes para o _design_. Essas práticas são fundamentais para o _design_ de ferramentas, sistemas, tarefas e contextos de uso humano. A ergonomia sempre objetiva o uso humano seguro, confortável e efetivo.

A seguir, explicaremos a interação homem-computador, o desdobramento da ergonomia fundamental para o entendimento da atividade de _design_ na experiência do usuário (UX) e a interface do sistema com o usuário (UI).

#### IHC: interação homem-computador

A aplicação da ergonomia em projetos de sistemas computacionais gera um debate sobre a interação humano-computador (IHC), área que estuda a interação entre homens e computadores. Uma interação é uma relação entre duas ou mais entidades em que cada ação de uma parte corresponde a uma reação das demais.  

A interação humano-computador ocorre por meio da interface com o usuário, formada pelo sistema computacional, composto por _hardware_ e _software_.

![[stb01 3.png]]

Como pode ser visto na figura, o usuário tem um objetivo em mente ao iniciar o acesso a um sistema computacional. Ele interage com o sistema para alcançar determinado objetivo realizando ações, e o sistema fornece como reação um _feedback_. O contexto de uso, que inclui o ambiente físico social e cultural, interfere nessa interação.
A interação e a interface devem ser adequadas para que o usuário aproveite ao máximo o apoio do sistema computacional à realização de suas tarefas.  

**O sistema deve mostrar ao usuário, de forma clara, quais ações são possíveis e como realizá-las. Além disso, seu _feedback_ deve ser claro, para que o usuário possa compreendê-lo e dar continuidade à interação.**  

Esses objetivos são alcançados no _design_ do sistema ou aplicativo quando são atendidos critérios de qualidade de uso, como: **usabilidade, experiência do usuário, acessibilidade e responsividade**. A figura a seguir apresenta em detalhes esses critérios.

![[Pasted image 20241014163924.png]]

Todos esses critérios estão relacionados com a ergonomia, pois influenciam a realização do trabalho, e serão abordados em detalhes nesta aula.  

Considere a declaração de Alan Dix, autor, pesquisador e professor universitário britânico, especializado em interação humano-computador. Ele é um dos quatro coautores do livro didático de nível universitário _Human-computer interaction_, além de diretor da Fundação Computacional da Swansea University, desde maio de 2018.

> _A interação humano-computador envolve o design, implementação e avaliação de sistemas interativos no contexto da tarefa e trabalho do usuário.”_
(DIX; FINLAY; ABOWD, 2004, p. 4, tradução nossa.)

É importante ressaltar, considerando a declaração de Dix, que a atividade de projeto e implementação de protótipo do artefato (_desktop ou mobile_), em estágios iniciais do projeto, em que conceitos e valores podem ser verificados, é fundamental para seu sucesso.  

Também se considera que **observar o contexto em que o usuário se encontra** e os objetivos fáticos que busca em seu trabalho **são condições _sine qua non_ para o projeto correto**, pela verificação de outras variantes, como: estímulos, ruídos, tempo, _workflow_, etc.

### Usabilidade de interface

Primeiramente, para compreender a usabilidade de interface (UI), é importante entender a diferença entre _user experience_ (UX) e a própria UI.  

A experiência do usuário é frequentemente definida como a sequência de interações entre um usuário e um sistema projetado para atender satisfatoriamente a suas necessidades e metas. O termo é conhecido pela sigla inglesa UX, abreviação de _user experience_.

![[01 9.png]]

![[02 10.png]]

![[03 10.png]]

Assim, a ISO 9241-11 (2002) explica como identificar a informação necessária a ser considerada na especificação ou avaliação de usabilidade de um computador em termos de medidas de desempenho e satisfação do usuário. É dada orientação sobre como descrever explicitamente o contexto de uso do produto (_hardware_, _software_ ou serviços) e as medidas relevantes de usabilidade. A orientação é dada na forma de princípios e técnicas gerais.  

A partir disso, explicam-se os principais conceitos:  

- Eficácia: capacidade de executar uma tarefa de forma correta e completa.

- Eficiência: recursos gastos para conseguir ter eficácia, sejam eles tempo, dinheiro, produtividade ou memória.

- Satisfação: conforto na execução da tarefa.

Dessa forma, **precisamos de interfaces alinhadas às expectativas dos usuários** e que permitam interagir com os dispositivos de forma intuitiva e com fácil aprendizado. Nesse sentido, é muito importante **conhecer o modelo mental do usuário**. Qualquer pessoa com qualquer nível de experiência com tecnologias digitais pode acessar um _website_ ou aplicativo _mobile_ atualmente. Assim, tanto a identidade visual como a arquitetura da informação precisam ser planejadas com cuidado e testadas previamente.  

Hoje, as pessoas esperam muito dos _websites_ e cada vez menos aceitam um projeto ruim. Assim, equívocos em usabilidade resultam em clientes insatisfeitos e perda de negócios. Jakob Nielsen, um dos precursores da Usabilidade na _web_, ainda na década de 1990, trata disso em seu livro _Usabilidade na web_. 

![[02 1 2.png]]

![[03 1 2.png]]

![[04 7.png]]

![[05 5.png]]

![[06 2.png]]

Assim, conclui-se que UX e UI são componentes essenciais no projeto de _software_. Na próxima seção, será explicado o plano projetual de Garrett (2003) e em que etapa entram as distinções de UX e UI do _software_ que se deseja construir.

### Os cinco planos de projeto de Garrett

Como pode ser visto no diagrama a seguir, Garrett explica os cinco planos – **estratégia, escopo, estrutura, esqueleto e superfície** – como uma estrutura conceitual para falar sobre os problemas de experiência do usuário e as ferramentas que usamos para resolvê-los.

![[imagem_teste.png]]

No plano mais baixo, não estamos preocupados com a forma final do _site_, produto ou serviço – apenas em como o _site_ se encaixará em nossa estratégia (enquanto atende às necessidades de nossos usuários). No plano mais alto, só nos preocupamos com os detalhes mais concretos da aparência do produto. Plano a plano, as decisões que temos de tomar tornam-se um pouco mais específicas e envolvem níveis mais sutis de detalhes.

Cada plano depende daqueles que estão abaixo dele. Então, a superfície depende do esqueleto, que depende da estrutura, que depende do escopo, que depende da estratégia. Considera-se que a UX compreende as etapas de estratégia, escopo e estrutura do _software_. Ou seja, o bom planejamento, a inteligência de negócio, as necessidades do usuário e a visão macro do produto (_design_ da interação e arquitetura da informação). O esqueleto, representado pelo _wireframe_, está na posição intermediária entre o UX e o UI, fazendo a ponte para a superfície ou _design_ visual. Nesse plano mais concreto, todas as etapas anteriores são materializadas em protótipos visuais fiéis ao produto final.  

Com o _design_ maduro e interativo, podemos começar a considerar questões de estrutura visual da tela e de navegação. Na próxima seção, entraremos em detalhe nesses tópicos.

### Navegação na _web_

Steve Krug, em seu famoso livro _Não me faça pensar_ (2006), já no título deixa claro o desejo de todos nós ao acessarmos um _website_: **não queremos perder tempo com dúvidas**, pensando no que devemos fazer, para onde ir ou onde estamos. Queremos rapidamente resolver nosso problema, seja ele comprar um produto ou contratar um serviço, obter maiores informações sobre um evento, descobrir o endereço e telefone de um restaurante, etc. Isso sem erros e dúvidas, como itens confusos no menu, dúvidas de como preencher um formulário (“Coloco ponto ou hífen?”; “Com o CEP, ele buscará minha rua?”), entre tantas outras questões que nos deixam confusos e, consequentemente, frustrados ao interagirmos com uma interface mal projetada.  
  
Krug também declara:

> “_Usuários não leem sua página... Escaneiam!_”
(KRUG, 2015, p. 9.)

No infográfico a seguir, descrevem-se as perguntas fundamentais que devem ser feitas para escrutinar uma UI.

![[stb06 1 1.png]]

Na _web_, temos que seguir a intuição, por meio da navegação, de acordo com os rótulos, títulos e menus disponibilizados. Uma boa UI deve responder três perguntas básicas: “Onde estou?”, “De onde vim?” e “Para onde posso ir?”.

![[stb07 1 1.png]]

Consideradas as questões de estrutura dos elementos na tela e as oportunidades de interação que eles trazem, podemos iniciar a discussão sobre as diferenças das mídias _desktop_ e _mobile_.

### Diferenças no _design_ da interface _desktop_ e _mobile_

Compreender as características específicas do _design_ para aplicativos é fundamental para guiar seus projetos. Uma dessas características é que a experiência em dispositivos móveis (_mobile_), em que os aplicativos são implementados, é muito diferente daquela em computadores de mesa (_desktop_).  

Assim, acompanhe o infográfico a seguir:

![[stb08 4.png]]

Na experiência com _desktop_, há muito menos variações, pois o computador normalmente é utilizado no mesmo ambiente, com características constantes (como iluminação e privacidade), geralmente próximo de pessoas conhecidas e com maior controle sobre o tempo de uso. O próprio ambiente de uso do computador _desktop_, seja em casa, no escritório ou em uma _lan house_, é projetado para esse uso. Portanto, a experiência com _desktop_ não pode ser copiada para a experiência com _mobile_.  

A seguir, você verá alguns exemplos comparativos das diferenças básicas no _design_ das interfaces _desktop_ e _mobile_ para entender que nunca é adequado copiar a página _web_ para a versão _mobile_.

![[Pasted image 20241014174708.png]]

![[Pasted image 20241014174736.png]]

- O _scroll_ horizontal da página é péssimo UX! (Funciona para categorias e menus contextuais.)
- Minimizar tudo, para caber, também não é a solução.

![[Pasted image 20241014174837.png]]

![[Pasted image 20241014174855.png]]

- Os controles devem facilitar o toque e não imitar o mundo real (como se faz tradicionalmente no _desktop_).
- Atenção aos padrões de componentes (principalmente _mobile_).

![[Pasted image 20241014174959.png]]

![[Pasted image 20241014175028.png]]

- Organização.
- Simetria.
- Alinhamento.
- Atenção aos padrões de componentes (principalmente _mobile_).

![[Pasted image 20241014175125.png]]

![[Pasted image 20241014175234.png]]

Outros exemplos que discutiremos na aula expositiva (considerados diferentes dispositivos): prioridade de conteúdo; _breadcrumbs_ (navegação estrutural) _versus_ navegação contextual/global; e indicador de progresso (_desktop_) x ausência (_web app_ e aplicativo).

#### _Design_ da usabilidade de interface

![[Pasted image 20241014181741.png]]

![[Pasted image 20241014181826.png]]
![[Pasted image 20241014181848.png]]
![[Pasted image 20241014181902.png]]
![[Pasted image 20241014181918.png]]
![[Pasted image 20241014181930.png]]
![[Pasted image 20241014181944.png]]
![[Pasted image 20241014181956.png]]
![[Pasted image 20241014182008.png]]
![[Pasted image 20241014182022.png]]

![[Pasted image 20241014182047.png]]

![[Pasted image 20241014182057.png]]

![[Pasted image 20241014182115.png]]

![[Pasted image 20241014182128.png]]

![[Pasted image 20241014182143.png]]

![[Pasted image 20241014182151.png]]

![[Pasted image 20241014182205.png]]

Após esse comparativo entre diferentes dispositivos e o impacto de diversos formatos no _design_ do _software_, podemos seguir para a próxima seção.

### _Design_ responsivo e adaptativo

Nesta seção, descreveremos as diferenças entre o _design_ de aplicativos nativos (instalados em diferentes sistemas operacionais, como Android, Apple iOS e Windows Phone) e _websites_ responsivos e adaptativos. A imagem a seguir mostra os desdobramentos entre aplicativos nativos e adaptados.

![[stb13 5.png]]

Já a imagem a seguir apresenta um comparativo entre aplicativos nativos (iOS, Android e Windows Phone) _versus_ aplicativos _web_ (_web apps_), que são basicamente HTML responsivo e adaptativo.

![[stb14 2.png]]

Se você optar por um _website_ adaptado, em vez de um aplicativo nativo, precisará adaptá-lo para ser usado em diferentes dispositivos móveis com tamanhos e resoluções de tela distintos. Esse problema foi resolvido com o _design_ responsivo, uma técnica que possibilita mudar o tamanho do _layout_ do _website_ e de seus elementos de acordo com o dispositivo e sua resolução. Para isso, basta o uso de HTML e de alguns padrões na CSS (_cascading style sheets_), que é um guia de estilos que formaliza o documento web com definição de cores, fontes, espaçamento, etc.

A figura à baixo mostra o mesmo _site_, adaptado para ser visto em diferentes dispositivos.

![[img1.jpg]]

Dessa forma, é possível analisar que o _design_ responsivo apresenta as seguintes vantagens e desvantagens:

![[01 1 3.png]]

![[pos-graduacao/Acervo de Imagens/02 2 1.png]]

Uma alternativa semelhante ao _design_ responsivo é o _design_ adaptativo, pois com ambos o _website_ se torna acessível em diferentes resoluções, adaptando-se à tela. A diferença é que o adaptativo utiliza uma medida fixa na largura do _layout_ e de seus elementos para cada resolução, enquanto o responsivo é mais flexível, com a largura definida em porcentagem, variando em cada intervalo de um ponto de quebra.

A figura à baixo mostra as instruções de programação para a apresentação de diferentes interfaces. A largura mínima e máxima em _pixels_ (px) define a interface que deve ser apresentada no navegador do usuário (p. ex., “max-width: 1200px” apresenta um “_large desktop_”).

![[stb16 2.png]]

Com essa flexibilidade, a tela parece estar sempre preenchida. Já no _design_ adaptativo, com as medidas fixas, o _designer_ tem um controle maior sobre a aparência do _layout_.

Na figura à baixo, é possível notar que, embora semelhantes, há diferenças entre os designs responsivo e adaptativo: enquanto o responsivo se adequa automaticamente e em porcentagem, conforme a largura da tela, o adaptativo apresenta design próprio, conforme o formato da tela. Para conhecer mais sobre os princípios do design responsivo, [clique aqui](https://blog.froont.com/9-basic-principles-of-responsive-web-design/).

![[stb17 2.png]]

Na próxima seção, explicamos as regras de colunagem para organização estrutural dos componentes visuais e funcionalidades da página. Essas definições são fundamentais para o bom projeto de _design_ e para os aspectos responsivos e adaptativos dos conteúdos apresentados em diferentes dispositivos _mobile_ e _desktop_.

### Colunagem

Colunagem são malhas que dividem a tela em partes proporcionais para facilitar a organização do _layout_ e o posicionamento de seus elementos. O _layout_ responsivo utiliza um _grid_ fluido com porcentagens. Durante anos, o _grid_ mais utilizado tinha 960 px de largura, pois a resolução mais utilizada era de 1024 x 768 px. Atualmente, o mais comum é usar a largura de 1200 px, ou mais, para adaptar o _grid_ às resoluções maiores de monitores.

Na figura à baixo, é possível verificar um _grid_ de 12 colunas para _layouts_ responsivos.

![[stb18 1.png]]

#### Resoluções

Um dos muitos questionamentos que surgem quando se está trabalhando com _design_ interativo é por que se devem utilizar 1200 px para a área segura. Isso ocorre porque todos os monitores modernos (principalmente _widescreen_) suportam, pelo menos, 1280 x 1024 px de resolução. Em janeiro de 2010, 76% dos computadores usavam uma resolução superior a 1024 x 768 px. Além disso, 1200 é divisível por 2, 3, 4, 5, 6, 8, 10, 12, 15, 16, 20, 24, 30, 40, 48, 60, 80, 120, 150, 200, 240 e 400. Isso faz com que seja um número-base altamente flexível para trabalhar.

A tabela à baixo apresenta a tabela atualizada com as resoluções de tela mais comuns usadas mundialmente. Para conhecer mais sobre as resoluções de tela mais comuns [clique aqui](https://www.w3schools.com/browsers/browsers_display.asp).

![[stb19 1.png]]

Podemos verificar na tabela que as resoluções mais comuns são 1366 x 768 e 1920 x 1080. Já a tabela a seguir apresenta as faixas de largura em _pixels_ e o tipo de janela correspondente a dispositivos, que vão de “_extra-small_” (celulares) a “_small_” (_tablets_), “_medium_” (_laptops_) e “_large_” (computadores _desktop_ e TVs de grandes dimensões). Mostra, também, a recomendação da quantidade de colunas para cada dispositivo e a largura adequada do intervalo entre colunas.

![[stb20 1.png]]

A tela _desktop_ é dividida em colunas, sendo 12 colunas o formato mais utilizado, pois divide o _layout_ de forma uniforme, já que 12 é um número divisível por 2, 3 e 4. Contudo, a quantidade de colunas pode variar de acordo com o projeto. Em _tablets_, costumam-se usar 8 colunas e, em _smartphones_, de 6 a 4 colunas. Observe na imagem a seguir:

![[stb21 1.png]]

Você pode utilizar o _grid_ como uma camada do Adobe XD, Figma ou outro _software_ especializado. Ou seja, pode usar um _grid_ já pronto ou fazer um. Pode, também, usar um _layout_ fluido, como porcentagens, ou incluir pontos de quebra (_breakpoints_). Veja, nas imagens a seguir, exemplos de colunagem com diferentes pontos de quebra.

![[Pasted image 20241014222652.png]]

![[Pasted image 20241014222716.png]]

### _Smartphones_

Assim como no _design_ de aplicativos nativos, para o _layout_ responsivo de _smartphones_, que têm telas com dimensões reduzidas e trabalham com resoluções de 320 ou 480 px e cerca de 4 a 6 colunas, você deve seguir estas dicas:  

- Priorizar os principais conteúdos e funcionalidades.
- Itens de menu que são visíveis em resoluções maiores podem ficar ocultos, acessíveis pelo clique no ícone de menu ou arrastando a tela, ou dispostos em uma lista vertical, dependendo da quantidade de itens.
- Imagens e textos podem ter seu tamanho reduzido, cuidando para que a área de toque fique dentro do tamanho adequado e a leitura não seja prejudicada.
- Alguns conteúdos ou funcionalidades menos prioritários podem ficar ocultos, sem acesso nessas resoluções.
- Conteúdos dispostos lado a lado em colunas em outras resoluções podem ficar um abaixo do outro em uma coluna única nessas resoluções.

### _Tablets_

Os _tablets_ têm telas maiores do que os _smartphones_ e menores do que os computadores _desktop_, com resoluções de 768 ou 960 px e cerca de 8 colunas. São diferentes dos _smartphones_ em relação à experiência, e essas diferenças impactam as decisões sobre o _design_ e o conteúdo a ser mostrado em cada dispositivo:  
  
- _Smartphones_ são relacionados a um indivíduo, enquanto _tablets_ podem ser usados por um grupo.
- _Smartphones_ são carregados e usados em qualquer local, seja em casa, na rua ou no trabalho. _Tablets_ são muito mais usados em casa, hotéis e situações em que o usuário está descansando.
- A frequência de uso é consideravelmente menor nos _tablets_. Por outro lado, os usuários ficam mais tempo em cada uso do _tablet_ do que nos _smartphones_.
- _Smartphones_ são muito usados para comunicação, enquanto _tablets_ são usados mais para consumo de conteúdo.
- Tarefas como preenchimento de cadastros, realização de buscas, exibição de vídeos ou filmes são melhor realizadas em _tablets_, devido ao tamanho maior da tela.
- Itens de menu que podem ficar ocultos em _smartphones_ podem ser exibidos no _tablet_, principalmente na orientação paisagem, seja em menus horizontais ou em colunas à direita ou à esquerda da coluna central que contém o principal conteúdo.
- O conteúdo pode ser dividido em mais colunas e ser visível em boa parte sem precisar rolar a tela.

### _Desktops_

Aqui, já há uma mudança significativa tanto na experiência do usuário quanto no design. Computadores _desktop_ utilizam resoluções acima de 1140 px e cerca de 12 colunas no _grid_. Todas as colunas são exibidas, incluindo menus laterais e itens dos menus horizontais. Quanto maior o uso de colunas, maior a possibilidade de usar trechos do conteúdo dispostos lado a lado, aproveitando a maior largura da tela e reduzindo a rolagem. Tanto em _tablets_ quanto em _desktops_, é preciso ocupar ao máximo a largura da tela, evitando deixar espaços em branco e, ao mesmo tempo, blocos de texto com larguras excessivas que dificultem a leitura.

Na figura à baixo, é possível verificar a área segura de 1200 px dentro da resolução de 1366 x 768 px.

![[stb23.gif]]

A seguir, descrevemos as resoluções de imagem adequadas para exibição em telas de dispositivos _desktop_ e _mobile_.

### Qualidade da imagem: resolução em PPI (_pixel per inch_)

Nesta seção, faremos um breve resumo de um aspecto importante das imagens inseridas em uma UI de alta definição: a resolução em polegadas, ou PPI.  

A resolução de uma imagem é o número de _pixels_ por polegada que ela contém (1 polegada é o equivalente a 2,54 centímetros). É expressa em PPI (_pixels per inch_, ou pontos por polegada) ou DPI (_dots per inch_).  

PPI ou DPI são a descrição da densidade de _pixels_ de uma tela de monitor. Uma densidade maior de _pixels_ significará que há mais _pixels_ em cada polegada quadrada de sua tela.

Como é possível observar na figura à baixo, a densidade de _pixels_ deve ser maior em dispositivos com resolução mais alta.

![[stb24 1.png]]

Quanto mais _pixels_ (ou pontos) por polegada, mais informações haverá na imagem (mais precisa). Por exemplo, uma resolução de 300 dpi significa que a imagem comporta 300 _pixels_ de largura e 300 _pixels_ de altura. É, então, composta por 90.000 _pixels_ (300 x 300 ppi). Graças a essa fórmula, é fácil conhecer a resolução da imagem.  

A resolução de 72 ppi consiste no menor padrão de resolução que existe e é considerada a ideal para imagens na _web_ e telas de computador, visto que não é preciso um alto número de _pixels_ para se obter uma boa resolução. Quando geramos arquivos para _desktop_, é comum usar essa resolução e formatos _bitmap_ (mapa de bits) de imagem, como .JPG e .PNG.  

Em UI para dispositivos _mobile_, também se usam esses formatos, mas atualmente se observa o popular formato de terminação .SVG, ou _scalable vector graphic_. Formatos vetoriais como esse podem ser reajustados para diferentes dimensões, sem perda de qualidade (pixelização).  

Como pode ser observado na imagem a seguir, _smartphones_ comportam cada vez mais pontos por polegada em suas telas, aproximando-se das resoluções de imagens impressas. Isso garante a qualidade de alta definição das imagens apresentadas na tela. Em outras palavras, cada vez mais _pixels_ por polegada são comportados.

Na tabela à baixo, é possível verificar alguns dispositivos mobile disponíveis no mercado, seus sistemas operacionais, dimensões e a quantidade de pixels por polegada (coluna na extremidade direita). Para ver mais detalhes sobre estas características presentes nos dispositivos, [clique aqui](https://screensiz.es/phone).

![[stb25 1.png]]

### _Grid_ e alinhamento

O alinhamento e o espaçamento entre os componentes de um _layout_ são feitos com o uso de um _grid_, uma estrutura-base composta por uma malha de quadrados que ajuda a ordená-los.

No _layout_ do [Material Design](https://m1.material.io/layout/metrics-keylines.html#metrics-keylines-baseline-grids), o _grid_ onde os componentes são alinhados tem quadrados com 8 dp em suas dimensões. Por isso, as dimensões utilizadas, como margens, larguras e alturas de componentes, são múltiplos de 8: 16, 24, 32, 40, 48, 56, 64, 72, etc.

![[stb26 1.png]]

Nota-se, na figura à baixo, a aplicação de colunagem e _grid_ no projeto de um _wireframe_, sendo 4 colunas e _grid_ de 8 px dentro de um dispositivo iPhone 14 Plus, 13 Pro Max, ou 12 pro Max (428 x 926 px).

![[img2.png]]

Já o _grid_ para alinhamento dos textos tem 4 dp em suas dimensões, [como orienta o Material Design](https://m1.material.io/layout/metrics-keylines.html#metrics-keylines-baseline-grids). Nesses casos, como nas alturas e margens de textos, cabem outras dimensões, que são múltiplos de 4: 8, 12, 16, 20, 24, 28, etc.

![[stb27 1.png]]

Note que, nos conceitos apresentados, foi utilizada a nomenclatura “dp”. Você sabe o que isso significa? A densidade de _pixels_ é um cálculo que retorna o número de _pixels_ físicos por polegada em uma tela de dispositivo. É, muitas vezes, referida como _pixels per inch_ ou PPI (explicado na seção anterior).

### _Wireframes_

O nome _wireframe_ vem da junção de duas palavras em inglês: _wire_ (linha) e _frames_ (telas).

Um _wireframe_ é um desenho básico, como um esqueleto, que demonstra de forma direta a arquitetura de como o objeto final (interface, página _web_, aplicativo _mobile_, etc.) será, conforme as necessidades dos usuários e os objetivos do _site_.  

Ele é elaborado para organizar os elementos que entrarão na composição do projeto final. Deve ser feito da maneira mais simples possível, mostrando apenas o essencial, como uma espécie de rascunho, sem cores ou imagens.  

O objetivo do _wireframe_ é auxiliar o desenvolvedor no entendimento dos requisitos que foram recolhidos junto ao cliente com relação às funções e objetos que um sistema deverá conter.  

A seguir, é possível verificar uma sequência de _wireframe_ de baixo detalhamento, _wireframe_ de alto detalhamento e o resultado do _wireframe_ no _layout_ final:

![[Pasted image 20241015121710.png]]

![[Pasted image 20241015121731.png]]

![[Pasted image 20241015121802.png]]

#### Diferença entre _sketches_ x _wireframe_ x _mockups_ x protótipos

Basicamente, a partir de uma ideia inicial, é desenvolvido um esboço (_sketch_) em papel. A partir desse esboço, é desenvolvido o _wireframe_, com uma ferramenta digital. Se for necessário e pertinente ao projeto, deve ser desenvolvida uma maquete (_mockup_), que é uma representação estática do artefato a ser produzido. Já no caso de um projeto _web_, deve ser desenvolvido um protótipo, para validação da navegação e usabilidade.  

Veja, a seguir, um resumo de cada um dos elementos, com base em referências específicas. Todos os _sites_ citados são de referência, e é importante que você os conheça.

![[Pasted image 20241015121957.png]]

![[Pasted image 20241015122106.png]]

![[Pasted image 20241015122346.png]]

![[Pasted image 20241015122624.png]]

![[Pasted image 20241015122738.png]]

Contudo, nem sempre é vantajoso produzir um _wireframe_. Acompanhe, no infográfico a seguir, as vantagens e os riscos do uso de _wireframes_ na ideação da tela.

![[stb30.png]]

As ferramentas digitais para construção de _wireframes_ existem para ajudar, seja na ideação e cocriação com _stakeholders_ (como Mural, Miro ou Balsamiq), seja em entregas mais formais (Figma, Adobe XD ou Invision). Entretanto, ferramentas têm limitações – estamos restritos às funcionalidades que oferecem –, e isso pode limitar a criação livre e ágil.

### Referências:

BARBOSA, S. D. J. et al. **Interação Humano-Computador e Experiência do Usuário.** [S.l.]: Edição da autora; 2021. E-book.  

BUXTON, B. **Sketching user experiences:** getting the design right and the right design. San Francisco: Morgan Kaufmann, 2007.  

CHUEKE, J. **Perceptible affordances and feedforward for gestural interfaces:** assessing effectiveness of gesture acquisition with unfamiliar interactions. British Library, 2016. Disponível em: [http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556.](http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556.) Acesso em: 3 nov. 2022.  

DIX, A.; FINLAY, J.; ABOWD, G. **Human-computer interaction.** 3. ed. New York: Parsons Education Ltd., 2004.  
  
GARRETT, J. **The elements of user experience:** user-centered design for the web. New York: New Riders, 2003.  
  
HOOBER, S.; BERKMAN, E. **Designing mobile interfaces:** patterns for interaction design. Sebastopol: O’Reilly Media, 2011.  
  
KORTUM, P. **HCI beyond the GUI**: design for haptic, speech, olfactory, and other nontraditional interfaces. Burlington, MA: Elsevier, 2008.  

KRUG, S. **Não me faça pensar!**: uma abordagem de bom senso à usabilidade mobile e na web. São Paulo: Market Press, 2015.  
  
LOPES, S. **A web mobile**: design responsivo e além para uma web adaptada ao mundo mobile. São Paulo: Casa do Código, 2014.  
  
MCELROY, K. **Prototyping for designers.** Sebastopol: O’Reilly, 2017.  

NIELSEN, J. **Usability engineering**. San Francisco: Morgan Kaufmann Publishers, 1994.  

NIELSEN, J.; LORANGER, L. **Usabilidade na web:** projetando websites com qualidade. Rio de Janeiro: Campus Elsevier, 2007.  

NORMAN, D. **The design of everyday things.** New York: Basic Books, 1988.  

ROGERS, Y.; SHARP, H.; PREECE, J. **Design de interação:** além da interação humano-computador. 3. ed. Porto Alegre: Bookman, 2013.  

STICKDORN, M. **This is service design doing:** applying service design thinking in the real world. Sebastopol: O’Reilly, 2018.  

TIDWELL, J. **Designing interfaces:** patterns for effective interaction design. Sebastopol: O’Reilly Media, 2010.  

WIGDOR, D.; WIXTON, D. **Brave NUI world:** designing natural user interfaces for touch and gesture. TH Köln, 2015.

## Prototipagem Aplicada I (Aula 2)

### Conceitos básicos

Vamos começar conhecendo os conceitos de _affordance_ e _feedback_, inerentes à _user interface_ e que visam a tornar a interface digital autoexplicativa e intuitiva para o usuário.

### _Affordance_

A _affordance_ pode ser utilizada para descrever:  

- a **identidade** de um objeto, ou seja, o que ele é; ou
- a **função** que determinado objeto realiza por meio da percepção de seus atributos.

O termo _affordance_ é um neologismo criado a partir do verbo em inglês afford, que pode ser traduzido como “habilitador”.  

O termo foi cunhado em 1966 pelo psicólogo James Gibson (1904-1979), que estudou, a partir da década de 1960, o sistema de percepção humano e o seu impacto nas nossas ações mais simples, mais intuitivas. O termo só foi plenamente solidificado em 1979 em seu livro _The Ecological Approach to Visual Perception_. Gibson explica _affordance_ como _uma situação na qual as características sensórias do objeto sugerem intuitivamente sua funcionalidade e uso. Ações são latentes no ambiente, mensuráveis e independentes da habilidade do indivíduo de reconhecê-las, mas sempre em relação ao ator, e, portanto, dependentes da sua capacidade._

Uma maçaneta em uma porta, por exemplo, indica que podemos girá-la para abrir a porta. Essa percepção é resultado da análise das propriedades da maçaneta, como altura relativa ao chão, proximidade ao nosso braço e forma que indica que pode ser girada.

No entanto, também podem ocorrer situações nas quais a mensagem transmitida é contraditória.

Se olharmos a imagem à baixo, de uma porta dupla de uma loja de conveniência de um posto de gasolina, podemos perceber que uma das portas oferece uma mensagem contraditória: o sinal explicitamente diz para empurrar para abrir a porta, mas o formato vertical da alça implicitamente diz para puxar para abrir a porta. Isso porque alças são para puxar, e barras horizontais, para empurrar.

![[Imagem1.png]]

Anos depois, o professor Don Norman adaptou o conceito para as interfaces digitais no livro O _design do dia a dia_ (1988), renomeando o termo para **_affordance_** **perceptível**:

> “A _affordance_ perceptível é uma propriedade desejável na interface usuário-programa que naturalmente guia as pessoas a tomarem os passos corretos para atingirem seus objetivos. São ações que usuários compreendem apenas ao olharem para o objeto, antes de usá-lo (ou senti-lo, caso seja um aparelho, e não um objeto em uma tela).”

Esse princípio está diretamente relacionado ao **_design_** **de interação**. Para interagir, o usuário precisa compreender o que o elemento da interface significa, qual é a sua função. Adivinhá-la levaria a um processo de tentativa e erro que pode fazer com que o usuário desista de usar o _software_. Uma boa _affordance_ evita também a necessidade de adicionar mais informações sobre o objeto (como _tooltips_ de explicação) e ocupar a tela.

![[Imagem47.png]]

Estudos de _affordances_ perceptíveis têm sido aplicados com mais frequência a interfaces de _desktop_ de teclado e ponteiro WIMP-GUI (_window_, _icon_, _menu_ e _pointing device_ – _graphic user-interface_, ou janela, ícone, _menu_ e dispositivo apontador – interface gráfica do usuário).

Nas interfaces GUI e na metáfora da área de trabalho, as _affordances_ convencionais geralmente são estáticas, ou seja, elas não contêm movimento e dependem de convenções **icônicas ou simbólicas** exibidas em locais esperados com rótulos ou ícones fixos para implicar uma interação, como os menus da barra de ferramentas.

**Vamos ver um exemplo?**

A imagem a seguir apresenta um _menu_ de ferramentas no _software_ Keynote. O item Ordenar está desdobrado com a ação do ponteiro do _mouse_.

![[Imagem2.png]]

Note que as opções indisponíveis são apresentadas com cinza claro. Apenas as disponíveis de serem executadas, ou seja, Alinhar Objetos e Distribuir Objetos, são exibidas na cor preta e nítida.

Metaforicamente, isso simula o mundo físico real e permite o **mapeamento** entre o digital e o material: objetos “próximos” podem ser tocados. Objetos “fora de alcance” não estão acessíveis a mão. A _affordance_ está clara ao fazer uso dessas metáforas visuais.

No entanto, em interfaces gestuais, como nas telas de toque dos celulares, pode não haver um objeto de controle (visível ou não), e o gesto para executar a ação pode ser mais complexo do que um simples “empurrar”, como, por exemplo, girar dois dedos ou deslizar quatro dedos. Eles não são facilmente comunicados por um botão ou pelos rótulos na tela usados ​​predominantemente em WIMP-GUIs.

Nesse caso, o _designer_ precisa compreender qual é o modelo mental do usuário, uma representação de como ele percebe o mundo conquistada por meio de experiências anteriores. Além de oferecer um modelo mental de acordo com as expectativas do usuário, o _designer_ precisa tornar essa representação visível na interface.

Sobre esse assunto, Norman (NORMAN, 2012, _apud_ CHUEKE, 2016:25) reitera:

> “Um dos poderes dos computadores modernos é a descoberta, você pode explorar, mas com sistemas de gestos é uma dor. É incrível quantas coisas as pessoas não sabem sobre os computadores que usam e não há como descobrir”.

Vamos observar outro exemplo.

Na imagem a seguir, é possível visualizar o sistema operacional do Apple iPhone (iOS). Na parte superior da tela (a), é possível observar uma guia de notificação que oculta uma aba do centro de notificações, onde estão reunidas todas as atualizações disponíveis do sistema, como mensagens de _e-mail_, avisos de aplicativos, alarmes, calendário, etc. Para revelar a guia (b), o usuário deve deslizar para baixo a partir do painel superior.

![[REVISADO-DPIU_STB15_UN2_IMAGEM.png]]

Essa dica visual é discreta e pouco informativa, pois não incorpora uma representação clara do gesto disponível para realizar, nem a direção correta, nem seu efeito. Nesta caso temos uma convenção. Ou seja, um símbolo criado de forma arbitrária. Como usuários devemos aprender com observação, seguido de tentativa e erro no uso correto deste recurso. E tudo bem, é necessário - e natural - tentar e errar para aprender. De qualquer forma, recomenda-se preocupação constante no design da UI, em informar o usuário todo o tempo das oportunidades de interação.

Ao conhecerem o mundo, as pessoas podem prever comportamentos específicos no caso de atos físicos aplicados sobre objetos digitais, que se assemelham a objetos familiares.

Por exemplo, se você deslizar um dedo da esquerda para a direita sobre um ícone, ele ou suas propriedades se moverão da esquerda para a direita. A imagem à baixo exemplifica essa ação: o conteúdo pictórico sugere o movimento que o usuário deve realizar, com a devida ativação baseada no toque (uso de apenas um dedo).

![[Imagem3.png]]

A representação visual do gesto também varia, podendo ser:

**Icônica**  
No exemplo anterior, faz-se uso de uma metáfora visual icônica, ou seja, a representação de uma mão reconhecível e o toque do dedo na tela.
![[iconica.png]]

**Simbólica**  
Por exemplo, um círculo demonstrando o dedo tocando a tela e a direção em que a tela deve ser “arrastada” para que mais informações possam ser exibidas.
![[simbolica.png]]

Veja, na imagem a seguir, um exemplo de representação visual simbólica.

![[Imagem4.png]]

Note que a dica visual para o gesto é “animada”, e não estática, ou seja, ela demonstra via movimento a direção do gesto. Esse recurso é indicado para maximizar a compreensão do usuário das ações implícitas requeridas pelo sistema e suas funcionalidades.

Perceba que os dispositivos _mobile_, de toque e multitoque, não permitem o chamado “clique com o botão da direita do dispositivo apontador”, como, por exemplo, um _mouse_ ou o _trackpad_ de um _laptop_.

![[Imagem56.png]]

Em dispositivos _mobile_, todas as ações acontecem com toques, multitoques (dois dedos), tocar e segurar, arrastar e deslizar sobre a tela. Diante dessas características, a indústria de dispositivos móveis teve de inovar no design da _user interface_.

Novas formas de interação tiveram de ser desenvolvidas para substituir o “clique da direita”, como é o caso do “tocar e segurar” no aplicativo Pinterest.

![[Imagem7.png]]

Outra metáfora visual que emergiu nos últimos anos foi o uso de “três pontinhos”: clicando neles, ações adicionais são exibidas ao usuário.

Nesse aplicativo de busca de ônibus, a exibição de uma _tooltip_ (dica) explica a função das “reticências” de oferecer mais opções de interação.

Perceba que as reticências, assim como na língua escrita, sugerem algo inacabado, ou por continuar; portanto, a metáfora visual é eficiente.

As reticências no exemplo são apresentadas verticalmente, devido ao pouco espaço horizontal na tela. No _design_ da UI, é comum fazer uso do formato horizontal ou vertical, dependendo do espaço disponível.

![[Imagem8.png]]

Veja algumas dicas sobre affordances para UI de desktops e aplicativos:  
  

- _Links_ e botões na tela remetem a ações como tocar, selecionar ou clicar. Em interfaces WIMP-GUI, esses objetos devem “reagir” ao passar o _mouse_ sobre eles, mudando de estado e informando que estão ativos e “clicáveis”.

- Em interfaces de toque, espera-se que os botões façam alguma ação e alterem a tela, ou seja, apresentem algum tipo de _feedback_.

- A depender do contexto, imagens, textos e gráficos podem indicar que é possível selecioná-los.

- Se o usuário não reconhecer que um objeto pode revelar mais informações, ele vai ignorá-lo como elemento decorativo e não funcional.

Agora que você já entendeu melhor o conceito de _affordance_ e a sua importância para o _design_ e a prototipação da interface do usuário, vamos conhecer a sequência natural das _affordances_, ou seja, o _feedback_, ou resposta à ação/_input_ do usuário.

### _Feedback_

O _feedback_ descreve o resultado imediato de uma ação, confirmando que foi realizada e apresentando mais informações para o usuário.

![[pedais.png]]

Quando falamos em dispositivos móveis, o _feedback_ deve ser imediato, indicando uma mudança perceptível de estado para diferenciar do estado anterior. Essa ação pode ocorrer de diversas formas.

![[Pasted image 20241015180812.png]]
![[Pasted image 20241015180842.png]]
![[Pasted image 20241015180909.png]]
![[Pasted image 20241015180930.png]]

O _spinner_ pode ser apresentado, por exemplo, na base da tela de um aplicativo de vendas de produto para indicar o carregamento de mais produtos. O tempo de carregamento é curto, e a lista – no caso do aplicativo de varejo – é infinita.

![[Imagem48 1.gif]]

Como pode ser visto na figura a seguir, é possível também apresentar a porcentagem na barra de progresso.

![[Imagem49.png]]

Outra solução de interface mais recente é o uso de **_skeletons_**. As telas que apresentam são basicamente uma página em branco na qual o conteúdo é carregado gradualmente. Veja um exemplo:

![[Imagem9.png]]

Áreas demarcadas em cinza apresentam o carregamento do conteúdo. Esse recurso é eficiente em informar ao usuário que o sistema continua responsivo e “trabalhando” para apresentar o conteúdo requisitado.

Além destes, outros _feedbacks_ possíveis são:

![[1.png]]
![[2.png]]
![[3.png]]

Veja um exemplo a seguir.

Na figura, pode ser observada a criação de nova senha em um sistema.

![[Imagem10.png]]

Nesse exemplo, é possível observar que a UI informa ao usuário que a senha está curta e, com isso, evita que o usuário submeta a senha para processamento. Sem esse tipo de _feedback_, impede que o usuário desperdice tempo e se fruste e que o sistema fique onerado com a requisição.

![[popup.png]]

Um exemplo desse tipo de _feedback_ é quando o usuário tenta fechar um arquivo sem salvá-lo antes, deletar arquivo singular ou em lote ou fechar múltiplas abas de um navegador _web_, como pode ser visto na figura a seguir:

![[Imagem11.png]]

É importante observar que um alerta de erro – como _feedback_ de uma ação – deve ser relevante ao usuário, falando sua própria língua. Erros técnicos, descritos em forma de código que apenas o desenvolvedor do sistema consegue interpretar, nada significam ao usuário final.

No exemplo, é possível ver um erro com descrição técnica, irrelevante para o usuário.

![[erro.png]]

As notificações de mudança também podem ser passivas. No exemplo a seguir, o sistema do Facebook informa ao usuário – sem que este tenha feito requisição alguma na tela – que existem alterações a serem verificadas nas telas de novos amigos e _posts_.

![[Imagem12.png]]

Outro aspecto fundamental a se investigar é a utilização de **restrições**. Esse recurso é utilizado para impedir que o usuário execute ações fora de hora ou não adequadas ao contexto da tela em que ele se encontra.

No _design_ de interfaces, as restrições podem ser usadas para:

- prevenir ou reduzir erros ao exibir mensagens para confirmação após o usuário pressionar botões de ações críticas como Excluir, Salvar ou Cancelar;
- adequar a exibição do conteúdo ao tamanho da tela do dispositivo do usuário;
- tornar botões que não são importantes em determinado contexto inativos, porém ainda visíveis. No exemplo a seguir, o botão para criação da conta só é habilitado após o usuário preencher os campos solicitados.

![[Imagem13.png]]

Vamos conhecer o estilo de _design_ adotado na última década no _design_ das interfaces _web_ e _mobile_. Confira mais a seguir.

### _Flat design_

Entre os estilos de _design_ visual mais utilizados em aplicativos nos últimos anos, está o _flat design_. É um estilo de _design_ de interface que enfatiza a baixa utilização de elementos estilísticos que dão a ilusão de **profundidade**, como o uso de sombras, gradientes ou texturas, e tem como foco um uso minimalista de elementos, tipografia e cores 'chapadas'.

Antes do _flat design_, predominava o uso de animações e ilustrações com excesso de efeitos visuais, que culminou no **skeumorfismo**, estilo que procura trazer para o meio digital as características de objetos reais, usando texturas, sombras e outros efeitos, muito utilizado pela Apple no iOS.

O _flat design_ se opõe a técnica do Skeumorfismo em favor de um _design_ mais simples, minimalista, com ênfase na usabilidade. Oferece cores saturadas, bordas nítidas e ilustrações em duas dimensões, semelhantes aos ícones. Isso evita distrações durante a experiência do usuário, focando nos aspectos funcionais. O uso das cores “chapadas”, contudo, ajuda a manter essa experiência agradável e atraente.

Veja um exemplo:

Na esquerda da figura podemos ver o logo antigo do Instagram. À direita podemos ver o logo atual baseado em conceitos de _flat design_.

![[Imagem14 1.png]]

Para projetar um _website_ ou aplicativo no estilo _flat design_, é preciso:

- focar na simplicidade e nos aspectos funcionais;
- focar no usuário;
- usar cores sólidas e brilhantes;
- não usar texturas;
- usar tipografia sem serifa;
- ser conciso e direto no uso de textos;
- destacar e tornar facilmente percebidos os componentes da interface, como _links_ e botões.

O _flat design_ inspirou a linguagem _material design_ do Google e o _design_ dos sistemas operacionais Windows a partir da versão 8. Acompanhe.

### _Material design_

O _material_ é um sistema de _design_ criado pelo Google para ajudar as equipes a criar experiências digitais de alta qualidade. Embora projetado inicialmente para o Android, o _material design_ pode ser aplicado em _websites_, _web-apps_ e em aplicativos para iOS.

Para conhecer os componentes e ferramentas descritos pelo _material design_, como barras de aplicativos, _banners_, botões, cartões, _chips_, tabelas de dados, seletores e campos de formulário, basta acessar a página _web_ [https://material.io](https://material.io).

Lá você encontra esses componentes, que são os blocos de construção interativos para criar uma UI.

_Softwares_ de _design_ da UI como Adobe XD, Figma, entre outros, fazem o uso de _templates_ que oferecem os componentes listados pelo estilo _material_.

É fundamental fazer uso desses padrões, sem receio de que eles restrinjam a criatividade. Padrões visuais são confortáveis para os usuários. Fazem a manutenção da expectativa deles ao encontrarem componentes em posições já conhecidas, além de ferramentas com uso e comportamentos também familiares.

Como vimos na seção inicial de _affordance_ e _feedback_, a UI apresenta elementos de interação de fácil identificação e conhecimento do uso, além dos resultados das ações do usuário. Iconografias, simbolismos e convenções visuais apresentam uso eficiente e efetivo, de acordo com os preceitos da ergonomia.

Conheça, a seguir, os principais **objetivos** do _material design_:

![[REVISADO-DPIU_STB4_UN2_INFOGRAFICO_ESTATICO 1.png]]

O _material design_ também segue alguns **princípios** básicos.

![[01 2 2.png]]
![[02 3 1.png]]
![[03 2 2.png]]

#### Ambiente

No _material design_, a UI apresenta um **ambiente tridimensional**, integrando luz e volume, projetando sombras.

![[Pasted image 20241015183359.png]]
![[Pasted image 20241015183425.png]]
#### Propriedades

Conheça, a seguir, as principais características gráficas da inteface digital do _material design_:

![[REVISADO-DPIU_STB7_UN2_CHECKLIST 1.png]]

Nesse exemplo, você pode ver materiais sólidos, com elevações diferentes.

![[propriedades.png]]

#### Elevações e sombras

A apresentação gráfica dos objetos na tela simula dimensão e profundidade. Ou seja, o eixo Z cria a ilusão de elevação do objeto.

Conheça mais características sobre as _elevações_ a seguir.

![[REVISADO-DPIU_STB8_UN2_vertical.png]]

As **sombras** indicam visualmente a profundidade de objetos com a simulação de luz projetada. No mundo físico real, observamos que é por meio da incidência de luz que sombras são projetadas. No ambiente digital, as sombras são simuladas.

#### Movimento

Os movimentos acontecem por meio de transições, ou animações utilizadas para apresentar relações espaciais, funcionalidades e intenções com fluidez e beleza. São inspirados pelos movimentos no mundo físico. Mostram o que o aplicativo pode fazer. Nesse sentido, o **_design_** **dos movimentos** deve:

![[REVISADO-DPIU_STB9_UN2_CHECKLIST 1.png]]

Em seguida, descreveremos o uso e a importância da cor em interfaces digitais.

#### Cor

Cores são utilizadas principalmente para comunicação visual, muitas vezes relacionada à identidade da marca associada ao aplicativo. Além da comunicação, as cores podem dar suporte ao conteúdo e à interação de diversas formas. Clique para conhecer mais características de como elas podem ser utilizadas.

- **Transmitir um estilo e valores associados ao propósito do aplicativo**:
	Pela escolha das cores, o aplicativo pode transmitir sensações diferentes, seja de alegria, entretenimento ou sobriedade e elegância.​

- **Diferenciar entre sessões da página**
	Cores são usadas para destacar alguns elementos e áreas da página em relação aos demais, estabelecendo relacionamentos e hierarquias ou dando suporte à estrutura do conteúdo e à sua separação.​

- **Diferenciar os elementos estáticos dos interativos**
	O uso de contrastes entre as cores pode ajudar os usuários a distinguir entre o conteúdo estático, como texto, e os elementos da interface com os quais o usuário pode interagir, como _links_ e botões de ação. Além disso, pode ajudar a distinguir os diferentes estados de um mesmo elemento.​

- **Comunicar o _feedback_ do sistema**
	O uso das cores pode ajudar a comunicar determinado tipo de _feedback_, diferenciando de forma mais rápida as mensagens de erro, alertas ou confirmação.


Quando escolhemos uma cor em um trabalho visual, devemos ter em mente que estamos lidando com um elemento de estímulo imediato e que essa cor escolhida provocará diversas reações em seus observadores, que podem ser positivas ou negativas, dependendo da sua utilização.

![[psicologia 1.png]]

A percepção de cores e de luminância, ou seja, nossa capacidade de perceber padrões de tons de cinza, resultou em diversas diretrizes de _design_ que podem ser utilizadas no projeto de interfaces com usuário.

O _material design_ oferece uma [ferramenta para seleção de cores](https://m2.material.io/design/color/the-color-system.html) primárias e secundárias de forma equilibrada. Veja:

![[Imagem15.png]]

#### Tipografia

A tipografia está relacionada à escolha correta da fonte do texto, incluindo família, estilo, tamanho, peso, variação, contraste, posição, espaçamento entre letras e espaçamento entre linhas. Sua origem está na impressão de livros e outros documentos, em que cada tipo (letra, número, etc.) era móvel, disposto lado a lado com os demais para compor o texto a ser impresso.

A sua aplicação em um _website_ já é um desafio devido às variações de resolução de tela, cores e contraste, tamanho e padrão do texto.

Nos dispositivos móveis, essa variação é ainda maior. O foco deve ser proporcionar a melhor legibilidade do texto de acordo com o contexto de uso, principalmente porque as condições de uso dos dispositivos requerem uma leitura rápida em ambientes com condições variadas de luminosidade.

A maior parte das fontes utilizadas em dispositivos móveis é vetorial em sua origem, mas transformada em pixels, o que acarreta perda dos detalhes, exceto nas resoluções mais altas. Por isso, a maior parte dos aplicativos utiliza as mesmas fontes, já adaptadas à leitura nos dispositivos.

A [escala do tipo](https://m2.material.io/design/typography/the-type-system.html#applying-the-type-scale) _material design_ é uma combinação de 13 estilos que são suportados pelo sistema de tipos. Este contém categorias reutilizáveis ​​de texto, cada uma com uma aplicação e significado pretendidos.

A escala de tipo apresentada na tabela a seguir usa o tipo de letra **Roboto** para todos os títulos, corpo e legendas, criando uma experiência de tipografia coesa. A hierarquia é comunicada por meio de diferenças no peso da fonte (_light_, _medium_, _regular_), tamanho, espaçamento entre letras e maiúsculas e minúsculas.

![[Imagem16.png]]

A escala de tipo aparece como texto nos componentes e no _layout_ geral. Os atributos de tipo podem usar valores personalizados para tipo de letra, fonte, maiúsculas e minúsculas, tamanho e espaçamento entre letras, títulos (_headline_), subtítulos, texto corrente (_body_), etc.

![[Imagem17.png]]

Os atributos sobre tipografia apresentados aqui, estão presentes no site do Material Design, recomendamos a leitura para maior entendimento.

[Clique aqui](https://m2.material.io/design/typography/the-type-system.html#applying-the-type-scale) e acesse!

A seguir, examinamos padrões para interfaces _web_ – formato _desktop_ – que se consolidaram ao longo das últimas décadas.

### Padrão e posicionamento de componentes da interface _desktop_ (_web_)

Com a popularização do conteúdo digital em _websites_, sistemas e aplicativos, também houve a necessidade de criar padrões específicos para um meio que envolve aspectos distintos das mídias impressas, pois há grande variedade de conteúdo e de formas de acessá-lo, e o leitor também pode interagir e produzir conteúdo.

O _designer_ elabora modelos de interface (_templates_) que podem ser usados em diversas páginas: artigos, perfis de usuário, notícias, mensagens, eventos, entre outros tipos de conteúdo que variam em relação ao conteúdo exibido, mas não em relação à sua estrutura.

![[imagem80.png]]

Nesses modelos, o _designer_ deve organizar as informações de forma hierárquica, estabelecendo as prioridades de acordo com os objetivos do usuário, ou seja, quais tarefas são necessárias para alcançar cada objetivo, quais informações e funcionalidades são necessárias para realizar cada tarefa e o contexto de uso.

É importante lembrar também de dois conceitos muito antigos, de _guidelines_ tradicionais do _webdesign_, que frequentemente são esquecidas pelos _designers_ e devem ser uma preocupação constante.

![[01 3 2.png]]
![[02 4 1.png]]

Outro ponto importante é o **tamanho da área de toque**. As áreas de toque de cada elemento da interface devem considerar o tamanho do ponteiro ou cursor.

O padrão das dimensões dessa área é de 24 px. Este é o tamanho de “alvo” recomendado para _links_, botões e imagens que são “clicáveis” com o ponteiro do mouse.

Isso pode ser visto no _website_ da W3C ([World Wide Web Consortium](https://www.w3.org/WAI/GL/mobile-a11y-tf/wiki/Proposed_SC_Target_Size#SC_Shortname)), que apresenta a padronização (_standards_) e regras de codificação das linguagens HTML e CSS. Veja, a seguir, a indicação dos tamanhos recomendados para o ponteiro de mouse ou _trackpad_ e toque na tela.

![[REVISADO-DPIU_STB12_UN2_INFOGRAFICO_ESTATICO.png]]

Conheça, na sequência, os principais componentes e seus posicionamentos para interfaces de _websites_.

#### Logotipo

O logotipo, ou marca, tem a função de identificar o _website_ e mostrar ao usuário a sua posição em relação à _web_ como um todo.

Geralmente fica localizado **no topo esquerdo da página e tem** **_link_** para a _homepage_. Observe:

![[logotipo.png]]

Esse padrão surgiu da cultura ocidental de **leitura da esquerda para a direita, de cima para baixo**.

#### Busca

O campo de _input_ da busca, ou _placeholder_, deve ter uma sugestão de ação.

![[busca.png]]

No exemplo a seguir, é possível ler “busque aqui o seu produto”, em um _website_ de comércio eletrônico. Atualmente cada vez mais se observa o uso de ícone de lupa no lugar do botão de ação.

![[Imagem19.png]]

As opções avançadas, com diferentes filtros e formas de buscar, devem sempre ser separadas em uma página de “busca avançada”.

Para sites de **_e-commerce_**, o natural é o posicionamento da **busca no lado esquerdo**. Já em sites **institucionais**, o comum é posicionar a **busca à direita**.

No exemplo a seguir, é possível ver o _website_ da eBay. O campo de busca em destaque fica posicionado à esquerda.

![[Imagem20.png]]

Já neste outro exemplo, vemos o _site_ institucional da IBM, no qual o campo de busca fica posicionado à direita.

![[Imagem21.png]]

#### Navegação global

A barra de navegação global contém os _links_ para as áreas-chave do site, as grandes categorias do modelo de organização. Frequentemente é o único elemento de navegação comum a todo o _website_ e, por isso, tem grande impacto na usabilidade.

Barras em formato horizontal têm quantidade de _links_ limitada para que a página não tenha _scroll_ horizontal. Uma alternativa, portanto, é criar mais de uma barra de navegação global, agrupando os _links_ por funcionalidade. O ícone de _drawer_ se tornou padrão na indústria tanto para interfaces _desktop_ como _mobile_.

![[Imagem22.png]]

#### Navegação local

A barra de navegação local apresenta _links_ para páginas que estão próximas, na estrutura do _website_, à página que está sendo visitada (páginas irmãs, filhas, pais, etc.). É importante que os _menus_ de navegação horizontal ou vertical se conectem com seus conteúdos por meio das seções ativas. Opções minimalistas proliferam – _menus_ que expandem e colapsam.

![[Imagem23.png]]

#### _Breadcrumbs_

Informam a posição da página na estrutura do _site_, mostrando _links_ para todas as páginas hierarquicamente superiores até a _homepage_. A página tem sempre o mesmo _breadcrumb_ (traduzido do inglês como ‘migalha de pão’) independentemente do caminho percorrido para alcançá-la.

Cada página tem um _breadcrumb_ único e hierárquico.

![[Imagem24.png]]

#### Navegação contextual (conteúdo relacionado)

Apresenta uma série de _links_ relacionados ao conteúdo da página que está sendo visitada, geralmente posicionados à direita da página e próximo ao conteúdo.

![[Imagem25.png]]

Ao longo dos anos, é observado o desenvolvimento de estratégias de _trending_ em _sites_ de comércio eletrônico, em que também são exibidos componentes que listam o que outros clientes do _site_ estão buscando e comprando. Isso pode influenciar o comportamento de compra e aumentar a receita do portal.

![[Imagem26-27.png]]

#### Mapa do _site_ e _footer_

O mapa do _site_ apresenta toda a estrutura do _website_, normalmente na forma hierárquica.

![[Imagem28.png]]

Esse recurso facilita o acesso de modo rápido e direto ao conteúdo. No entanto, não é recomendado para _websites_ com com pouca organização hierárquica. O mapa do _site_ está caindo em desuso e sendo substituído pelo _footer_, que tem apresentado, por padrão, além dos _links_ principais do _site_, atalhos para mídias sociais e formulários de inscrição em notícias relacionadas.

Agora que você já conheceu os padrões e o posicionamento de componentes da interface _desktop_, a seguir iremos examinar os padrões para interfaces mobile que se consolidaram ao longo da última década.

### Padrão e posicionamento de componentes da interface _mobile_

Os conceitos descritos nesta seção compreendem os sistemas operacionais para dispositivos _mobile_ mais populares: iOS e Android. Além disso, descrevem boas práticas do _design_ para aplicativos. Escrutinam comportamentos da UI (posicionamento de componentes, apresentação de cores e tipografias adequados à mídia), tamanho de alvos “tocáveis” para os dedos, etc. A mídia compreende dispositivos móveis.

Celulares têm, em média, um quarto do tamanho de uma tela _desktop_, e _tablets_, a metade. Portanto, escolhas de _design_ devem ser feitas para que favoreçam a adequação das ferramentas e dos conteúdos aos dispositivos em questão. Os usuários precisam identificar e compreender essa estrutura de forma rápida para continuar sua tarefa, evitar erros e obter uma boa experiência de uso.

Veja, a seguir, algumas recomendações para uma boa experiência do usuário em dispositivos móveis.

![[Respostas.png]]
![[polegar.png]]

Algumas porções da tela são desconfortáveis ergonomicamente para o alcance com o polegar. A figura abaixo mostra as áreas de toque de fácil (**natural**), ok (**stretching**) e difícil (**hard**) alcance para mão esquerda, direita e combinadas.

![[Imagem29.png]]

Para conhecer mais sobre a ergonomia para o alcance dos objetos na interface, recomendamos a leitura do artigo “**A área do polegar: Projetando para usuários mobile**”.

[Clique aqui](https://medium.com/@allanroubertie/a-%C3%A1rea-do-polegar-projetando-para-usu%C3%A1rios-mobile-c47a7820dcdd) e acesse!

![[touch.png]]

Como pode ser observado no gráfico a seguir, a Microsoft conduziu um estudo que testa a área de toque de alvos na UI em relação à porcentagem de erro em se atingir esses alvos com os dedos.

![[Imagem30.png]]

O estudo demonstrou que alvos menores que 5 mm (18 pixels) são difíceis para os usuários acertar. Os erros diminuem a partir dos 7 mm (26 pixels) em diante: 9 mm (34 pixels), 11 mm (41 pixels), 13 mm (49 pixels) são alvos adequados.

Portanto, considerando a média dos valores, o padrão das dimensões dessa área é de 44 px. Esse é o tamanho de “alvo” recomendado para botões e imagens que são “clicáveis”.

![[recomenda.png]]

O _material design_ também explica que o elemento gráfico de alvos como ícones e botões não precisa ter exatamente o tamanho recomendado de 48 x 48 px para toque ou 24 x 24 px para dispositivo apontador. A área de toque deve seguir essas recomendações, mas o ícone ou botão pode ser menor.

Essas áreas “invisíveis” podem ser definidas em ferramentas de prototipagem para posterior codificação HTML, como será visto na parte prática desta aula.

![[REVISADO-DPIU_STB1_unico.png]]

Com relação ao espaçamento mínimo entre alvos, o _material design_ sugere o valor de 24 px para evitar erros. O usuário pode acionar áreas que não condizem com suas intenções por acidente, caso esses alvos estejam muito próximos. A figura mostra ícones e o espaçamento adequado entre eles.

![[REVISADO-DPIU_STB17_unico.png]]

![[telefone.png]]

Como pode ser visto na imagem a seguir (Apple iPhone), algumas porções da tela não apresentam a melhor “sensibilidade” ao toque.

![[Imagem33.png]]

#### Abertura do aplicativo

Na primeira vez que o usuário abrir o aplicativo, deve ser oferecida uma tela sem possibilidade de interação enquanto ele aguarda o carregamento – é a chamada.

Na sequência, a UI oferece tutorial em etapas para o usuário tomar conhecimento das principais funcionalidades e benefícios do produto.

Algumas recomendações:

- É comum, após exibir a tela de abertura que apresenta a logomarca (_splash screen_), apresentar opções de _login_.
- Evite utilização da marca ou material publicitário na tela de carregamento, para que o usuário não ache que está vendo um anúncio.
- Quando o usuário abrir novamente o aplicativo, ofereça para ele o último conteúdo que foi acessado.

Tela de abertura do aplicativo com opções de *login* e registro.
![[Imagem34.png]]

Tela com tutorial apresentando algumas das principais funcionalidades do app.
![[Imagem35.png]]

#### Primeiras impressões
![[Pasted image 20241015193430.png]]
![[Pasted image 20241015193500.png]]
![[Pasted image 20241015193718.png]]

Ainda resistem, em interfaces _desktop_, as metáforas visuais como setas direcionais para indicar conteúdo “escondido”. As setas são exibidas apenas com o _mouse hover_ (pousar a seta do _mouse_ sobre o objeto de interesse e observar _feedback_) do ponteiro do _mouse_ sobre a lista horizontal de produtos disponíveis.

![[Imagem36 1.png]]

#### Tecnologia embarcada

É importante lembrar que o dispositivo _mobile_ apresenta tecnologias nativas que devem ser consideradas quando do _design_ da UX e UI.

![[check.png]]

#### Ações secundárias/microinterações

O usuário deseja ter acesso a controles que são secundários ou apenas relevantes para seções ou conteúdos específicos do aplicativo. Algumas interfaces podem dar acesso a diversas ações, porém nem todas têm a mesma importância, e é preciso evitar o excesso de informações na tela.

Recomenda-se deixar algumas ações ocultas na tela para que sejam descobertas pelos usuários por meio de gestos como tocar ou arrastar a tela.

Há inúmeras alternativas para revelar as ações secundárias. Acompanhe:

![[REVISADO-DPIU_STB14_UN2_INFOGRAFICO_ESTATICO.png]]

Agora que você conhece algumas alternativas para revelar ações secundárias, veja dois exemplos:

![[Imagem39.png]]
Apple iOS _e-mail_: é possível usar gestos de deslizar ou _swipe_ para revelar funcionalidades escondidas.

#### Entrada de dados

O usuário, ao se deparar com campos de busca, formulários, entre outros campos de _input_, aciona o surgimento do teclado virtual para digitar no campo.

O teclado exibido é nativo do sistema operacional (Apple iOs ou Android), e não do aplicativo ou web-app sendo usado. O teclado oferece diferentes visualizações entre as quais você pode alternar: uma com o alfabeto, outra com dígitos e uma terceira visualização com símbolos.

![[teclado.png]]
Alterne entre as visualizações pressionando estas teclas especiais: Pressione a tecla 123 para exibir uma visualização com dígitos e símbolos comuns. Pressione a tecla */= para mostrar símbolos menos comuns. Pressione a tecla ABC para retornar à visualização do alfabeto para seu idioma.

Seguem algumas recomendações quando no uso do teclado:  

- Cuidado com as entradas de dados automáticas. Decida quais estarão disponíveis no aplicativo: correção automática, capitalização automática (maiúsculas) ou complementação automática.
- Ofereça suporte para a orientação em paisagem na digitação de textos.

#### Gestos

É preciso considerar alguns fatores ao projetar suas interações com gestos:

**Invisibilidade**: gestos são invisíveis, por isso é preciso mostrar para o usuário como interagir.

**Duas mãos**: evite a exigência de uso das duas mãos para interagir com o aplicativo. Ofereça controles que possam ser utilizados com uma única mão.

![[Imagem41.png]]

#### Orientação

Os dispositivos _mobile_ podem exibir conteúdo no modo **retrato** (a mais utilizada) ou **paisagem**.

![[flip.png]]

Um dos assuntos mais recorrentes quando pensamos em ergonomia e interfaces _mobile_ é a forma como as pessoas seguram o _smartphone_ na hora de interagir com ele.

Steven Hoober no Site UX Matters (2014), fez uma pesquisa em profundidade para entender qual é a forma mais comum de segurar o celular de acordo com a tarefa que o usuário quer realizar. Dependendo da ação que o usuário quer realizar, é possível que ele segure o celular:

- com as duas mãos usando os dois polegares para interagir;
- com as duas mãos, em “conchinha”, usando um dos polegares para interagir;
- com uma das mãos, usando o dedo indicador da outra para interagir;
- com uma mão só, usando o polegar para interagir.
- É possível que ele considere a orientação paisagem principalmente para edição de texto e exibição de vídeos.
- Deve-se oferecer uma configuração que possibilite ao usuário bloquear a mudança de orientação.

![[REVISADO-DPIU_STB18_unico.png]]

#### Ações adicionais

Para finalizarmos esta aula, confira algumas das funcionalidades adicionais que podemos encontrar em _mobiles_.

![[REVISADO-DPIU_STB19_vertical 1.png]]

Os padrões e _templates_ oferecidos pela indústria e fabricantes existem para ajudar. Eles dão ordem ao caos de estilos gráficos que diferentes _designers_ estavam praticando. Os usuários, por sua vez, precisam de coerência e consistência. O conforto de encontrar telas, ferramentas, componentes, posicionamentos e comportamentos de UI que se mantêm não quebra expectativas e oferece o que o usuário precisa – e já conhece.

### Referências:

BABICH, N. **Disabled buttons in user interface.** UX Planet, 2021. Disponível em: [https://uxplanet.org/disabled-buttons-in-user-interface-4dafda3e6fe7](https://uxplanet.org/disabled-buttons-in-user-interface-4dafda3e6fe7). Acesso em: 25 nov. 2022.

BARBOSA, S. D. J. et al. **Interação humano-computador e experiência do usuário**. 2021. Disponível em: [http://leanpub.com/ihc-ux](http://leanpub.com/ihc-ux). Acesso em: 25 nov. 2022.

BUXTON, B. **Sketching user experiences**: getting the design right and the right design. San Francisco: Morgan Kaufmann, 2007.

CHUEKE, J. **Perceptible affordances and feedforward for gestural interfaces**: assessing effectiveness of gesture acquisition with unfamiliar interactions. City University of London, 2016. Disponível em: [http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556](http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556). Acesso em: 25 nov. 2022.

**COLOR tool (Material 2).** Disponível em: [https://material.io/resources/color/#!/?view.left=0&view.right=0&primary.color=512DA8](https://material.io/resources/color/#!/?view.left=0&view.right=0&primary.color=512DA8). Acesso em: 25 nov. 2022

DIX, A. et al. **Human-computer interaction**. 3. ed. Prentice Hall, 2004.

**ELEVATION (Material 2).** Disponível em: [https://material.io/design/environment/elevation.html](https://material.io/design/environment/elevation.html). Acesso em: 25 nov. 2022.

GARRETT, J. **The elements of user experience**: user-centered design for the web. New York: New Riders, 2003.

GIBSON, J. J. **The ecological approach to visual perception**. Boston: Houghton Mifflin, 1979.

GIBSON, J. J. **The senses considered as perceptual systems**. Boston: Houghton Mifflin, 1966.

HOOBER, S.; BERKMAN, E. **Designing mobile interfaces**: patterns for interaction design. O´Reilly, 2012.

HOOBER, S. **Insights on switching, centering, and gestures for touchscreens.** UX matters, 2014. Disponível em: [https://www.uxmatters.com/mt/archives/2014/09/insights-on-switching-centering-and-gestures-for-touchscreens.php](https://www.uxmatters.com/mt/archives/2014/09/insights-on-switching-centering-and-gestures-for-touchscreens.php). Acesso em: 16 mar. 2023.

KOTRUM, P. **HCI beyond the GUI**: design for haptic, speech, olfactory, and other nontraditional interfaces. Copyright Elsevier Inc., 2008.

KRUG, S. **Não me faça pensar!** Uma abordagem de bom senso à usabilidade mobile e na web. São Paulo: Market Press, 2015.

**LIGHT and shadows (Material 2).** Disponível em: [https://material.io/design/environment/light-shadows.html](https://material.io/design/environment/light-shadows.html). Acesso em: 25 nov. 2022.

LOPES, S. A. **Web mobile**: design responsivo e além para uma web adaptada ao mundo mobile. São Paulo: Casa do Código, 2014.

**MATERIAL Design.** Disponível em: [https://material.io/](https://material.io/). Acesso em: 25 nov. 2022.

**MATERIAL UI File upload example with Axios & Progress Bar.** Bezkoder, 2021. Disponível em: [https://www.bezkoder.com/material-ui-file-upload/](https://www.bezkoder.com/material-ui-file-upload/). Acesso em: 25 nov. 2022.

MCELROY, K. **Prototyping for designers**. Sebastopol: O’Reilly, 2017.

MEMÓRIA, F. **Design para a internet**. Campus, 2005.

NIELSEN, J.; LORANGER, L. **Usabilidade na web**: projetando websites com qualidade. Rio de Janeiro: Campus Elsevier, 2007.

NIELSEN, J. **Usability engineering**. Morgan Kaufmann Publishers, 1994.

NORMAN, D. **The design of everyday things**. Basic Books, 1988.

**PRINCIPLES (Material 1).** Disponível em: [https://m1.material.io/#introduction-principles]. Acesso em: 25 nov. 2022.

ROGERS, Y.; SHARP, H.; PREECE, J. **Design de interação**: além da interação humano-computador. 3. ed. Porto Alegre: Bookman, 2013.

ROUBERTIE, A. **A área do polegar: projetando para usuários mobile.** Medium, 2017. Disponível em: [https://medium.com/@allanroubertie/a-%C3%A1reado-polegar-projetando-para-usu%C3%A1rios-mobile-c47a7820dcdd](https://medium.com/@allanroubertie/a-%C3%A1reado-polegar-projetando-para-usu%C3%A1rios-mobile-c47a7820dcdd). Acesso em: 16 mar. 2023.

SIQUEIRA, R. **Como as skeletons screens podem ajudar a aprimorar a experiência de uso do seu produto.** UX Collective BR, 2019. Disponível em: [https://brasil.uxdesign.cc/como-as-skeletons-screens-podem-ajudar-aaprimoram-experi%C3%AAncia-de-uso-do-seu-produto-987c736651ca](https://brasil.uxdesign.cc/como-as-skeletons-screens-podem-ajudar-aaprimoram-experi%C3%AAncia-de-uso-do-seu-produto-987c736651ca). Acesso em: 25 nov. 2022.

STICKDORN, M. **This is service design doing**: applying service design thinking in the real world. O’Reilly, 2018.

TIDWELL, J. **Designing interfaces**: patterns for effective interaction design. Sebastopol, CA: O'Reilly Media, Inc., 2010.

**TYPE scale (Material 2).** Disponível em: [https://m2.material.io/design/typography/the-type-system.html#typescale](https://m2.material.io/design/typography/the-type-system.html#typescale). Acesso em: 25 nov. 2022.

USERLANE. **Software Advice**. Disponível em: [https://www.softwareadvice.co.uk/software/42687/userlane](https://www.softwareadvice.co.uk/software/42687/userlane) .Acesso em: 25 nov. 2022.

WEISER, M. **The computer for the 21st century.** Scientific American, 1991. Disponível em: [https://www.scientificamerican.com/article/the-computerfor-the-21st-century/](https://www.scientificamerican.com/article/the-computerfor-the-21st-century/). Acesso em: 16 mar. 2023.

**WHAT IS the optimum button size of touch screen applications?** UX, 2013. Disponível em: [https://ux.stackexchange.com/questions/39023/what-is-theoptimum-button-size-of-touch-screen-applications](https://ux.stackexchange.com/questions/39023/what-is-theoptimum-button-size-of-touch-screen-applications). Acesso em: 25 nov. 2022.

WIGDOR, D.; WIXON, D. **Brave NUI world**: designing natural user interfacesfor touch and gesture. Morgan Kauffman Publishers, 2011.

WROBLEWSKI, L. **Mobile first**. New York: A Book Apart, 2011.

**W3C - Proposed SC Target Size (2016).** Disponível em: [https://www.w3.org/WAI/GL/mobile-a11y-tf/wiki/Proposed_SC_Target_Size#SC_Shortname](https://www.w3.org/WAI/GL/mobile-a11y-tf/wiki/Proposed_SC_Target_Size#SC_Shortname). Acesso em: 25 nov. 2022.

## Prototipagem Aplicada II (Aula 3)

### Diretrizes globais

Vamos aprender agora sobre padrões relacionados à visualização e à apresentação de elementos da interface do aplicativo relacionados a **página, informação e componentes**. Esses padrões são relacionados a dispositivos móveis em geral. Padrões e diretrizes específicos das plataformas Android e iOS serão descritos no decorrer da aula.

Com a popularização do conteúdo digital em dispositivos _mobile_ (celulares e _tablets_), também houve a necessidade de criar padrões específicos para um meio que envolve aspectos distintos: tela de tamanho reduzido e ausência do dispositivo apontador das interfaces _desktop_.

A configuração de componentes que emergiu na última década, como áreas úteis, ferramentas e seus posicionamentos, será descrita a seguir.

#### Componentes

O _design_ de interfaces de aplicativos é uma evolução do _design_ para interfaces gráficas, já presentes tanto na plataforma _desktop_ quanto na _web_.

Nas interfaces _mobile_, alguns elementos são típicos e estão presentes como componentes de exibição de informação ou de interação. São como peças do brinquedo Lego, utilizadas em situações diversas.

Acompanhe a seguir.

##### Barra de rolagem

Para acessar conteúdo não visível na tela.
![[pos-graduacao/3º Acervo de imagens (Disc 1)/STB1.png]]

##### Barra de _status_

Informa as condições de componentes fundamentais do _hardware_ para a experiência do usuário, como nível de carregamento da bateria e conectividade.

É fixa, mas pode ser ocultada na exibição de tela cheia de conteúdos como vídeos.
![[STB2 3.png]]

##### Notificações

Exibição de informações sobre o aplicativo ou outros aplicativos, seja por mensagens de texto ou alertas sonoros.

Sua exibição é temporária.
![[STB3 3.png]]

##### Títulos

Essenciais para identificação de cada tela, são exibidos no topo e na horizontal para reconhecimento rápido.
![[pos-graduacao/3º Acervo de imagens (Disc 1)/STB4.png]]

##### _Menus_ ocultos

Exibidos a partir da interação do usuário, como clique em ícones ou arrastar a tela. Um dos ícones mais usados é o do “_menu_ hambúrguer”, que consiste em três linhas horizontais distribuídas na vertical para indicar uma lista.
![[pos-graduacao/3º Acervo de imagens (Disc 1)/STB5.png]]

##### _Menus_ fixos

Barra de navegação que está sempre presente na tela, geralmente composta por ícones com rótulos em textos relacionados.
![[pos-graduacao/3º Acervo de imagens (Disc 1)/STB6.png]]

##### _Home_

Tela de acesso às funcionalidades do aplicativo exibida após carregar o aplicativo ou quando o usuário não está realizando uma tarefa específica.
![[STB7 4.png]]

##### Tela de bloqueio

Utilizada pelo sistema para reduzir o consumo, prevenir entradas acidentais ou não autorizadas. Pode requerer senha para o desbloqueio.
![[STB8 4.png]]

##### Tela intermediária

Utilizada para que o usuário possa aguardar uma operação realizada pelo sistema, como carregamento de páginas. O sistema deve indicar o progresso da sua operação.
![[STB9 1.png]]

##### Anúncios

Devem ser distinguíveis do conteúdo e não podem atrapalhar a experiência do usuário.
![[STB10 1 1.png]]

##### _Link_

O usuário precisa acessar conteúdo relacionado a partir de qualquer lugar da página, incluindo dentro de textos ou em imagens. O _link_ é o padrão utilizado para carregar uma nova página, ir para outra seção da mesma página, abrir uma janela _pop-up_ ou revelar uma página adjacente.

São os elementos do hipertexto, consagrados pelas páginas na _web_. Quando inseridos em textos como parágrafos de artigos ou notícias, devem ser diferenciados dos textos comuns, seja pela cor (padrão azul escuro) ou pelo sublinhado.
![[STB11 1 1.png]]

##### Botão

Em algumas situações, principalmente em formulários, o usuário precisa realizar ações, enviar informações ou alterar o _status_.  

O botão é um padrão indicado para esses casos, derivado de objetos físicos que possibilitam interação, como máquinas, controle remoto de aparelhos e painel do elevador. Realiza ações imediatas que vão além da mera navegação entre páginas ou seções da página. Deve ser destacado visualmente e ter a “cara de objeto clicável”. Deve ter rótulo em texto, ícone ou combinação de ambos, indicando de forma precisa qual é a ação que realiza.
![[STB12 1 1.png]]

##### Ícone

Ícone é um padrão utilizado para representar de forma gráfica uma funcionalidade ou destino. São usados em navegações ou em botões de ação para reforçar a compreensão dos rótulos em texto. Em aplicativos, o uso de ícones é muito comum, pois ocupam pouco espaço na tela. Contudo, é importante acrescentar junto a ele, geralmente embaixo, o rótulo em texto, para melhor compreensão.
![[STB13 1 1.png]]

##### Campo de formulário

O usuário precisa de componentes na interface voltados para a entrada de dados. Os campos de formulário são padrões derivados dos formulários impressos, com áreas delimitadas que possibilitam a digitação de textos ou seleção de itens.

Para digitação de texto, existem os campos _text_, para textos em uma linha, e _textarea_, para textos em múltiplas linhas. Já para seleção de itens, os campos são do tipo radio, para seleção única, e _checkbox_, para seleção múltipla.

Para entrar dados em um campo, é preciso que ele esteja em foco, e o _designer_ deve destacar esse campo em relação aos demais pela presença de bordas mais grossas, cor de fundo diferente ou outros efeitos.

Campos podem ter dicas de preenchimento localizadas internamente, porém elas devem desaparecer quando o campo está em foco. Os campos devem ter rótulos localizados junto a eles de forma a possibilitar uma associação rápida.
![[STB14 1 1.png]]

##### _Menu_ de seleção

_Menu_ de seleção é um padrão utilizado para selecionar um ou mais itens pré-cadastrados em uma lista para entrar com dados em formulários. Requerem que os dados já estejam pré-cadastrados, e os itens são geralmente apresentados em ordem alfabética.

Muitas vezes são sinalizados pelo ícone **drawer**, ou gaveta - que são 3 trancinhas horizontais localizados no topo da tela (mais comumente à esquerda, mas também podendo ser apresentado à direita da tela).

Podem estar ocultos e ser exibidos a partir do toque no campo ou já ser exibidos na tela, em ambos os casos contendo uma barra de rolagem quando a quantidade de itens ultrapassar o limite. O campo deve apresentar um valor padrão, correspondendo à opção mais utilizada ou relacionada ao preenchimento prévio do mesmo formulário pelo usuário ou das mesmas informações em outros formulários do aplicativo ou sistemas relacionados.
![[STB15 4.png]]

#### Exibição da informação

Definida a organização das informações no aplicativo, incluindo quais irão aparecer em cada tela, é preciso apresentá-las na interface, comunicando suas importâncias e relacionamentos.

Para isso, é preciso considerar alguns atributos:
##### Posição
Objetos situados um pouco abaixo do topo da tela e na parte central são mais bem percebidos pelos usuários. Se for importante para a tarefa, alguns objetos podem ser fixos na tela, estando sempre visíveis (como um _menu_ fixo, por exemplo).

##### Tamanho
Objetos maiores chamam mais atenção, mas é preciso ter cuidado com a hierarquia visual para destacar aqueles mais importantes para a tarefa, além de evitar que um tamanho fora do padrão torne a função do objeto irreconhecível.

##### Forma
Alguns objetos apresentam formas padronizadas para facilitar seu reconhecimento. Avisos são identificados por triângulos; cantos arredondados podem facilitar o reconhecimento de um botão.

##### Contraste
Estabelece uma relação comparativa (claro-escuro) entre dois elementos adjacentes ou sobrepostos, descontando suas cores. Quando dois elementos têm muito contraste, sua legibilidade é favorecida.

##### Cor
Está relacionada a aspectos diferentes, como _branding_ e acessibilidade. Algumas cores são utilizadas como padrão para apresentar tipos de informação como _links_, mensagens de erro ou confirmação. É preciso manter a consistência nas cores padrão para não confundir o usuário.

##### Estilo 
Características visuais específicas que ajudam a diferenciar o elemento, como texto em negrito ou itálico.


A apresentação de informações pode ser feita por meio dos seguintes padrões:
![[01 4 2.png]]
![[02 5 1.png]]
![[03 3 2.png]]
![[04 1 2.png]]
![[05 1 2.png]]
![[06 1 1.png]]
![[07 2.png]]
![[pos-graduacao/3º Acervo de imagens (Disc 1)/08.png]]
![[pos-graduacao/3º Acervo de imagens (Disc 1)/09.png]]
![[10 2.png]]

A revelação de mais informações pode ser feita por meio dos seguintes padrões:

![[Pasted image 20241016122646.png]]
![[Pasted image 20241016120811.png]]
![[Pasted image 20241016120847.png]]
![[Pasted image 20241016120908.png]]

A seguir, iremos dissecar os componentes de interface do sistema operacional Android.

### Android
Após analisar os componentes para aplicativos de forma geral, passaremos para os principais componentes da interface para Android.

#### _Floating action button_
Um botão circular que muda de elevação e cor quando pressionado.

Usado em ações principais do aplicativo.

Muitas vezes é posicionado na base da tela.
![[STB19 1 1.png]]

#### _Raised button_
Um botão retangular que muda de elevação e cor quando pressionado.

Usado alinhado com outros elementos.

Geralmente usado para ações de confirmação da ação.
![[STB20 1 1.png]]

#### _Flat button_
Um botão sem cor de fundo que muda a cor do texto, porém não muda de elevação quando pressionado.

Usado em diálogos ou alinhado com outros elementos.

Geralmente usado para ações de cancelamento da ação.
![[STB21-1.png]]

#### Cartões
Elementos que servem de suporte para conteúdo como texto, imagens ou _links_.  

Geralmente são usados em listas com conteúdo.
![[STB22 1.png]]

#### Chips
Representação em um bloco pequeno que resume informações mais complexas, como contatos, e resultados de buscas e filtragens.  

Pode incluir ícone, texto, foto (no caso de contato telefônico ou _messenger_) e _link_.
![[STB23 1.png]]
#### Tabelas
Exibem dados e/ou ações relacionados a itens que fazem parte de um mesmo conjunto, como mensagens, contatos, eventos, etc.  

Devem ter cabeçalho para informar os nomes das colunas.  

Devem destacar os itens selecionados mudando a cor de fundo e dos campos de seleção. Podem prever ações gerais no topo, ações por item, ordenação por coluna, edição de cada item ou de cada dado, _menus_ de opção.  

Tabelas podem ser incluídas dentro de cartões.
![[STB24 1 1.png]]

#### Diálogos
Exibem informações sobre uma tarefa específica, podendo requerer decisões por parte dos usuários.  

Aparecem sobre o conteúdo da tela e podem desaparecer caso o usuário decida fechar ou executar uma ação requerida.  

Contêm textos e controles, como _links_ ou botões.  

Podem servir para alertas, confirmações, erros ou exibição de _menus_.
![[STB25 1 1.png]]

#### Divisores
Régua que ajuda a organizar o conteúdo de uma página por meio da divisão em itens ou seções com separação por linhas horizontais.

Muito utilizados em listas de mensagens.
![[STB26 1 1.png]]

#### Painéis expansíveis
São _containers_ que podem ser expandidos ou recolhidos para a edição de informações em tabelas ou formulários.  

Podem ser incluídos isoladamente ou dentro de cartões.  

Utilizam setas para indicar a possibilidade de expansão ou recolhimento.
![[STB27 1 1.png]]

#### _Grids_
Listas organizadas em células a partir da divisão em linhas e colunas.  

São utilizadas para que em cada célula seja exibido um item diferente, porém do mesmo tipo de informação, como uma galeria de fotos.
![[STB28 1.png]]

#### Listas
Apresentam uma série de itens organizados na vertical em múltiplas linhas.  

Cada item contém um título e ações complementares representadas por ícones ou textos. São utilizadas para apresentar informações de um mesmo tipo.  

Se o item contiver mais de três linhas, prefira o uso de cartões. Se o conteúdo for de imagens, prefira _grids_.
![[STB29.png]]

#### Controles de listas
Apresentam informações ou ações para os itens da lista. São exemplos de controles de listas: marcar (_checkbox_);

- habilitar/desabilitar (_switch_);
- reordenar (ícone);
- expandir/recolher (ícone de seta para baixo ou para cima).

Ações principais e estados são colocados na esquerda do item, e ações secundárias são colocadas à direita do item.

Podem ser exibidos com gestos do tipo _swipe_, ao deslizar o item com o dedo.
![[STB30 1.png]]

#### Menus
Exibem uma lista de opções a partir da interação com um botão, ação, ponteiro ou outro controle.

Cada item deve ocupar uma única linha, e o _menu_ deve conter no mínimo dois itens. Geralmente sinalizados pelo ícone drawer, ou gaveta.
![[STB31.png]]

#### Selecionador (_picker_)
Oferece a capacidade de selecionar data e horário utilizando _views_ consagradas, como calendário e relógio, para facilitar a interação, tornando-a mais natural para o usuário.

A opção escolhida deve ser destacada (data marcada ou horário escolhido).
![[STB32.png]]

#### Indicador de progresso e atividade
São indicadores visuais que representam operações do sistema, mostrando o tempo exato que vão demorar ou um tempo restante não determinado.

Podem ser lineares, em barra que vai de 0 a 100% preenchida de acordo com o progresso, ou circulares, que mostram o progresso até completar o círculo.

Podem ser carregados em etapas ou adicionando-se um conteúdo novo.
![[STB33.png]]

#### Controles de seleção
São usados para selecionar opções. Por exemplo:

- _checkbox_, para marcar múltiplas opções;
- _radio_, para marcar uma única opção;
- _switch_, para habilitar ou desabilitar a seleção.
![[STB34.png]]

#### _Sliders_
Possibilitam ao usuário selecionar valores dentro de uma escala ao movê-lo. Usados para configurações que refletem intensidade, como volume, brilho ou saturação de cor.
![[STB35.png]]

#### _Snackbars_
São barras que aparecem de forma breve para oferecer _feedback_ sobre uma operação exibindo uma mensagem em uma única linha, podendo conter uma única ação, como desfazer a operação.

Se houver necessidade de mais de uma ação, utilize um diálogo.
![[STB36.png]]

#### _Steppers_
Apresentam o progresso em uma sequência lógica e numerada de passos.

Podem ser editáveis ou não editáveis, opcionais, exibidos na vertical, horizontal, de forma linear ou não linear.

Outras formas de _stepper_, usadas em aplicativos, são aquelas que representam navegação em texto (Próximo e Anterior) com setas para navegação ou pontos, que mostram a quantidade de passos e em qual deles o usuário se encontra.
![[STB37.png]]

#### Títulos de seção
Espaços destinados a títulos de itens de listas, _grids_ ou _menus_.

São muitas vezes relacionados a critérios de filtragem ou ordenação de listas (galeria de fotos dividida por mês, por exemplo).
![[STB38.png]]

#### Abas
Possibilitam a navegação de alto nível hierárquico entre diferentes _views_, conjuntos de dados ou funcionalidades.

São apresentadas em uma linha única acima do conteúdo relacionado.

Seus rótulos ajudam a descrever esse conteúdo.
![[STB39.png]]

#### Campos de texto
Possibilitam a entrada de dados em texto pelos usuários e a visualização dos dados completados automaticamente pelo sistema.

Os campos são divididos em de linha única, múltiplas linhas ou ocupando toda a largura.

Têm rótulo, campo e dica. Os dados podem ser texto, número ou ambos.
![[STB40.png]]

#### Barras de ferramentas
Aparecem logo acima da _view_ afetada pelas ações.

Devem permanecer fixas na rolagem do conteúdo.

Ao arrastar um elemento para fora da tela, ele pode cobrir temporariamente a barra de ações.

Entre as ações, podem estar a busca e ícone para exibir navegação oculta.
![[STB41.png]]

#### Dicas
Um botão retangular que muda de elevação e cor quando pressionado.

Usado alinhado com outros elementos

Geralmente usado para ações de confirmação da ação.

![[STB42.png]]

Na próxima seção, investigaremos a cor dentro das interfaces Android.
#### Cor
Como já foi explicado na aula anterior, o Android faz uso da palheta de cores descrita no _material design_. Cores são geralmente opacas, mas podem receber o atributo de **_alpha_**, ou transparência. O Android oferece também uma ferramenta para seleção de cores primárias, secundárias e variantes mais claras/escuras de forma equilibrada.

Acompanhe, a seguir, como escolher a paleta de cores do seu aplicativo:

![[STB43a.png]]
![[STB43b.png]]
![[STB43c.png]]
Clique [aqui](https://m2.material.io/design) para acessar o _site_ do _material design_ e conhecer todas as suas possibilidades.

Agora, vamos entender como utilizar a tipografia no Android.

#### Tipografia

No Android, as fontes padrão são Roboto, a mais utilizada, e Noto.  
Acompanhe mais sobre elas no infográfico a seguir.
![[STB44a.png]]
![[STB44b.png]]
![[STB44c.png]]
Vamos agora conhecer os padrões da Apple iOS.

### Apple iOS

A Apple explica que a combinação de UX e UI do iPhone integra os recursos da plataforma e os recursos do dispositivo e faz algumas recomendações.

Permite que o usuário se concentre nas tarefas e no conteúdo principais, limitando o número de controles na tela e tornando os detalhes e as ações secundários detectáveis ​​com o mínimo de interação.

A UI se adapta às mudanças de aparência – como orientação do dispositivo, modo escuro, etc. –, permitindo que as pessoas escolham as configurações que funcionam melhor para elas.

É ergonomicamente pensada: permite interações que suportam a maneira como as pessoas geralmente seguram seus dispositivos.

Por exemplo, tende a ser mais fácil e confortável para as pessoas alcançarem um controle quando ele está localizado na área central ou inferior da tela.

O dispositivo integra as informações disponíveis por meio dos recursos da plataforma de maneira a aprimorar a experiência sem solicitar que as pessoas insiram dados.

Por exemplo, o usuário pode aceitar pagamentos, fornecer segurança por meio de autenticação biométrica/facial ou oferecer recursos que usam a localização do dispositivo. Isso tudo pode ser desativado nas configurações do sistema iOS.

A seguir, aprenda mais sobre os componentes de _layout_ para iOS.

#### Componentes de _layout_ iOS

Assim como o Android, o iOS oferece _templates_ de componentes e do _layout_, dimensionamento, cor, tipografia, etc. Esses elementos de interface são divididos em três categorias: **barras,** **_views_** **e controles**.

Vamos explorá-los a seguir.

##### Barras
Informam para os usuários sua localização no aplicativo. Oferecem navegação e podem conter botões ou outros elementos para iniciar ações e comunicar informações.

##### Barra de navegação
![[02 6 1.png]]
**Dicas:**
- Utilize o título da _view_ atual na barra de navegação.
- Evite excesso de controles na barra de navegação.
- Não inclua o caminho de navegação. Basta o botão de voltar à esquerda para navegar para o nível hierárquico superior.
- Considere configurar para a barra de navegação ficar oculta em determinadas situações, como exibição em tela cheia.
- Se utilizar muitos botões, dê espaço suficiente para os rótulos, usando apenas um separador vertical entre eles.

##### Barra de busca
![[02 7 1.png]]
**Dicas:**
- Use a barra de busca em vez de um campo de texto adaptado.
- Habilite os botões para limpar (ícone “X”) e cancelar.
- Utilize uma barra de busca proeminente, se a busca for uma funcionalidade primária, ou mínima, se for uma funcionalidade não frequente.
- Ofereça um _placeholder_ no campo de busca para exibir dicas de preenchimento. Se necessário, utilize uma frase acima do campo para melhor orientação.

##### Barra de _status_
![[02 8 1.png]]
**Dicas:**
- Utilize a barra de _status_ padrão do sistema iOS.
- Integre o estilo da barra de _status_ com o _design_ visual do seu aplicativo.
- Não utilize conteúdo abaixo da barra de _status_.
- Oculte a barra de _status_ quando exibir conteúdo em tela cheia.
- Não oculte a barra de status de forma permanente.

##### Barra de abas (_tab bars_)
![[02 9 1.png]]
**Dicas:**
- Utilize as barras de abas para organizar informações em poucas categorias.
- Assegure-se de que todas as abas sejam navegáveis, mesmo que não haja conteúdo. Nesse caso, explique o motivo de não haver conteúdo e ofereça ajuda.
- Utilize somente para navegação. Para realizar ações já existe a barra de ações.
- Evite usar muitas abas; mantenha entre 3 e 5 abas.
- Destaque a aba atual.
- Se houver novo conteúdo na aba, informe a quantidade por meio de um ícone específico (_badge_) com o número correspondente.
- A navegação entre as abas somente deve afetar a _view_ na qual a barra está incluída.

##### Barra de ferramentas
![[02-1.png]]
**Dicas:**
- Escolha as ações mais relevantes, usadas com maior frequência.
- Considere o uso de ícones (3 a 5 botões) ou botões com texto (para 3 botões ou menos).
- Evite utilizar para navegação entre contextos diferentes. Se for esse o caso, prefira a barra de abas.
- Se utilizar muitos botões, dê espaço suficiente para os rótulos, usando apenas um separador vertical entre eles.

##### _Views_
Contêm o principal conteúdo que os usuários veem no aplicativo, como textos, gráficos, animações e elementos interativos. Podem conter comportamentos como rolagem, inclusão, exclusão e organização de conteúdo.

Acompanhe a seguir as principais _views_ do iOS.

###### Folhas de ação (_action sheets_)
![[01 5 1.png]]
![[02 10 1.png]]
**Dicas:**
- Ofereça um botão para cancelar na base da folha de ações.
- Destaque as opções mais críticas, como Excluir, e as inclua no topo das opções.
- Desabilite a rolagem na folha de ações.

###### _Views_ de atividades (_activity views_)
![[01 6 1.png]]
![[02 11.png]]
**Dicas:**
- Crie rótulos para as atividades que as descrevam de forma sucinta, pois aparecem abaixo do ícone, e há pouco espaço.
- Certifique-se de que as atividades tenham sentido no contexto atual.
- Utilize um botão de ação para exibir a _activity view_.

###### Alertas
![[01 7 1.png]]
![[02 12.png]]
**Dicas:**
- Use com cautela, somente para situações importantes, como confirmação de compra, de ações destrutivas, como exclusão de conteúdo, e notificações de problemas.
- Teste a aparência do alerta em ambas as orientações de tela.
- Utilize títulos e mensagens curtos e descritivos para os alertas.
- Evite utilizar insultos, acusações ou julgamentos.
- Evite explicar os botões utilizados no alerta. Utilize rótulos claros e concisos.
- Geralmente, utilize dois botões de alerta.
- Coloque os botões de alerta nos locais esperados.
- Destaque os botões que realizam ações destrutivas, como exclusão.
- Possibilite que o botão Home do dispositivo cancele o alerta.

###### Coleções
![[01 8 1.png]]
![[02 13.png]]
**Dicas:**
- Evite criar _designs_ radicais. Facilite a seleção de itens providenciando espaço suficiente na tela para a área de toque.
- Considere utilizar uma tabela em vez de uma coleção para conteúdo em texto.
- Utilize cautela quando realizar mudanças dinâmicas no _layout_. A mudança deve fazer sentido para facilitar o uso.

###### _Image view_
![[02-1 1.png]]
**Dicas:**
- Assegure-se de que todas as imagens em uma _image view_ tenham tamanho consistente, se possível ajustado, antes de serem incluídas no aplicativo.

###### Mapas
![[02 14.png]]
**Dicas:**
- Mantenha o mapa interativo.
- Utilize cores esperadas para os marcadores de localização, de acordo com o existente no aplicativo padrão.

###### _Popovers_
![[02-1 2.png]]
**Dicas:**
- Evite o uso no iPhone; use somente no iPad. No _smartphone_, prefira usar janela modal em tela cheia.
- Utilize um botão de ação para fechar o _popover_, cancelar a operação ou concluí-la.
- Sempre salve o trabalho após fechar um _popover_, pois é fácil fechá-lo ao clicar em outro ponto da tela.
- Posicione o _popover_ sem cobrir conteúdo essencial que precise ser visto mesmo com o _popover_ aberto.
- Mostre um _popover_ de cada vez.
- Não exiba outra _view_ sobre o _popover_, exceto alertas.
- Evite usar um tamanho excessivo no _popover_.
- Ofereça transição suave nas mudanças de tamanho do _popover_.

###### _Scroll views_
![[02 15.png]]
**Dicas:**
- Possibilite o _zoom_ de forma apropriada, configurando valores máximo e mínimo de escala de forma que façam sentido.
- Se a _scroll view_ estiver em modo de página, ofereça um controle apropriado para navegação.
- Não inclua uma _scroll view_ dentro de outra _scroll view_.
- Exiba uma _scroll view_ de cada vez.

###### _Split views_
![[01 9 1.png]]
![[02 16.png]]
**Dicas:**
- Escolha um _layout_ na _split view_ que esteja de acordo com o seu conteúdo.
- Destaque sempre no painel secundário o item de navegação relacionado ao conteúdo ativo.
- Em geral, utilize navegação apenas em um dos painéis.
- Ofereça mais de uma forma para acessar um painel principal que está ocultado, como botão de ação e gestos.

###### Tabelas
![[02-1 3.png]]
**Tipos de tabelas**
- **Simples:** linhas podem ser separadas em seções rotuladas, e um índice opcional pode aparecer do lado direito. Pode conter cabeçalho e rodapé antes e depois de cada seção.
- **Agrupada:** linhas são apresentadas em grupos, sem apresentar índice. Pode conter cabeçalho e rodapé antes e depois de cada seção.

**Tipos de linhas**
- **Padrão:** imagem opcional no lado esquerdo, título alinhado à esquerda. Setas para a direita são usadas na direita para indicar que o item é usado para navegação. Evite itens que requeiram informações adicionais.
- **Subtítulo:** utiliza uma linha para o título e outra para o subtítulo logo abaixo. Como variação, o subtítulo pode estar na coluna seguinte, na mesma linha do título. Depende da extensão desejada.

**Dicas:**
- Considere a largura da tabela para evitar sobreposição das colunas quando reduzida e distância excessiva quando ampliada.
- Utilize títulos sucintos para evitar sobreposição.
- Apresente logo o conteúdo no carregamento, sem esperar pelo carregamento total.
- Informe o progresso de atualização do conteúdo.
- Atualize o conteúdo para refletir novas informações
- Evite combinar o índice com elementos alinhados à direita da linha.
- Ofereça _feedback_ quando o item é selecionado, seja por _checkbox_ ou ícones que indicam seleção do item.

###### _Text views_
![[01 10.png]]
![[02 17.png]]
**Dicas:**
- Mantenha o texto legível usando _dynamic type_, mesmo com mudanças de estilo ou do tamanho do texto no dispositivo.
- Mostre o teclado apropriado ao tipo de conteúdo (texto, números, telefone, _e-mail_, endereço _web_, etc.).

###### _Web views_
![[02 18.png]]
**Dicas:**
- Habilite a navegação para avançar e voltar, utilizando controles com setas, de forma a possibilitar a visita em diversas páginas.
- Evite utilizar uma _web view_ como se fosse um navegador alternativo. Use somente dentro do contexto do aplicativo, pois, para acessar _websites_ em geral, já existem navegadores apropriados no dispositivo do usuário.

##### Controles
Iniciam ações e oferecem informações. São exemplos de controle: botões, _switches_, campos de texto e barras de progresso.

Veja, a seguir, os principais controles do iOS:

###### Botões
![[02 19.png]]
Há três tipos de botões:

■ **Botões de sistema:** aparecem com frequência em barras de navegação ou de ações, mas podem ser usados em qualquer lugar. Dicas:
- Utilize verbos nos títulos.
- Utilize títulos concisos.
- Considere usar uma borda ou cor de fundo apenas quando for necessário.

■ **Botões de divulgação de detalhes:** abrem _views_, geralmente modais, contendo informações adicionais ou funcionalidades relacionadas a um item específico na tela. Mais utilizados em tabelas.

■ **Botões de informações:** revelam detalhes de configuração sobre um aplicativo, às vezes por trás da _view_ atual, após esta ser girada.

■ **Botões para adicionar contatos:** exibem uma lista de contatos existentes para incluir um deles em um campo de texto ou outra _view_. É preciso considerar também a alternativa de incluir o contato por texto.

###### _Menus_ de edição
![[02-1 4.png]]
**Dicas:**
- Mostre ações relacionadas ao contexto atual. As demais podem ser desabilitadas.
- Possibilite que os usuários utilizem os gestos padrões para acessar as opções do _menu_.
- Ajuste a posição do _menu_ para impedir que cubra conteúdo importante.
- Não implemente outros controles com a mesma funcionalidade do _menu_ de edição.
- Possibilite que os textos não editáveis sejam selecionados e copiados pelos usuários.
- Não adicione as opções de edição a um botão para que este não seja ativado na seleção.
- Possibilite que o usuário desfaça qualquer ação de edição.
- Expanda as opções de edição adicionando outros comandos, mas só os exiba após os comandos padrão.
- Evite excesso de opções.
- Utilize rótulos curtos para os comandos de edição.

###### Rótulos (_labels_)
![[01 12.png]]
![[02 20.png]]
Rótulos podem apresentar qualquer quantidade de texto estático, mas é melhor mantê-los curtos e legíveis, mesmo quando têm um estilo aplicado ou o usuário altera o tamanho padrão do texto do dispositivo.

###### Controles de página (_page controls_)
![[02-1 5.png]]
**Dicas:**
- Os usuários podem tocar na borda inicial ou de saída de um controle de página para visitar a página seguinte ou anterior, mas não podem tocar em um ponto específico para ir para uma página específica.
- Não devem ser usados para páginas organizadas hierarquicamente, somente para sequência de páginas em um mesmo nível.
- Não exiba muitas páginas, pois mais de 10 pontos são difíceis de serem contados, e mais de 20 páginas tomam muito tempo para serem navegadas.
- Centralize o controle de páginas na parte inferior da tela, abaixo do conteúdo.

###### Selecionadores (_pickers_)
![[01 13.png]]
![[02 21.png]]
**Dicas:**
- Ordene os valores de forma previsível para o usuário, pois a maior parte da lista está oculta.
- Evite mudar de _view_ para mostrar o selecionador. Funciona melhor quando mostrado junto ao conteúdo, no contexto, abaixo ou próximo ao campo relacionado.

###### Indicadores de progresso
![[01 14.png]]
![[02 22.png]]
São divididos em dois tipos:
- **Indicadores de atividade:** mostram, por meio de um ícone animado, apenas que o sistema está processando a operação. É útil fornecer mais informações para o usuário.
- **Barras de progresso:** mostram o progresso da atividade em relação ao tempo total estimado. Use quando a duração for conhecida.

###### Controle de segmentos
![[02-1 6.png]]
**Dicas:**
- Limite a quantidade de segmentos.
- Mantenha a quantidade de conteúdo dos segmentos consistente.
- Evite misturar texto e ícones em um controle de segmento.
- Posicione o conteúdo de forma apropriada em um segmento, sem desalinhar.

###### _Sliders_
![[02 23.png]]
**Dicas:**
- Customize a aparência do _slider_ se agregar valor.
- Não use o _slider_ para ajustar o volume do áudio, pois já existe uma _view_ específica para volume, que é customizável e oferece maior capacidade de configuração.

###### _Steppers_
![[02-1 7.png]]
**Dicas:**
- Apresente de forma clara o valor afetado pela interação com o _stepper_.
- Não utilize o _stepper_ para realizar grandes alterações de valor. Ele funciona melhor quando as mudanças requerem poucos toques no controle.

###### _Switches (toggle)_
![[02 24.png]]
**Dicas:**
- Considere alterar a aparência do _switch_ de acordo com o _design_ visual do aplicativo.
- Utilize somente em _views_ em tabela, relacionados a itens.
- Evite usar rótulos para descrever os valores, pois os estados são sempre ligado e desligado.
- Considere utilizar _switches_ para habilitar ou desabilitar elementos de interface relacionados.

###### Campos de texto
![[02-1 8.png]]
**Dicas:**
- Mostre uma dica dentro do campo em um _placeholder_ para comunicar seu propósito.
- Utilize campos de texto de segurança, que não exibem os caracteres digitados, substituindo por “*” em senhas e outras informações críticas.
- Mostre o tipo de teclado apropriado (texto, número, endereço web, _e-mail_, telefone, etc.).
- Utilize imagens e botões ao lado do campo para indicar funcionalidades adicionais.
- Mostre no final do campo um botão “X” para limpar o conteúdo digitado no campo.

##### Cores

No iOS, as cores identificam a interatividade, proporcionam consistência visual e transmitem vitalidade. Veja os princípios de aplicação de cores nessa plataforma:

- Utilize cores complementares, de forma coordenada e harmônica.
- Utilize uma paleta de cores limitada e relacionada ao logotipo do aplicativo, usando as cores de forma sutil.
- Utilize uma cor específica para enfatizar os elementos interativos no aplicativo, tornando-a mais destacada do que as demais cores.
- Evite utilizar a mesma cor para elementos interativos e não interativos.
- Considere como as variações de cores em determinados elementos ou _views_, incluindo uso de transparência, afetam as cores próximas.
- Aplique nas imagens usadas no aplicativo o mesmo perfil de cor padrão do iOS, o Standard RGB (sRGB).
- Teste o esquema de cores do seu aplicativo em situações diversas de luminosidade do ambiente físico.
- Considere como o display True Tone, que usa sensores para ajustar o ponto branco da tela para se adaptar às condições de luminosidade do ambiente, afeta as cores do seu aplicativo.
- Considere os usuários daltônicos e como as diferentes culturas percebem as cores.
- Utilize contraste suficiente para favorecer a legibilidade.

O iOS 7 introduziu uma nova propriedade na UI denominada _tintColor_. Ela é usada para indicar visualmente quais controles na tela estão ativos ou têm uma ação associada a eles. Por exemplo, os botões em barras e barra de abas usam cor de matiz por padrão.

![[STB73.png]]

#### Tipografia

No iOS, a fonte do sistema é a San Francisco, que tem duas variantes: SF UI Text, para textos com 19 pontos ou menores, e SF UI Display, para textos com 20 pontos ou maiores.

Quando se usa a fonte do sistema para texto em rótulos ou outros elementos da interface, o iOS aplica o estilo de texto mais apropriado com base no tamanho do ponto. Também altera as fontes automaticamente se for necessário e respeita as configurações de acessibilidade.

![[img1 1.png]]

Veja os princípios de aplicação de tipografia nessa plataforma:

■ Destaque as informações mais importantes por meio de peso, tamanho e cor.
■ Utilize, se possível, uma única fonte e algumas variações de estilo e tamanho.
■ Utilize os estilos de texto já disponíveis, baseados nas fontes do sistema:
- Title 1
- Title 2
- Title 3
- Headline
- Body
- Callout
- Subhead
- Footnote
- Caption 1
- Caption 2

Assegure-se de que as fontes customizadas, aquelas que não fazem parte do sistema, estejam legíveis. Só utilize fontes customizadas quando houver muita necessidade, como para fins de identidade da marca. Certifique-se de que essas fontes customizadas atendam aos requisitos de acessibilidade.

A seguir, discutiremos questões de acessibilidade para _web_ e _mobile_.

### Acessibilidade

Nesta seção, iremos investigar conceitos sobre a acessibilidade, um dos requisitos de qualidade de um projeto de sistemas e produtos, sejam eles para interfaces _desktop_, _mobile_ ou dispositivos móveis.

#### Princípios gerais de acessibilidade

A acessibilidade é um requisito de qualidade de um produto, espaço ou sistema que certifica que estes possam ser usados de forma universal, incluindo pessoas que possuem dispositivos diversos ou aquelas com alguma dificuldade física, seja visual, auditiva, motora ou cognitiva.

O Decreto nº 5.296/2004 explica: acessibilidade é “**condição para utilização, com segurança e autonomia**, total ou assistida, dos espaços, mobiliários e equipamentos urbanos, das edificações, dos serviços de transporte e dos dispositivos, sistemas e meios de comunicação e informação, **por pessoa portadora de deficiência ou com mobilidade reduzida**”.

É um requisito que precede a própria usabilidade, pois, se o usuário não consegue acessar, por exemplo, o conteúdo e as funcionalidades do aplicativo, ele não conseguirá interagir com ele e ter a experiência de uso.

> Na internet, o termo “acessibilidade” se refere também a recomendações do W3C, que visam a permitir que todos possam ter acesso aos _websites_, independentemente de terem alguma deficiência ou não. As recomendações abordam desde o tipo de fonte a ser usado, bem como seu tamanho e cor, de acordo com as necessidades do usuário, até orientações relativas ao código (HTML e CSS, por exemplo).
ACESSIBILIDADE. 2022. Disponível em: [https://pt.wikipedia.org/wiki/Acessibilidade](https://pt.wikipedia.org/wiki/Acessibilidade). Acesso em: 22 dez. 2022.

Fazendo uma relação com o conteúdo da aula 1, um _site_ responsivo ajuda na acessibilidade a partir de dispositivos diferentes, mas não garante que seja automaticamente acessível para todos os usuários. Enquanto no _design_ responsivo a preocupação é adequar o _layout_ e o conteúdo para visualização em dispositivos diversos, na acessibilidade o foco é que esse conteúdo seja acessível por usuários diversos.

Um exemplo de acessibilidade no _design_ de aplicativos é o uso de cores e contrastes suficientes entre cor do texto e do fundo para leitura por pessoas com baixa capacidade de visão.

A ideia é comunicar uma informação utilizando mais do que o uso de cores para evitar confusão por parte de pessoas daltônicas.

![[Pasted image 20241016160129.png]]
![[Pasted image 20241016160156.png]]
![[Pasted image 20241016160226.png]]
![[Pasted image 20241016160249.png]]

Veja alguns princípios que devem ser seguidos para promover a acessibilidade em diferentes plataformas.

#### Acessibilidade de _websites_

**Diretrizes de acessibilidade para conteúdo web da W3C**

Para saber mais sobre os princípios de acessibilidade, clique [aqui](https://www.w3.org/Translations/WCAG20-pt-br/WCAG20-pt-br-20141024/) e acesse as diretrizes.

Para _websites_, são feitas as seguintes recomendações.

##### Recomendações visuais (_design_ universal)
- Utilize fontes de bom tamanho e legíveis.
- Escolha ícones claros e objetivos.
- Evite elementos que possam distrair, como elementos animados.
- Utilize linguagem objetiva, com frases e parágrafos curtos.
- Indique no texto de _link_ o próprio conteúdo a que se destina. Evite o 'clique aqui'.
- Use um _layout_ consistente entre páginas do _site_.
- Evite imagens de fundo atrás de texto.
- Use abreviações, acrônimos e termos técnicos apenas quando necessário; eles devem conter explicação e, quando possível, ser evitados.
- Contemple resoluções de diferentes dispositivos (responsivo/adaptativo).
- Faça seu _design_ ser bom para o SEO do Google (_search engine optimization_).

##### Baixa acuidade visual
- Aplique texto redimensionável.
- Utilize controle para redimensão de textos.
- Opte por texto incluído em imagens (_alternate text_, apresentado quando no _mouse hover_ do cursor).
- Use títulos largos.
- Aplique _links_ em alto contraste.
- Mantenha contraste de cores (texto, fundo, botões).

##### Dificuldades motoras
- Utilize grandes alvos clicáveis.
- Aplique _links_ reativos a _hover_ (_focus_).
- Use a tecla Tab do teclado para que o usuário possa navegar sequencialmente (troca de foco) pelos _links_ e áreas clicáveis da UI.

#### Acessibilidade _mobile_

**Diretrizes de acessibilidade para conteúdo web da W3C**

Para saber mais sobre os princípios de acessibilidade, [clique aqui](https://www.w3.org/WAI/standards-guidelines/mobile/) e acesse as Diretrizes de Acessibilidade para Conteúdo Web da W3C.

Para dispositivos _mobile_, são feitas as seguintes recomendações.

##### Som, vídeo e animações
Possibilite navegação somente por áudio para pessoas com dificuldades visuais ou por meios visuais para pessoas com dificuldades auditivas. Por exemplo, notificações em áudio devem ser sempre acompanhadas de notificações em texto, e vice-versa.

Evite excessos incluindo sons e imagens desnecessários, como músicas de fundo.

Use animações em transições de visualizações para manter o foco do usuário.

Configure controles de objetos, como vídeos, para desaparecerem após determinado tempo para não ocuparem espaço na tela.

##### Componentes da interface
Utilize componentes padrões da interface do dispositivo.

Evite ocultar controles de funções de alta prioridade.

##### Toque 
Mantenha a área de toque dos elementos com no mínimo 48 x 48 dp para possibilitar o toque por qualquer pessoa.

Separe as áreas de toque entre os elementos por no mínimo 8 dp para evitar erros.

##### Texto
Ofereça tamanho e contraste suficientes para leitura.​

Mantenha o texto legível mesmo se o usuário utilizar _zoom_ para aumentar o seu tamanho.

Possibilite o ajuste do tamanho da fonte por parte do usuário usando a unidade sp (_scaleable pixels_).

##### Navegação 
Oriente o usuário quanto à sua localização dentro do aplicativo, incluindo o oferecimento de _feedback_ visual para apontar onde o usuário se encontra em _menus_ de navegação (sessão ativa).

Reduza a quantidade de passos na navegação e no fluxo das tarefas. Considera-se adequado até três etapas para alcançar objetivos. Mais do que isso pode gerar confusão e desperdício de tempo.

Implemente o controle de foco para possibilitar a navegação pelo teclado, estabelecendo uma ordem para a troca de foco dos elementos da interface.

Possibilite, por meio dos leitores de tela, que os usuários com dificuldades visuais ouçam as descrições do conteúdo ao percorrerem a tela com seus dedos (explorar com os dedos) ou ao deslizarem os dedos pela página linearmente (navegação linear).

##### Hierarquia visual 
Torne os elementos mais visíveis (alto contraste figura-fundo).

Ofereça uma hierarquia da informação clara.

Destaque as informações mais importantes usando cores, ênfase, animações ou dicas em texto.

​Posicione as ações mais importantes no topo da página para acesso rápido.

Agrupe os elementos da interface e os conteúdos que são relacionados para melhor distinção por pessoas com dificuldades visuais.

##### Ajuda
Ofereça rótulos em texto para todos os elementos, para que pessoas com dificuldades visuais possam compreender o conteúdo.

​Inclua as informações sobre acessibilidade na documentação de ajuda do aplicativo.

Use textos curtos, diretos, descritivos e independentes para melhor diferenciação pelo usuário e velocidade de leitura pelas tecnologias assistivas.

Indique no texto alternativo no elemento da interface o que esse elemento faz, especificando a tarefa. Evite o 'clique aqui'.

Utilize verbos para descrever o que o elemento faz.

​Não diga para o usuário como ele deve interagir com o elemento da interface. Deixe que a tecnologia assistiva faça essa descrição.

##### Funcionalidades específicas
Para pessoas com dificuldades específicas, ofereça algumas funcionalidades especiais, como leitores de tela, ferramentas para ampliar texto e outros elementos, auxílio para audição e memorização.

Possibilite que o usuário faça alterações no aspecto da aplicação por meio das definições de acessibilidade do dispositivo.

#### Tecnologias assistivas

Existem diversas ferramentas para auxiliar na acessibilidade, como leitores de tela, analisadores de níveis de contraste em cores, validadores de código HTML e tecnologias assistivas dos próprios dispositivos.

As principais tecnologias assistivas das plataformas são os programas de leitura de tela VoiceOver no iOS e TalkBack no Android.

![[img2 1.png]]

Para verificar a acessibilidade dos aplicativos, podem ser realizados diversos testes. Veja os mais comuns:

- Leitura de tela para acesso por pessoas com dificuldades visuais
- Ampliação do tamanho do conteúdo (_zoom_)
- Níveis de contraste entre as cores
- Facilidade de leitura do texto
- Navegação
- Sem som
- Sem cores
- Uso apenas por controles de voz

Nesta aula, investigamos as características de _design_ dos sistemas operacionais Andoid e iPhone para _mobile_. O conhecimento dos padrões de páginas e componentes permite que criemos protótipos de alta fidelidade realistas e de acordo com os padrões dos fabricantes.

### Referências:

BARBOSA, S. D. J. et al. **Interação humano-computador e experiência do usuário**. [S.l.]: Edição da autora, 2021. _E-book_.

BUXTON, B. **Sketching user experiences**: getting the design right and the right design. San Francisco: Morgan Kaufmann, 2007.

CHUEKE, J. **Perceptible affordances and feedforward for gestural interfaces**: assessing effectiveness of gesture acquisition with unfamiliar interactions. 2016. Disponível em: [http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556](http://ethos.bl.uk/OrderDetails.do?did=3&uin=uk.bl.ethos.697556). Acesso em: 3 nov. 2022.

DIX, A.; FINLAY, J.; ABOWD, G. **Human-computer interaction**. 3. ed. Essex, England: Parsons Education Ltd., 2004.

GARRETT, J. **The elements of user experience**: user-centered design for the web. New York: New Riders, 2003.

HOOBER, S.; BERKMAN, E. **Designing mobile interfaces**: patterns for interaction design. Sebastopol, CA: O’Reilly Media, 2011.

KOTRUM, P. **HCI beyond the GUI**: design for haptic, speech, olfactory, and other nontraditional interfaces. Burlington, MA: Elsevier, 2008.

KRUG, S. **Não me faça pensar!**: uma abordagem de bom senso à usabilidade mobile e na web. 2. ed. Rio de Janeiro: Alta Books, 2015.

MCELROY, K. **Prototyping for designers**. Sebastopol, CA: O’Reilly Media, 2017.

NIELSEN, J.; LORANGER, L. **Usabilidade na web**: projetando websites com qualidade. Rio de Janeiro: Campus Elsevier, 2007.

NORMAN, D. A. **Affordance, conventions and design.** Interactions, v. 6, n. 3, maio/jun., p. 38-43, 1999.

NORMAN, D. **The design of everyday things**. New York: Basic Books, 1988.

ROGERS, Y.; SHARP, H.; PREECE, J. **Design de interação**: além da interação humano-computador. 3. ed. Porto Alegre: Bookman, 2013.

STICKDORN, M. **This is service design doing**: applying service design thinking in the real world. Sebastopol, CA: O’Reilly, 2018.

TIDWELL, J. **Designing interfaces**: patterns for effective interaction design. Sebastopol: O’Reilly Media, 2010.

WIGDOR, D.; WIXTON, D. **Brave NUI world**: designing natural user interfaces for touch and gesture. Burlington, MA: Morgan Kaufmann, 2015.

WROBLEWSKI, L. **Mobile first**. New York: A Book Apart, 2011.

# Desenvolvimento Front-End  Avançado (Disciplina 2)

##  Primeiros passos no desenvolvimento front-end (Aula 1)

### Entendendo o front-end

Uma página _web_ pode ser dividida em três partes: **estrutura, estilo** e **comportamento**. Existem três tecnologias base para a implementação dessas partes:

#### HTML
É uma linguagem de marcação responsável pela forma de apresentar os conteúdos de maneira estruturada e lógica, mesclando textos com _tags_.

#### CSS
É uma linguagem de folhas de estilos utilizada para definir como os documentos escritos na linguagem HTML devem ser apresentados em termos de _layout_.

#### JavaScript
É uma linguagem de programação responsável por manipular comportamentos de páginas _web_.

Os navegadores são capazes de interpretar um documento HTML e combiná-lo com as suas informações de estilo definidas no CSS. Para isso acontecer, os navegadores carregam o HTML e o convertem para uma interface que representará como esses documentos devem ser lidos pelos navegadores. Chamamos essa interface de DOM (_Document Object Model_ – modelo de documento por objetos).

O DOM fornece uma representação estruturada do documento, possibilitando que os programas alterem sua estrutura, estilo e conteúdo. O documento é representado como se fosse uma espécie de árvore com galhos, que chamamos de “nós”.

A imagem a seguir mostra como um documento pode ser representado na árvore do DOM.

![[STB02 5.png]]

Com essa representação criada, o navegador fará a requisição da maioria dos recursos que estão linkados no documento, inclusive a folha de estilo que foi definida.  
  
O navegador analisa o CSS encontrado, interpreta as regras que foram criadas por meio dos seletores, inserindo e anexando essas regras de estilo para cada nó no DOM. Após o estilo ser aplicado para cada elemento, a visualização da página é exibida na tela.

#### Temos uma página com estrutura e estilo, mas como a interatividade pode ser adicionada?

O JavaScript, que é uma linguagem de programação, utiliza o DOM para acessar e manipular os elementos de um documento.

O DOM permite que as páginas sejam alteradas sem que haja a necessidade de atualização, possibilitando mover, arrastar, adicionar, alterar e remover elementos dentro de uma página, bem como alterar os estilos e criar efeitos CSS.

### Entendendo o modelo de documentos do objeto
![[Pasted image 20241017172232.png]]
![[Pasted image 20241017172246.png]]
![[Pasted image 20241017172258.png]]
![[Pasted image 20241017172320.png]]
![[Pasted image 20241017172400.png]]
![[Pasted image 20241017172532.png]]
![[Pasted image 20241017172643.png]]
![[Pasted image 20241017172619.png]]
![[Pasted image 20241017172819.png]]
![[Pasted image 20241017173121.png]]
![[Pasted image 20241017173150.png]]
![[Pasted image 20241017173526.png]]
![[Pasted image 20241017173619.png]]
![[Pasted image 20241017173629.png]]
![[Pasted image 20241017173648.png]]
![[Pasted image 20241017173658.png]]
![[Pasted image 20241017173710.png]]

Ao longo do tempo, as linguagens base de desenvolvimento _web_ tiveram várias atualizações, de modo a facilitar o desenvolvimento e resolver problemas encontrados nas versões anteriores.

![[STB03 4.png]]

O CSS 3 possibilita a criação de um sistema mais atrativo, rápido, com menos consumo de memória, além de demorar menos tempo para ser desenvolvido. Essa versão suporta o _design_ responsivo de sistemas, ou seja, quando um sistema é capaz de adaptar o tamanho das suas páginas de acordo com o tamanho das telas que estão sendo exibidas.

A versão mais atual do JavaScript é a [ES2022](https://exploringjs.com/impatient-js/ch_new-javascript-features.html), que trouxe funcionalidades como o método .at(), que permite interagir com índices de _arrays_ e _strings_ a partir do final, e a declaração de atributos e métodos privados das classes.  

Porém, vale destacar a [ES2015](https://262.ecma-international.org/6.0/) (popularmente conhecida como ES6), pois por muito tempo o JavaScript não recebeu atualizações, e a versão lançada em 2015 trouxe inúmeras funcionalidades que marcaram um avanço importante na linguagem (como _constants, operador spread, template literals, arrow functions_, parâmetros _default_, etc.).

### _Frameworks_ e bibliotecas para o desenvolvimento _front-end_

O desenvolvimento de interfaces requer o uso de diversos recursos, entre eles os _frameworks_ e as bibliotecas. É importante que entendamos para que cada um deles serve e os usemos de forma adequada. Caso contrário, podemos acabar nos encurralando de um ponto de vista de engenharia de _software_ e tendo que realizar uma quantidade significativa de retrabalho.

Em geral, _frameworks_ nos ajudam a estruturar nossas aplicações. Esse seria o caso de algo como o [Angular](https://angular.io/), que modifica a forma como desenvolvemos interfaces nos fazendo focar puramente em JavaScript e CSS, ao mesmo tempo que faz toda a integração de bibliotecas utilizadas no sistema.

Dessa forma, o uso de múltiplos _frameworks_ simultaneamente pode não ser possível, dada a possibilidade de incompatibilidade entre suas regras e comportamentos, mas o uso de diferentes bibliotecas pode ser. Tudo depende das bibliotecas sendo consideradas e de como elas são integradas no sistema em geral.

Assim como _frameworks_, algumas bibliotecas também podem impor sua própria lógica que limita sua compatibilidade com outras bibliotecas. Esse seria o caso do React e do Vue, que são bibliotecas, mas que modificam a forma da implementação do _front-end_, impondo sua lógica componentizada. Assim, elas podem limitar quais bibliotecas podemos eventualmente usar.

Ao se basearem no uso componentes implementados inteiramente em JavaScript e que são eventualmente traduzidos em HTML, essas bibliotecas, assim como o Angular, permitem que foquemos nossa implementação inteiramente no JavaScript.  
  

Entretanto, esta não é a norma quando discutimos bibliotecas. A maioria delas é autocontida e não impõe uma lógica de implementação maior no resto da aplicação. Assim, podem ser utilizadas conforme o necessário, sem problemas de compatibilidade com outros recursos.

![[STB04 4.png]]

Hoje, alguns dos _frameworks_ e bibliotecas mais importantes para desenvolvimento _web_ são aqueles que permitem desenvolvimento de aplicações puramente em JavaScript. Eles permitem que escrevamos nosso código em JavaScript, seguindo seus padrões, e depois o interpretam para gerar o HTML, o JavaScript e o CSS resultantes que vão sustentar nossa aplicação. Esse é o caso de Angular, [Vue](https://vuejs.org/) e React, que vamos ver mais à frente. Nosso objetivo geral, ao utilizá-los, é conseguir focar exclusivamente em JavaScript, sem ter que lidar com HTML.

Uma das características mais interessantes dos _frameworks_ e das bibliotecas mencionados é o quanto eles facilitam o desenvolvimento de SPAs (_single page applications_, ou aplicações de página única). Como o nome já indica, estas são aplicações compostas por apenas uma página _web_. Em vez de ter que trocar de páginas, fazendo solicitações ao servidor que alimenta o conteúdo _web_, essa página única simplesmente muda a sua estrutura de forma dinâmica em tempo de uso, por meio do JavaScript. Fica responsável por modificar o código HTML e CSS no _browser_, modificando a página sendo exibida. Dessa forma, reduzimos a quantidade de chamadas ao servidor de _front-end_ e mantemos a lógica e a dinamicidade da aplicação dentro dos _browsers_ de nossos usuários.

Muitos _frameworks_ e algumas bibliotecas, como React, Angular e Vue, se utilizam de diferentes notações similares a HTML para permitir que desenvolvedores consigam definir as _tags_ que deverão ser incluídas no DOM de dentro do próprio JavaScript. Um exemplo é a JSX, utilizada dentro do React para que nós possamos definir as _tags_ HTML que serão utilizados nos componentes que construímos. Assim, podemos definir e alterar nosso código HTML de dentro do nosso próprio código JavaScript, permitindo a construção de SPAs.

![[Pasted image 20241017175514.png]]
![[Pasted image 20241017175533.png]]
![[Pasted image 20241017175619.png]]
![[Pasted image 20241017175656.png]]
![[Pasted image 20241017175726.png]]

Vamos agora analisar alguns dos _frameworks_ e bibliotecas mais utilizados para o desenvolvimento _web_ atualmente: Angular, React e Vue.

![[stb07 5.png]]

### Trazendo para a prática

Durante o desenvolvimento, estamos constantemente testando versões do nosso código em HTML, JavaScript e CSS visualizando-o em nossos _browsers_ locais. Já nesse nível podemos considerá-los como ferramentas de desenvolvimento. Já foi pensando nesse papel que desenvolvedores de _browsers_ criaram uma série de funcionalidades para ajudar no desenvolvimento _web_. Há uma variedade entre diferentes versões (Edge, Firefox, Chrome, Safari, etc.), mas existe um conjunto que costuma estar presentes em todos os _browsers_.

#### Inspecionando elementos

A primeira funcionalidade que vamos analisar é o inspetor de elementos. Ela permite que analisemos o código HTML que é renderizado no _browser_. Podemos passar pelas diferentes _tags_ identificando em que parte da tela elas aparecem. Esse processo ganha ainda mais importância quando usamos bibliotecas de _front-end_ que utilizam componentes pré-feitos. Nesses casos, não sabemos necessariamente quais são as classes e os tipos de objetos utilizados para construir esses componentes. Caso queiramos modificá-los, precisamos primeiro identificar esses elementos e classes e depois alterar o código, ocasionalmente sobrescrevendo os comandos da biblioteca utilizada.

![[STB08 5.png]]

A imagem apresenta a visão do inspecionador de elementos. Nela observamos o HTML que está sendo renderizado pelo _browser_. Vale observar que esse HTML é dinâmico e que seu conteúdo poderá ser alterado a cada nova interação com a página. Quando uma interação do usuário dispara uma alteração no HTML, o inspecionador de elementos geralmente dá um destaque visual sob o elemento alterado.

#### O console

A segunda funcionalidade essencial para um desenvolvedor _web_ é o console. Nele conseguimos observar mensagens de erro e avisos do _browser_ sobre como o código JavaScript está rodando. Temos que lembrar que nosso código de _front-end_ sempre será compilado em um _browser_, não podendo ser facilmente testado no próprio IDE utilizado. Portanto, identificar a fonte de diversos problemas requer um uso eficiente do console. Ao longo do desenvolvimento pode haver diversos momentos em que queremos utilizar o comando “console.log()” para examinar algum elemento do código JavaScript.

![[STB09 4.png]]

Na imagem, temos uma visão do console que exibe mensagens de erros, destaques em vermelho, e mensagens de _warnings_ (alertas), destaques em amarelo. Essas mensagens são registros de _logs_ que foram disparadas durante o processo de construção do HTML renderizado pelo _browser_.

O console.log() vai ser extremamente útil para visualizar mensagens de _debug_. Um exemplo de utilização seria, após o login feito com sucesso, utilizar o comando console.log('Usuário %s logado com sucesso!', usuario.nome) para exibir no console o resultado de sucesso. Você também poderia utilizar o console.info(), para exibir outras informações; o console.debug(), para especificar mensagens de _debug_; o console.warn(), para criar mensagens de alerta; e o console.error(), para mensagens de erro.

#### _Debugging_ de JavaScript

Outra forma de examinar o funcionamento do código JS que está rodando em nossos _browsers_ é usando o _debugger_. Nele temos funcionalidades de _debugging_ similares às que teríamos em um IDE tradicional. Podemos criar pontos de parada e examinar variáveis, entre diversos outros aspectos do código, a fim de identificar a fonte de problemas ou comportamentos inesperados. Usado em conjunto com o console, o _debugger_ completa um conjunto de ferramentas que nos permite identificar os _bugs_ de nosso código JS de _front-end_.

![[02 25.png]]

Uma curiosidade: como todo e qualquer código JavaScript utilizado nesse processo será apresentado aqui, é comum o uso de ferramentas para “ofuscar” o código JavaScript para prejudicar a sua legibilidade e, assim, tentar evitar a reprodução do mesmo JavaScript por terceiros.

Também há ferramentas que fazem algo parecido, mas com o objetivo de compactar o código, reduzir o tamanho do código final. Nesse caso, o objetivo é reduzir o tamanho final da resposta do servidor, o que pode representar redução no tempo de resposta. Quanto menor for o tamanho da resposta, menor será o número e o tamanho das requisições necessárias para construir a página final.

#### Inspecionando as requisições

Indo além do código que roda no _browser_ local, também devemos considerar como nossa aplicação _web_ se comunica com outros recursos, como APIs. Para esse fim, _browsers_ costumam disponibilizar uma aba Network (rede) que visualiza quaisquer chamadas feitas a recursos externos. Nela podemos ver a chamada em si, como foi estruturada e qual era o seu conteúdo visível (algumas informações podem estar ocultas, como no caso de chamadas POST), além das respostas recebidas pelo _browser_.

![[stb11 5.png]]

Como exibido na imagem, na aba Network (ou rede) podemos visualizar e acessar o conteúdo de todas as requisições feitas pelo _browser_, que são chamadas feitas pela página durante o seu processo de construção.

Mediante uma análise cuidadosa dessas chamadas, devemos conseguir identificar quaisquer problemas com a forma como estruturamos esses pedidos a recursos externos e fazer as correções necessárias. **Se tivermos acesso ao _back-end_, podemos observar os _logs_ do servidor e ter um entendimento ainda melhor de como a comunicação com o _front_ se encaixa com o funcionamento interno do _back_.**

Esse tópico será discutido em mais detalhes na nossa terceira aula, na qual vamos trabalhar esse processo de comunicação entre _front-end_ e _back-end_.

#### Considerações finais sobre as ferramentas de inspeção

Dadas essas diversas funcionalidades que costumam estar presentes em _browsers_, podemos observar a importância que eles têm para o desenvolvimento _web_. **Como códigos de interface precisam ser compilados nessas aplicações, sem essas informações disponibilizadas não haveria como examinarmos o funcionamento de nossa aplicação**. Ao mesmo tempo, não é nos _browsers_ que escrevemos nosso código e passamos para o servidor de _front-end_, e sim no IDE.

Temos, então, um processo dividido. Escrevemos nosso código em IDEs e examinamos seu funcionamento em _browsers_. **Podemos nos perguntar então: como podemos utilizar essas duas ferramentas de forma a facilitar nosso desenvolvimento? Como conseguimos deixar pistas no código que escrevemos em nossos IDEs que podem ser captadas em nossos _browsers_? Como podemos utilizar os _browsers_ para achar os erros na aplicação para consertá-los no IDE?**

Essa é uma busca constante de desenvolvedores de _front-end_, que, ao ficarem cientes da importância desse uso conjunto, desenvolvem suas próprias estratégias e estilos para fazer um uso apropriado das duas ferramentas. Ao longo de nossas aulas, especialmente as discutindo técnicas aplicadas, vamos mencionar algumas dessas possíveis estratégias.  
  

Dadas as funcionalidades presentes em _browsers_ para permitir que inspecionemos como nossas interfaces estão rodando na prática, torna-se importante que os desenvolvedores saibam tirar o máximo dessas funcionalidades. **Em primeiro lugar, temos a possibilidade de usar o _log_ do console para externalizar o valor de variáveis em tempo de execução. Durante nosso desenvolvimento, nem sempre saberemos os valores assumidos pelas variáveis por trás de nossas interfaces.**

Utilizar o comando _console.log_() dentro de nosso código JavaScript permite que esses valores sejam imprimidos no console. Com um bom uso dessa funcionalidade, torna-se possível identificar pontos problemáticos de forma eficiente. Um dos problemas mais encontrados em aplicações que utilizam JavaScript é a possibilidade de nossas variáveis assumirem um valor _undefined_. Isso se dá tanto por erros no nosso próprio código quanto pelos entendimentos errôneos sobre como as bibliotecas que utilizamos funcionam.

A fim de identificar quais variáveis podem ter valores problemáticos, precisamos observar com cuidado as mensagens de erro que são imprimidas no console:  
- Usando o trace de erros, podemos ver onde em nosso código esses erros começam.
- A partir desse ponto, podemos passar a imprimir os valores das variáveis no console a fim de investigá-las.  

Além do uso do console, a própria forma como estruturamos o nosso código pode facilitar a nossa identificação de problemas. Quando discutimos questões visuais da interface, não conseguimos imprimir nos consoles os próprios elementos renderizados no DOM.  
  

Nesses casos, precisamos ter outra forma de identificar os elementos que não estão funcionando. Para isso, podemos nos aproveitar do campo de ID de elementos HTML, além de suas classes CSS, para rapidamente identificar a _tag_ que queremos investigar na aba Elements de nossos _browsers_.

O que há de comum entre essas estratégias é a antecipação que poderemos utilizar nos mecanismos dos _browsers_ para nos auxiliar durante o desenvolvimento. Uma implementação às cegas pode levar a retrabalho e um processo mais complexo de identificação de _bugs_. Sempre devemos ter todas as ferramentas à nossa disposição em mente quando desenvolvemos novas interfaces.

Estas são apenas algumas das estratégias existentes para aproveitar ao máximo as funcionalidades dos _browsers_ durante o nosso processo de desenvolvimento.

É importante frisar que diferentes bibliotecas têm diferentes lógicas de funcionamento e, portanto, podem se beneficiar de estratégias mais específicas de identificação de problemas no código.

De qualquer forma, essas estratégias terão de depender das ferramentas dos _browsers_ para conseguirmos externalizar os valores de variáveis em tempo de execução.

### Técnica aplicada

Agora chegou a hora de colocar em prática um pouco do que discutimos. Na técnica aplicada, vamos apresentar um código de uma proposta de front-end para um sistema de vendas feito utilizando HTML, CSS e JavaScript. Essa proposta será no estilo SPA e ilustrará o desenvolvimento de uma pequena aplicação front-end.

Vamos explorar como criar a estrutura da página, introduzindo estilos aos componentes e interatividade à aplicação. A imagem a seguir representa o protótipo da aplicação, que consiste em um sistema _web_ de página única que possibilita compras com um clique.

![[stb12 3.png]]

O nosso objetivo é implementar um sistema com as três linguagens bases do _front-end_, realizando a comunicação entre os arquivos de maneira que o _site_ seja estruturado, estilizado e interativo. Para o desenvolvimento do código, utilizaremos o Visual Studio [Code](https://code.visualstudio.com/) como o IDE e apresentaremos no _browser_ Firefox. Mas, claro, você pode utilizar o IDE e o _browser_ que preferir.  
  

Para melhor contextualização, esse _front-end_ será feito para que possa ser integrado futuramente a uma API que tratará toda a lógica de negócios do sistema. Na figura, veja um retrato dessa arquitetura em três camadas. Nas próximas aulas, vamos continuar o desenvolvimento desse _front_, e na última aula vamos focar na integração do _front-end_ a uma API.

![[01 1 4.png]]
![[Pasted image 20241024163158.png]]

### Referências:

ECMA INTERNATIONAL. **Standard ECMA-262**. 6. ed. [_S.l._], 2015. Disponível em: [https://262.ecma-international.org/6.0/](https://262.ecma-international.org/6.0/). Acesso em: 29 dez. 2022.  
  
RAUSCHMAYER, A. **JavaScript for impatient programmers**. [_S.l._]: Independently Published, 2019.

## Programando com React (Aula 2)

Com o passar dos anos, as interfaces _web_ têm ficado cada vez mais complexas, demandando novas e criativas estratégias para suas implementações. **Um dos maiores desenvolvimentos nos últimos anos na arquitetura desses sistemas foi a noção de componentes.**

![[Pasted image 20241024165742.png]]
![[Pasted image 20241024165804.png]]
![[Pasted image 20241024165824.png]]
![[Pasted image 20241024165845.png]]
![[Pasted image 20241024165907.png]]

Nesta aula, vamos discutir os principais conceitos que devemos ter em mente ao desenvolver componentes de interface, discutir a relação da estrutura de componentes e programação orientada a objeto e, por fim, comparar o código de uma interface implementada com e sem componentização, a fim de ilustrar a importância de estruturar nosso código de interface de forma modularizada e reutilizável.

### Componentização da aplicação

Antes de começarmos a discutir como implementar interfaces componentizadas, precisamos primeiro entender o que é um componente.

Componentes são pedaços de código modularizados que podem ser utilizados em diferentes contextos. Em termos de escopo, eles podem ir desde as funções mais básicas e pequenas até as mais complexas.

Em sua essência, utilizamos a estrutura de componentes para evitar retrabalho. Em vez de ter que reimplementar um pedaço de nosso código para cada contexto minimamente diferente, podemos construir um único artefato que pode ser instanciado de forma diferenciada de acordo com o contexto no qual ele existe. Ou seja, passando os parâmetros para esse elemento, seu comportamento se adapta.

Dada a existência de interações mais complexas, que podem depender de múltiplas partes e funcionalidades de nossos sistemas, há também a importância de pensar em como nossos componentes podem ser utilizados de forma conjunta.  
  

Entenda melhor a seguir:

![[stb02 1 2.png]]

Em termos dessa compatibilidade, um dos aspectos essenciais que devemos ter em mente é a questão do fluxo de informações. Em geral, bibliotecas e _frameworks_ tendem a se preocupar com o escopo das informações dentro de nossos sistemas, restringindo as formas como componentes podem passar esses dados de uns para os outros. É importante saber utilizar esses mecanismos de forma eficiente, evitando passar informações desnecessárias entre componentes e fazendo um bom controle de quais deles podem modificar uma informação específica.

### Os pilares da programação com o React

A programação com o uso de componentes versáteis e dinâmicas depende de uma série de conceitos centrais ao seu funcionamento. Estados e relações de parentesco entre componentes são apenas alguns dos tópicos que vamos explorar em nosso primeiro vídeo, se preparando para uma discussão mais aprofundada de como esses fundamentos são aproveitados na prática em nosso desenvolvimento de interfaces.

#### A separação de responsabilidades na prática

Neste vídeo, vamos explorar, a partir de casos de estudo, o papel da componentização no desenvolvimento de interfaces _web_. Com foco no React, serão apresentadas as diferentes formas de criação/definição de um componente e suas implicações. Também vamos além, explorando como se definem relacionamentos entre componentes e como tirar proveito desses relacionamentos.  
  

Nesse ponto, vamos explorar estados e propriedades de um componente, algo que vai ajudar a entender o ciclo de vida de um componente.

![[Pasted image 20241024172316.png]]
![[Pasted image 20241024172341.png]]
![[Pasted image 20241024172402.png]]
![[Pasted image 20241024172422.png]]
![[Pasted image 20241024172440.png]]
![[Pasted image 20241024172520.png]]
![[Pasted image 20241024172555.png]]
![[Pasted image 20241024172610.png]]
![[Pasted image 20241024172627.png]]

#### Renderização de componentes

Podemos considerar que os componentes são compostos de duas partes: sua parte visual, renderizada nos _browsers_ de nossos usuários, e sua parte funcional, com sua lógica de interação. Diferentes bibliotecas e _frameworks_ tratam a relação entre essas duas partes de forma diferenciada.

Vue e Angular, por exemplo, separam a parte lógica de seus componentes de sua parte visual. Já o React, que vamos explorar nesta aula, integra os dois em uma mesma classe ou função.

Como nossos componentes tendem a ser dinâmicos, modificando-se de acordo com nossas interações na interface, há a necessidade de eles serem renderizados múltiplas vezes. **Em relação a esse processo, uma das coisas que desenvolvedores _front-end_ devem saber sobre as bibliotecas e os _frameworks_ que utilizam é quais são os gatilhos para uma nova renderização.** Por exemplo, no caso de React, novas renderizações ocorrem toda vez que uma variável de estado do componente tem os seus valores modificados.

Essas renderizações diferenciadas dos componentes React também podem se basear em uma lógica condicional, ou seja, se for satisfeito um conjunto de critérios, o componente se renderiza de uma forma, se não, se renderiza de outra. Essa capacidade é essencial quando lidamos com componentes que importam os seus dados de uma fonte remota, por exemplo. No seu momento de inicialização no React, o componente ainda não teria as informações necessárias para carregar corretamente.

Assim, podemos denotar um estado inicial em que o _render_ não retorna nada. Uma vez carregados os dados, podemos passar a exibir as informações, caindo, então, em outra condição do processo de _render_. Este é apenas um dos exemplos em que o mecanismo de _render_ condicional se demonstra essencial.

Além de mudanças isoladas em componentes, temos também a questão do efeito cascata de renderizações. Quando um novo _render_ ocorre no componente pai, todos os componentes também são renderizados novamente. Ao se ter esse efeito em cascata, o fluxo de informação entre componentes também é combinado com as etapas da visualização da interface. Novamente, isso é algo que vale compreender bem como funciona nas ferramentas que utilizamos no desenvolvimento, pois podem variar.

Vamos agora discutir um pouco mais sobre o React e o seu uso de JSX, que permite que escrevamos um código XML em nossos arquivos JavaScript e que ele seja interpretado e transformado em HTML. Verifique a explicação abaixo:

![[Pasted image 20241024172916.png]]
![[Pasted image 20241024172944.png]]

**Além do uso de _tags_ de componentes React, outro mecanismo importante de JSX é a possibilidade de se adicionar código JavaScript dentro do próprio formato XML.** Isso se faz ao adicionar um bloco de código cercado por chaves “{...}”. Se o código JavaScript ali contido for uma função que retorne código JSX, este será integrado ao _script_ principal. Com esses mecanismos, nosso código JSX pode se tornar incrivelmente mais dinâmico.

Consideremos, então, o exemplo da instanciação de uma série de elementos com base em uma lista de dados. Em muitos casos, precisaremos pegar uma fonte de dados e instanciar componentes na interface de acordo com o que consta nela. Precisaremos de alguma forma de iterativamente montar nosso código JSX, já que isso terá que ser feito em tempo de execução. Podemos, então, mapear uma função à estrutura de dados que varre por seus elementos e retorna os componentes JSX equivalentes, aproveitando-se da propriedade do JSX que combina o retorno de funções no _script_ original. Nesse caso, vamos ver como ficaria um código similar:

![[stb04 1 1.png]]

Apesar de ser básico, esse exemplo ilustra a importância da integração de JSX com códigos JavaScript em geral. Permite uma execução iterativa e integra os seus resultados no _script_ original. Além desta, há infinitas possibilidades quanto ao que podemos realizar com essa execução dinâmica de JavaScript durante a renderização.

Qualquer função JavaScript que retorna um elemento JSX pode ser usada de forma equivalente. Além disso, declarações de funções também podem ser feitas usando essas chaves “{}” para que possamos defini-las e atribuí-las a _event listeners_ de elementos JSX diretamente.

#### Componentes dinâmicos

Como já mencionamos diversas vezes, nossos componentes costumam ser dinâmicos, ou seja, mudam de estado devido às interações de usuários com a interface, com o carregamento de dados externos ou outros gatilhos. O conceito principal que devemos levar em consideração em relação a essas alterações é o conceito de estado, que seria uma versão específica do componente.

Relembrando um pouco do que foi apresentado no primeiro vídeo, quando estamos desenvolvendo na prática, costumamos ter variáveis que estão atreladas a esses estados e influenciam o ciclo de vida do componente. **No caso do React, estas são chamadas de _state variables_ (variáveis de estado)**. Toda vez que os valores delas são alterados, o React considera que o componente mudou de estado, ativando, então, uma nova renderização dele.

No início do ciclo de vida do componente, temos um momento de inicialização, em que os valores iniciais dessas variáveis são atribuídos sem que tenhamos múltiplas renderizações. Após esse momento, quaisquer mudanças levam o componente a um novo estado.

Seguindo a linha de etapas especiais desses componentes, levando em consideração o exemplo do React, temos duas fases notáveis: o momento pré-renderização do componente e o momento logo após essa primeira visualização. Antigamente, estes eram referidos como componentWillMount e componentDidMount.

Atualmente, foram todos combinados dentro do guarda-chuva do _hook_ useEffect:  
- O momento componentWillMount costumava servir como um ponto ideal para o carregamento de dados para os componentes, antes que eles fossem visualizados. Assim que o componente fosse instanciado, o código relacionado seria rodado, e a visualização do componente esperaria sua conclusão.
- O momento componentDidMount ocorre logo após essa primeira renderização. Esse momento costumava ser útil para verificar se todas as informações foram carregadas corretamente ou fazer quaisquer processamentos iniciais que não deveriam travar a renderização do componente.  

Recentemente, o React mudou e permite utilizar apenas o _hook_ chamado useEffect, porém, antes de discuti-lo, precisamos falar sobre o que são _hooks_. Em primeiro lugar, _hooks_ são funcionalidades que podem ser adicionadas a componentes de forma opcional. Entre outras funcionalidades que são tratadas como _hooks_, podemos destacar as variáveis de estado.

Apenas quando utilizamos a função useState() é que avisamos para o interpretador do React que ele precisa se preocupar com a manutenção dos estados daquele componente. Caso contrário, não se presta atenção nesse aspecto do componente.

O useEffect é utilizado para declarar que há algum processamento assíncrono que deve ser feito de acordo com a mudança de um conjunto de variáveis. Ele é considerado efeito adicional à lógica principal do componente. Por _default_, todo protocolo instanciado no useEffect roda toda vez que o componente for renderizado, porém isso pode ser modificado, como veremos adiante.

Uma vez que só roda após a renderização, a utilização de useEffects praticamente elimina a noção de componentWillMount que existia antigamente, forçando que todo componente lide com uma primeira renderização antes da chegada de dados de fontes externas.

Uma forma de lidar com isso seria por meio do uso de um _render_ condicional, em que o primeiro caso seria quando os dados ainda não chegaram (caso em que se retornaria um elemento vazio, por exemplo), e outro, uma vez que os dados estivessem presentes.

Além dessa execução uma vez que o componente seja renderizado, podemos ter também a necessidade de ter efeitos rodando de forma assíncrona quando certas variáveis mudam de valor. Para isso, a função useEffect tem um segundo parâmetro que define quais variáveis determinam quando esse efeito é ativado. Ou seja, se o valor delas mudar, o efeito é rodado. Para que um efeito rode apenas uma vez quando o componente for renderizado, basta passar uma lista vazia nesse segundo parâmetro.  
  
Veja mais sobre o useEffect:

![[01 3 3.png]]
![[02 1 3.png]]
![[03 11.png]]

#### Fluxo de informação e arquitetura

Como já comentamos, componentes são estruturados de forma hierárquica. Componentes são pais de outros componentes, e por aí vai. Além de os filhos ficarem “dentro” dos pais no HTML resultante, outro aspecto crucial desse relacionamento é o fluxo de informações e controle de um sobre o outro.

Em geral, pais passam informações para os seus filhos diretamente. No caso do React, isso ocorre por meio do que chamamos de “props” (propriedades). Ao instanciarmos um componente no JSX, podemos passar parâmetros para esse componente da mesma forma como definimos parâmetros em HTML.

Uma vez passado pelos pais, no JSX, o componente filho precisa recuperar essas informações por meio do elemento props que fica disponível dentro do escopo interno do componente. Podemos ver um exemplo disso nas imagens a seguir:

![[stb06 4.png]]

Apesar de não ser padrão, há também formas de passar controle aos componentes filhos sobre as informações de seus pais. Por exemplo, quando temos um pedaço de informação que deveria ser alterado por dois componentes, devemos passar essa variável para o pai em comum dos dois.

Uma vez localizada a variável nesse componente, podemos passar para os filhos uma referência de função que permite alterar esse valor. Ao chegar aos componentes filhos, basta fazer uma chamada dessa função que o valor no componente pai será alterado.

Por um lado, esse é um mecanismo importante para conseguirmos ter informações compartilhadas entre componentes dentro do próprio React, mas isso deve ser usado com cautela.

Ao propagarmos a função que altera esse valor, damos mais autonomia para os componentes filhos, para o bem e para o mal. Se muitos tiverem esse acesso, eventuais erros no sistema causados por valores estranhos na variável em questão podem se tornar mais difíceis de resolver.

Para termos um desenvolvimento _front-end_ e uma aplicação mais robusta e organizada, temos que entender os escopos de cada pedaço de informação no nosso sistema. Assim, podemos evitar a propagação excessiva dessas propriedades e das funções que as alteram. Temos que saber onde dados de fontes externas são carregados, quem pode precisar deles, entre diversas outras dinâmicas.

Temos que balancear o incentivo a fazer poucas requisições para um _back-end_ e propagar essas informações pelo próprio _front-end_, com a complexidade que essas transmissões de informações podem ter. Como sempre, é necessário um olhar atento para o caso em que nos situamos.

### Como implantar componentes

Como vimos, componentes são uma parte importante da implementação organizada de interfaces reativas. Mas como as implementamos de fato? Componentes são pedaços modularizados da interface, com suas diferentes informações e funcionalidades.

Traçando paralelos com a engenharia de _software_, podemos logo notar as similaridades com a programação orientada a objeto, em que todo o nosso código é estruturado em classes que interagem umas com as outras. Eliminamos _scripts_ isolados. Tudo deve acontecer dentro de um objeto ou classe.

Assim, as similaridades entre os componentes de interface e as classes da engenharia de _software_ são muito grandes. De fato, muitas bibliotecas e arcabouços implementam os componentes como classes de JavaScript, utilizando-se de suas propriedades para auxiliar a implementação de _front-end_.

Por exemplo, uma propriedade importante de classes é a possibilidade de certas classes estenderem outras. A classe de extensão herda as variáveis e funcionalidades definidas da classe original, além de quaisquer outras que forem implementadas na nova classe.

O mesmo pode acontecer com componentes. Se tivermos versões mais específicas de outros componentes, podemos construir novas classes para estendê-las aproveitando-se da própria herança de comportamentos que o JavaScript implementa na sua lógica de programação orientada a objeto.

Esta é apenas uma das propriedades das classes de JavaScript que podem ser aproveitadas para a implementação de componentes. Construtores, métodos e propriedades estáticas, etc., todos podem ter suas próprias implicações para o desenvolvimento de _front-end_. **Portanto, ao descobrir essas mecânicas de classes, podemos sempre pensar: como utilizar isso na implementação de componentes?**

Falando mais especificamente do caso do React, vimos que componentes podem ser implementados tanto como funções quanto como classes JavaScript. Nesse segundo caso, a biblioteca se utiliza de alguns processos centrais às classes para também auxiliar na gestão de informações e estados nos componentes reativos.

Vale a pena discutirmos esses mecanismos e verificarmos quais são as vantagens e as desvantagens de optar pela implementação na forma de classes em vez de implementá-las como funções.

A primeira característica que o React utiliza de classes de JavaScript é a questão da herança entre classes. Toda vez que queremos criar um componente como uma classe, precisamos afirmar que essa nova instância estende a classe “React.Component” ou alguma outra classe que tem ela em sua cadeia de heranças. Além de ter um construtor que nos permite trabalhar com as propriedades do componente, ela também tem uma série de métodos que habilitam muitas mecânicas do React, como a questão de _lifecycle_.  
  

O construtor dessa classe permite que instanciemos esses componentes em nosso sistema e passemos parâmetros, que, no caso do React, são chamados de “propriedades”, que permitem que customizemos as instâncias. Na prática, isso costuma acontecer dentro do próprio JSX. Quando colocamos _tags_ relacionadas aos componentes que criamos e definimos esses parâmetros, o React interpretará essa _tag_ como uma chamada para a instanciação de uma nova classe desse componente utilizando os atributos definidos na _tag_ como as propriedades.  
  

Essa costuma ser a principal forma de comunicação de dados entre esses elementos. Componentes pais instanciam componentes filhos e passam informações como props por meio dos atributos nas _tags_.

Além do processo de construção da instância do componente, temos também o método de _render_, que nos permite visualizar esse elemento da interface. Quando criamos um componente como uma classe, temos que definir essa função para que o interpretador saiba o que deve ser gerado como HTML e CSS. Como mencionamos, a função de _render_ também tem o fim duplo de instanciar componentes filhos, quando adicionamos suas _tags_ no código JSX.

Como queremos construir interfaces dinâmicas, que se ajustam de acordo com a interação e as informações que passam pelo sistema, teremos que frequentemente lidar com eventos.

Para o React, costumamos atribuir funções para lidar com elementos nas _tags_ de componentes que definimos no JSX.

Porém, quando temos métodos customizados dentro da própria classe, teremos um passo adicional de ter que _bind_ esses métodos dentro do construtor. Isso se deve a uma necessidade de classes de JavaScript para que esses métodos fiquem disponíveis no momento da instanciação.  
  
Observe a seguir:

![[stb07 1 2.png]]

Esse trabalho adicional é uma das pequenas dificuldades de se trabalhar com React usando classes, mas pode ser superado com o uso de uma sintaxe um pouco diferente. Se, em vez de definirmos métodos da forma tradicional, nós os definirmos como _arrow functions_, elas já serão automaticamente disponíveis na classe, uma vez que são tratadas como variáveis, recebendo tratamento diferenciado. Nesses casos, os métodos estariam sempre disponíveis, e não haveria a necessidade de se fazer o _bind_ dentro do construtor.

Veja, a seguir, um bom exemplo de que entender o funcionamento de classes dentro de JavaScript pode facilitar nosso desenvolvimento:

![[stb08 1 1.png]]

Outra característica de classes é o modo como elas isolam seus métodos internos. Componentes React têm uma dinâmica similar quando falamos de variáveis de estado, cujos valores só podem ser alterados dentro de suas próprias classes originais. No entanto, pode haver situações em que queremos que componentes filhos modifiquem o estado de seus pais.

Nessas situações, temos que passar funções que modifiquem esse valor para os componentes filhos por meio de suas propriedades, quando os instanciamos no JSX. Essa é uma lógica geral; o controle flui de cima para baixo na hierarquia de componentes.

Levando em consideração todas essas dinâmicas da implementação de componentes React como classes JavaScript, podemos observar a importância de analisar como as dinâmicas dessas estruturas de código podem influenciar nosso desenvolvimento de _front-end_. Assim, temos que sempre levar em consideração a seguinte pergunta: como as dinâmicas de classes JS são traduzidas para o desenvolvimento com React e em quais contextos eu deveria optar pela outra forma de criação de componentes como funções?

### Técnica Aplicada

Após estudarmos todos esses conceitos de implementação reativa focando no React, temos uma boa noção de alguns dos processos com os quais precisamos nos preocupar. Mas como podemos começar nossos projetos? Como criamos uma aplicação React do zero? Essa é uma das questões que vamos explorar agora, indo passo a passo para a construção e _deploy_ de um novo projeto.

Em outros casos, não precisamos construir projetos novos, mas convertê-los em um _site_ já existente, reimplementando-o em React. Entre várias questões, teremos que decidir quais serão os componentes criados, como flui a informação, etc.

Para isso, o vídeo a seguir explora as diferenças entre implementar um **código com e sem React, demonstrando algumas das questões de conversão entre os dois paradigmas.**

Começar um novo projeto React não envolve apenas a biblioteca em si.

Como vimos na aula 1, bibliotecas não se sustentam por si só, exigindo o uso adicional de outras ferramentas, como Node e Webpack. **Precisamos, então, estruturar nosso projeto na mão, juntando todas essas partes?**

Felizmente, temos à disposição uma ferramenta chamada [create-react-app](https://create-react-app.dev/), que está disponível como um pacote Node. Ela permite que criemos um projeto React em um único comando.  

Curiosamente, esse pacote independe de instalação específica, já que faz uso do NPX, que permite a execução direta de pacotes, instalando-os se necessário. Vamos ver na imagem como isso acontece:

![[stb09 1 1.png]]

#### Aplicação

Agora que sabemos como construir uma nova aplicação React, vamos analisar um caso de desenvolvimento em que modificamos a aplicação descrita na aula 1 para usar React. Nosso objetivo: **facilitar o nosso desenvolvimento e criar um site mais robusto**. Todo nosso processo é explicado em detalhes no vídeo a seguir.

#### Com e sem o uso da componentização

Neste vídeo, vamos explorar o desenvolvimento _front-end_ com o React aproveitando o exemplo prático da aula anterior. Aqui, o objetivo é ilustrar os efeitos do uso da componentização no desenvolvimento de uma aplicação _web_. A melhor forma de fazer isso é comparando o desenvolvimento com e sem o uso do React. Como na técnica aplicada da primeira aula o desenvolvimento foi sem o React, com o conteúdo deste vídeo você vai poder comparar na prática a diferença entre os dois cenários.

![[Pasted image 20241025105224.png]]
![[Pasted image 20241025105249.png]]
![[Pasted image 20241025105303.png]]
![[Pasted image 20241025105324.png]]
![[Pasted image 20241025105346.png]]
![[Pasted image 20241025105417.png]]
![[Pasted image 20241025105431.png]]
![[Pasted image 20241025105447.png]]
![[Pasted image 20241025105458.png]]
![[Pasted image 20241025105510.png]]
![[Pasted image 20241025105522.png]]
![[Pasted image 20241025105533.png]]
![[Pasted image 20241025105808.png]]
![[Pasted image 20241025105823.png]]
![[Pasted image 20241025105833.png]]
![[Pasted image 20241025110306.png]]

### Referências:
BANKS, A. **Learning React:** modern patterns for developing react apps. 2. ed. [_S.l._]: O'Reilly Media, 2020.  
  
COMPONENTS and props. React, c2022. Disponível em: [https://reactjs.org/docs/components-and-props.html](https://reactjs.org/docs/components-and-props.html). Acesso em: 21 dez. 2022.  

REACT. Disponível em: [https://reactjs.org/](https://reactjs.org/). Acesso em: 21 dez. 2022.

## Integração com o _back-end_ e publicação (Aula 3)

Nas últimas duas aulas exploramos na teoria e na prática os conceitos necessários para o desenvolvimento de interfaces _web_ modernas e iterativas, tudo isso com o objetivo de servir ao cliente a melhor experiência possível para o nosso usuário final.  

Como comentamos nas aulas anteriores, o _front-end_ é a nossa camada de comunicação, responsável pela interação dos usuários com o sistema. Nesse cenário, o “sistema” abstrai toda a lógica necessária implementada para atender às necessidades do usuário. Comumente, chamamos esse outro lado de _back-end_. Em um contexto mais amplo, o termo _back-end_ faz referência a toda parte que não é diretamente acessível pelo usuário de uma aplicação _web_. Nela temos a execução da lógica de negócio, além da manipulação e da persistência dos dados.

![[stb1 3.png]]

Nesta terceira aula, vamos explorar as diferentes formas de comunicação entre _front-end_ e _back-end_, suas implicações e os desafios na implementação da comunicação assíncrona entre essas duas camadas. Também vamos relembrar um pouco a comunicação via protocolo HTTP.  

Ao final da aula, vamos discutir a publicação do _front-end_ (o _deploy_), a disponibilização da interface para o nosso usuário final.

### Processamento assíncrono e _promises_

Uma característica do JavaScript é que ele **é uma linguagem síncrona (_single-threaded_), ou seja, só executa um comando por vez**. Com isso, os outros comandos devem aguardar a execução em uma fila. Assim, a execução inicia do topo, realizando cada declaração/comando, até o final do arquivo de maneira sequencial.

Quando realizamos uma requisição, ela pode demorar alguns segundos para completar e retornar uma resposta de tal forma que essa requisição poderia “parar” o programa (_blocking code_). Entretanto, não desejamos que todo o programa seja bloqueado por causa de uma requisição – você pode desejar continuar navegando enquanto uma operação está sendo concluída. Para isso não acontecer, devemos utilizar **programação assíncrona**.

Na programação assíncrona, **as funções não são executadas em ordem**, possibilitando executar os comandos que podem demorar algum tempo para completar sem que o programa seja bloqueado. De forma geral, o programa irá esperar por uma parte do código enquanto executa outro comando em paralelo (ao mesmo tempo).  

Nesse contexto, temos o conceito de **_promises_ (promessas), que são um objeto usado para processamento assíncrono**. Uma _promise_ em JavaScript é como uma promessa na vida real, representando um valor que pode estar disponível agora, no futuro ou até mesmo nunca. Os exemplos irão ilustrar bem esses cenários.  

Uma _promise_ tem três possíveis estados: _pending_, _fulfilled_, _rejected_. Veja a seguir:

##### _Pending_ (pendente)
Estado inicial, que não foi realizado nem rejeitado.

##### _Fulfilled_ (realizado)
Sucesso na operação.

##### _Rejected_ (rejeitado)
Falha na operação.

Para exemplificar, podemos utilizar um construtor para criar uma _promise_. Ele receberá dois parâmetros, um para caso de sucesso e um para caso de falha, como exibido no Código 1. Podemos fazer uma condição: se ela for atendida, o estado da _promise_ será realizado; do contrário, será rejeitado. O console.log() da promessa criada está representado na figura a seguir. Podemos alternar os valores na soma para verificar os estados. Vamos observar juntos. 

![[Pasted image 20241025113847.png]]
![[Pasted image 20241025113911.png]]

**As _promises_ têm dois métodos fundamentais: _then_ e _catch_**. Quando uma _promise_ tem o estado realizado, podemos acessar o dado com o método _then()_, e, quando rejeitado, podemos acessar o erro que ocorreu com o método _catch()_.  

Partindo do exemplo anterior, o Código 2 apresenta a sintaxe utilizada para os métodos. Vale ressaltar que a resposta do _then_ é um dado, que pode ser utilizado para alguma operação; já a resposta do _catch_ é o erro interpretado, que pode ser apresentado. Confira:

![[stb4 1 1.png]]

As _promises_ podem falhar por diferentes razões, como, por exemplo, uma conexão de rede com falha ou um erro retornado do servidor (por exemplo, o erro 409 indica que a solicitação atual conflitou com o recurso que está no servidor).

### Requisições

A comunicação em HTTP reside no conceito de **ciclo de requisição e resposta**: o cliente (no caso o código JavaScript) envia uma requisição para o servidor na expectativa de receber uma resposta. Para fazer uma requisição em HTTP, a aplicação cliente precisa informar: a URL, o método e o cabeçalho.

![[Pasted image 20241025114426.png]]
![[Pasted image 20241025114535.png]]
![[Pasted image 20241025114603.png]]
![[Pasted image 20241025114623.png]]

Depois de o servidor receber a requisição, ele irá tentar fazer o que foi solicitado e retornará uma resposta. Essa resposta terá uma estrutura similar à da requisição, mas, em vez da URL e do método, **a resposta informará o _status code_**, que, como mencionado anteriormente, é um valor numérico que representa uma **mensagem autodescritiva** que informa sobre o estado final da execução daquilo que foi solicitado. Vamos ver na tabela um resumo sobre os diferentes códigos e seus significados:

![[stb6_01.png]]

O **cabeçalho** também é alterado na resposta do servidor, ele passa informações relevantes para a construção da representação da resposta. Por exemplo, a dado “Content-type” informa o tipo de dado retornado para indicar ao cliente como deve interpretar o dado retornado. A figura a seguir, apresenta um resumo sobre a estrutura da requisição e da resposta.

![[stb6_02.png]]

#### Formas de fazer a requisição

Como realizar as requisições na prática? Para fazer a solicitação para o _back-end_, podemos utilizar clientes HTTP como Fetch ou Axios. Ambos são baseados em _promises_.

A **API Fetch** é uma interface JavaScript que contém o método chamado _fetch()_ para realizar requisições. Ela já é integrada a navegadores e possibilita consultar (fazer requisições) um _back-end_ de forma assíncrona sem a necessidade de bibliotecas adicionais. Com a programação assíncrona podemos fazer requisições e executar tarefas em “segundo plano”, sem precisar interromper a execução de outras tarefas que podem estar acontecendo no _front_.  

Por exemplo, para atualizar uma contagem de “visualizações” de uma postagem, eu não preciso paralisar ou interromper a execução de toda a página; posso apenas consultar discretamente em segundo plano a contagem sem interromper a experiência do usuário.

O código a seguir apresenta a sintaxe básica de uma requisição com o Fetch, em que a URL é passada como único argumento à função _fetch()_. Note que não definimos o método explicitamente. Nesse caso, a função irá assumir que a requisição será um simples GET (apenas a URL e sem adição de parâmetros). **Como a _fetch()_ retorna uma _promise_, precisamos utilizar o método _then_ para definir o que será feito quando a promessa se concretizar**, que, no caso do exemplo, é acessar o conteúdo retornado da requisição HTTP.  

Vamos entender juntos vendo a imagem:

![[stb7 5.png]]

O objeto _response_ não contém diretamente o corpo da resposta, mas é uma representação de toda a resposta HTTP prometida. Supondo que o conteúdo da _response_ seja um JSON, cenário comum no uso de APIs, uma vez concretizada a promessa, seria necessário utilizar o método .json() da _response_ para fazer a interpretação do conteúdo. Uma vez recebida a resposta e interpretado o conteúdo, podemos então utilizar esse conteúdo para atualizar ou criar conteúdo na página. Essa informação vai ficar mais clara com o vídeo da técnica aplicada.  

Além disso, podemos utilizar as palavras-chave _async_ e _await_ – disponíveis no JavaScript a partir do ES2017 –, que possibilitam uma sintaxe simplificada para programação assíncrona. Podemos definir uma função como _async_ e utilizar _await_ antes de qualquer expressão que retorne uma _promise_. A execução da função _async_ será pausada até que a _promise_ seja resolvida. Entenda melhor a sintaxe básica apresentada no código:

![[stb8 5.png]]

No código, na primeira atribuição, a _await_ vai receber uma _promise_ da _fetch()_ que será transformada em um valor, quando a promessa for concretizada, que será atribuída à variável _response_. Nesse caso, _await_ poderá lançar uma exceção em caso de erro. Com a _await_, o JavaScript só interpretará a próxima linha após a finalização dessa primeira _promise_.

Também temos outra opção para a fazer requisições: a biblioteca JavaScript chamada [**Axios**](https://axios-http.com), que transforma os dados em JSON automaticamente. Por se tratar de um pacote externo, é necessário instalar para [utilização](https://axios-http.com/docs/intro). A sintaxe básica pode ser vista no código a seguir. Note que o JSON real já é obtido na resposta e podemos acessá-lo utilizando a propriedade data. Além disso, também poderíamos utilizar as palavras-chave _async_ e _await_ com Axios.

![[01 4 3.png]]

Na técnica aplicada desta aula, vamos apresentar exemplos de códigos como forma de fazer requisições a uma API de dados. Vamos explorar um pouco esses diferentes cenários continuando o desenvolvimento do _front-end_ iniciado na aula anterior, mas desta vez consumindo o dado de uma API.

O compartilhamento de recursos com origens diferentes (_Cross-Origin Resource Sharing_ – CORS) é um mecanismo utilizado por navegadores para possibilitar que um aplicativo _web_ seja executado em uma origem e acesse recursos de um servidor de uma origem diferente. O CORS faz uso de cabeçalhos do HTTP para informar aos navegadores se um recurso pode ser acessado ou não.  

Ao realizarmos uma requisição, podemos acabar encontrando o seguinte erro:  

_“[...] blocked by CORS policy: Cross origin requests are only supported for protocol schemes: http, data, chrome-extension, edge, https, chrome-untrusted.”_

Isso acontece por motivos de segurança, já que a política de mesma origem (_same-origin policy_) restringe a maneira de um _script_ de uma origem interagir com um recurso de outra origem, evitando, assim, ataques maliciosos. Porém, apesar de ser algo implementado nos navegadores, a política de CORS deve ser implementada no _back-end_.

### Publicação de uma aplicação

**A publicação, ou o _deploy_** da publicação, é um processo em que no final disponibilizamos a aplicação para o nosso cliente final. Um sistema moderno tem no mínimo três camadas, como na imagem apresentada no início da aula. O _front-end_ é a camada da comunicação que conecta o usuário (via _browser_) à aplicação (o _back-end_). Estamos chamando de _back-end_ tudo aquilo a que o usuário não tem acesso direto. Com isso, o que chamamos de _back-end_ pode abstrair várias outras camadas de serviços. Mas, para simplificar na explicação, vamos ficar com a representação feita e imaginar o _back-end_ como uma única aplicação que escuta as regras de negócio e que também serve e armazena dados.

**Uma das muitas vantagens dessa separação de responsabilidade é maior controle sobre como a infraestrutura é utilizada**. O servidor de _front-end_ tem geralmente baixo custo de manutenção (no sentido de que é barato mantê-lo disponível _on-line_). Já o _back-end_ tende a ser mais caro, seja pelo custo do armazenamento, seja pela complexidade na execução das regras de negócios. Dessa forma, podemos ter diferentes perfis de máquinas para hospedar essas aplicações: uma mais robusta para o _back-end_ e outra mais simples para o _front-end_.

Todo servidor, seja para _front_ ou para o _back-end_, deve ser _stateless_, ou seja, deve ter ausência de estados. Isso significa que um servidor não deve manter a “lembrança” de informações relativa a requisições anteriores. O servidor deve receber todo o contexto necessário dentro das requisições. Isso ficará mais claro na disciplina sobre o desenvolvimento _back-end_. Se é desejado guardar uma informação de contexto sobre um usuário, por exemplo, isso deve ser feito de outra forma. Uma possibilidade seria através de _cookies_ no _browser_.

O fato é que ser _stateless_ e isolado rende ao servidor a capacidade de atender mais de um cliente de forma mais eficiente – não precisar gastar tempo e processamento gerenciando esse tipo de informação. Ainda assim, esse atendimento acontece de forma sequencial, uma requisição atendida por vez, o que não é um problema, já que podemos ter executado mais de uma instância de um mesmo servidor e utilizar uma ferramenta para gerenciar o balanceamento de carga (_load balance_) entre essas diferentes instâncias.

Diferentemente da publicação de um _back-end_, que tende a ter um processo de preparação e configuração mais complexo, a publicação de um _front-end_ é geralmente simples. Existem várias soluções pagas que facilitam esse processo, assistindo o desenvolvedor durante todas as etapas da publicação. Ambientes como [Azure](https://learn.microsoft.com/pt-br/azure/app-service/quickstart-nodejs), [Google Cloud](https://cloud.google.com/nodejs/getting-started?hl=pt-br) e [Amazon AWS](https://aws.amazon.com/pt/getting-started/hands-on/deploy-nodejs-web-app/?nc1=h_ls) fornecem tutoriais com exemplos para a publicação de uma aplicação de _front-end_ feita em Node.js. Na figura a seguir, temos um cenário de publicação da aplicação em um ambiente Amazon AWS.

![[stb10 5.png]]

Na proposta de arquitetura da AWS apresentada na figura, temos um cenário completo para a execução de um servidor construído em node.js. Nela, instâncias do servidor são executadas em máquinas da _cloud_ AWS (Amazon EC2). O Elastic _Load Balancer_ é a ferramenta de load balance utilizada para receber a requisição do cliente e repassá-la para uma instância do servidor (a que estiver com menor carga). O Amazon S3 Bucket é o repositório de arquivos estáticos, como imagens, _gifs_ e qualquer outro recurso estático que pode ser exibido no _front-end_. O Amazon SNS é um sistema de mensagens que pode ser utilizado para monitoramento inteligente da aplicação. O DynamoDB é apenas um banco de dados que pode estar disponível para a aplicação.  

Comparando essa proposta de arquitetura com a exibida na figura do início da aula, o banco de dados não está diretamente acessível ao _front-end_. O _back-end_ assumiu essa responsabilidade.

#### Ambientes de teste, homologação e produção

Para chegar até o cliente, é esperado que a aplicação tenha sido pelo menos testada e homologada. Com isso, antes de ser entregue ao cliente, ou seja, posta em um ambiente de produção (PRD), a aplicação deve ser antes testada em outros dois ambientes: **teste (TST) e homologação (HMG)**.

![[stb11 2 1.png]]

Só após uma validação de conformidade no ambiente de teste é que a aplicação deve ser publicada no ambiente de HMG.

No ambiente de homologação, o teste agora é com os clientes. Nesse ambiente, o cliente (o “dono da aplicação”) ou pessoas selecionadas que podem representar o cliente final irão testar a conformidade do sistema entregue com aquilo que foi especificado. De forma análoga ao ambiente de teste, uma URL específica vai ser criada para a aplicação que está nesse ambiente, por exemplo, “http://meu_app-hmg.com.br”.

Só depois da validação no ambiente de HMG é que o código poderá finalmente ser entregue ao cliente final, ou seja, publicado no ambiente de produção.  

Essa prática é comum em todo e qualquer projeto de aplicação _web_. A proposta é que, a cada nova funcionalidade desenvolvida ou a cada nova atualização do _software_, uma nova versão da aplicação seja definida e passe por todos esses processos até a entrega ao cliente final.

### E quanto à acessibilidade?

Desenvolvemos interfaces para pessoas, e, como já foi dito aqui mais de uma vez, o _front-end_ é responsável pela comunicação entre sistema e usuário – não adianta ter o mais poderoso dos sistemas se o usuário é incapaz de interagir com ele. Para a comunicação ser eficaz, o usuário deve entender como interagir com o sistema. É nesse ponto que vem a questão da acessibilidade.

Falar de acessibilidade não se restringe a falar de usuários com deficiências permanentes, com a perda completa da visão em decorrência de um acidente, mas também da deficiência momentânea, como a causada quando a pessoa esquece os óculos e fica com sua visão limitada, ou quando a deficiência é decorrente de um processo natural de envelhecimento, como o aumento da miopia com o passar do tempo.

Como podemos tornar as nossas páginas _web_ mais acessíveis? No vídeo a seguir, apresento o tema acessibilidade no contexto do desenvolvimento _front-end_ ressaltando a relevância do tema e ferramentas que podem nos auxiliar no desenvolvimento de páginas cada vez mais acessíveis para todos.

#### Acessibilidade e o desenvolvimento _front-end_

Segundo quem criou a _web_, Tim Berners-Lee, “o poder da _web_ está em sua universalidade. O acesso por todos, independentemente de sua deficiência, é um aspecto essencial”. Neste vídeo, vamos ver qual caminho tomar para a promoção da acessibilidade na _web_. Você vai ver que o direito ao acesso à _web_ é algo previsto pela Organização das Nações Unidas (ONU) na Convenção sobre os Direitos das Pessoas com Deficiência e que o World Wide Web Consortium (W3C) tem uma série de diretrizes com recomendações relativas ao tema. Também vamos discutir como produzir, testar e verificar páginas atentas às diretrizes do W3C sobre o tema.

![[Pasted image 20241025124037.png]]
![[Pasted image 20241025124050.png]]
![[Pasted image 20241025124136.png]]
![[Pasted image 20241025124218.png]]
![[Pasted image 20241025124246.png]]
![[Pasted image 20241025124313.png]]
![[Pasted image 20241025124354.png]]
![[Pasted image 20241025124405.png]]
![[Pasted image 20241025124453.png]]
![[Pasted image 20241025124515.png]]
![[Pasted image 20241025124546.png]]
![[Pasted image 20241025124557.png]]
![[Pasted image 20241025124630.png]]
![[Pasted image 20241025124657.png]]
![[Pasted image 20241025124710.png]]
![[Pasted image 20241025124722.png]]
![[Pasted image 20241025124730.png]]
![[Pasted image 20241025124803.png]]
![[Pasted image 20241025124812.png]]

### Transformação de Mercado

Como vimos nesta disciplina, há uma grande diferença entre implementar um _site_ usando apenas HTML, JavaScript e CSS _versus_ implementar um _site_ reativo utilizando um _framework_ e bibliotecas. Essa mudança foi um processo histórico desde os primeiros dias da internet, com mais mecanismos e recursos sendo inventados com o passar do tempo.

Esse processo constante de avanço nos faz questionar: **como será o desenvolvimento _web_ no futuro? Quais serão os recursos que teremos à nossa disposição? Quais técnicas serão inventadas em cima desses recursos?**  

Temos dois tipos de avanços para considerar: avanços graduais e avanços revolucionários. Atualmente, ainda parecemos estar firmemente na era do desenvolvimento baseado em componentes, com novos desenvolvimentos focando em facilitar esse tipo de implementação. Novas bibliotecas são criadas todos os dias e visam a facilitar nossa vida como desenvolvedores.

Porém, há outra tendência que já está ocupando mais e mais espaço no desenvolvimento _web_, já que não requer muito conhecimento de programação. Este é o objetivo principal dos sistemas [**_low-code_**](https://www.ibm.com/cloud/blog/low-code-vs-no-code) e [**_no-code_**](https://www.ibm.com/cloud/blog/low-code-vs-no-code). Sistemas _no-code_ permitem que usuários construam seus próprios _sites_ a partir de uma série de componentes pré-construídos e que podem ser conectados. Já os sistemas _low-code_ apresentam algumas dessas facilidades, mas ainda requerem algum nível de programação.

Entre as vantagens desses sistemas está a baixa barreira de entrada para aqueles que não têm habilidades de programação. Ao precisarem apenas localizar componentes na interface, utilizando lógicas de funcionamento pré-estabelecidas, usuários precisam apenas projetar a interface, sem ter que mexer em código.

Por sua vez, a dependência de componentes pré-estabelecidos limita os tipos de _sites_ que podem ser construídos com eles. _Sites_ que dependem de interações mais complexas, por exemplo, podem ser impossíveis de construir nessas plataformas. Nesse aspecto, as versões _low-code_ têm certa vantagem ao permitirem um nível maior de customização, mas o controle nunca será tão completo quanto com o desenvolvimento em código.

É possível que essas plataformas evoluam e com o passar do tempo venham a dominar o desenvolvimento _web_, mas esse dia ainda não chegou. De qualquer forma, vale a pena prestarmos atenção nessas plataformas à medida que elas evoluem. Sempre temos que tentar focar em otimizar o nosso processo de desenvolvimento, mesmo que tenhamos que abandonar o código bruto em si.

### Técnica Aplicada

Agora chegou a hora de colocar em prática um pouco do que discutimos sobre a comunicação do _front_ com o _back-end_. Na técnica aplicada, vamos apresentar exemplos de códigos como forma de fazer requisições a uma API de dados. Além disso, vamos explorar como tratar a resposta e gerar conteúdo visual a partir dela de forma dinâmica.  

Vamos continuar o desenvolvimento da _single page application_ (SPA) iniciada lá na segunda aula, mas desta vez consumindo o dado de uma API em vez do acesso aos dados estáticos de um arquivo JSON.

Na técnica aplicada, vamos exercitar um pouco as formas de conexão entre _front_ e _back-end_. Vamos apresentar as formas mais comuns de comunicação com o Fetch e com o Axios, além dos modos de configurar requisições assíncronas. Não vamos só requisitar, mas também explorar como ler o dado retornado de uma resposta e como gerar conteúdo visual a partir desse conteúdo.

![[Pasted image 20241025131447.png]]
![[Pasted image 20241025131456.png]]
![[Pasted image 20241025131611.png]]
![[Pasted image 20241025131702.png]]
![[Pasted image 20241025131727.png]]
![[Pasted image 20241025131738.png]]
![[Pasted image 20241025131749.png]]


### Referências:

ACESSIBILIDADE. **React**, c2023. Disponível em: [https://pt-br.legacy.reactjs.org/docs/accessibility.html](https://pt-br.legacy.reactjs.org/docs/accessibility.html). Acesso em: 21 fev. 2023.

CHECKLIST, check your WCAG compliance. **A11y Project**, c2013-2023. Disponível em: [https://www.a11yproject.com/checklist/](https://www.a11yproject.com/checklist/). Acesso em: 21 fev. 2023.

CONTRAST checker. **WebAIM**, c1999-2023. Disponível em: [https://webaim.org/resources/contrastchecker/](https://webaim.org/resources/contrastchecker/). Acesso em: 21 fev. 2023.

DIRETRIZES de acessibilidade para conteúdo web (WCAG) 2.0. **W3C**, c2008. Disponível em: [https://www.w3.org/Translations/WCAG20-pt-br/](https://www.w3.org/Translations/WCAG20-pt-br/). Acesso em: 21 fev. 2023.

Tendência de desenvolvimento low-code ou no-code. Disponível em:[https://www.zdnet.com/article/the-future-of-the-web-will-need-a-different-sort-of-software-developer/](https://www.zdnet.com/article/the-future-of-the-web-will-need-a-different-sort-of-software-developer/). Acesso em: 21 fev. 2023.

THE A11Y PROJECT. **A11y Project**, c2013-2023. Disponível em: [https://www.a11yproject.com/](https://www.a11yproject.com/). Acesso em: 21 fev. 2023.

WAVE web accessibility evaluation tools. **WebAIM**, c1999-2023. Disponível em: [https://wave.webaim.org/](https://wave.webaim.org/). Acesso em: 21 fev. 2023.

WE HAVE web accessibility in mind. **WebAIM**, c1999-2023. Disponível em: [https://webaim.org/](https://webaim.org/). Acesso em: 21 fev. 2023.

# Desenvolvimento Front-End  Mobile (Disciplina 3)

## Desenvolvimento _front-end mobile_ (Aula 1)

Esta aula trata das especificidades do desenvolvimento _mobile_ e das macroetapas envolvidas no desenvolvimento. Iremos discutir os principais desafios e apresentar técnicas e ferramentas para ajudar o desenvolvedor.

Como ponto central, o desenvolvedor de um aplicativo _mobile_ terá sempre como foco saber **o que o usuário precisa e deseja** e deve se preocupar sempre com a questão de como será a experiência do usuário do aplicativo.

Inicialmente, é importante identificar **qual problema do usuário o seu aplicativo pretende resolver**, se é de localização/navegação, comunicação, localização de estabelecimentos, rede social, opções de entretenimento, etc. Depois, é necessário avaliar se o usuário de fato será capaz de usar o app, se terá interesse em usá-lo e o tempo necessário para usar o seu app. Por exemplo, aplicativos voltados para o trabalho no escritório não tendem a ter muito apelo para uso no aplicativo. No fundo, **você precisa estudar bem o problema e levantar os requisitos de app.** Quando você tiver estabelecido para o que e para quem será o seu aplicativo, você já estará quase pronto para começar.

![[stb1 2 1.png]]

Com esses números da indústria, logo fica claro que o desenvolvimento de aplicativos móveis é um fator-chave para o sucesso comercial.

### Identificar as necessidades do usuário e procurar aplicativos similares

Idealmente, o desenvolvimento de um app deve ser em equipe, envolvendo também pelo menos um **_designer_ de interfaces do usuário** (_Graphical User Interfaces_ – GUI) e um **desenvolvedor _back-end_**. O motivo é que um aplicativo _mobile_ quase sempre requer a interação com um servidor _back-end_ e precisa estar muito bem projetado do ponto de vista de usabilidade.

Como a responsividade do aplicativo é um fator crítico para a sua adoção, é também muito importante que a interação com o serviço _back-end_ tenha baixa latência e que seja assíncrona, isto é, nunca bloqueie a interface gráfica do usuário.

Além disso, como projetista do app, você dever fazer uma pesquisa preliminar para saber se já existe algum aplicativo similar, quais são suas funcionalidades, seus pontos fortes e suas limitações. Assim, evita-se “reinventar a roda” e já começar com um forte aplicativo concorrente, que pode limitar o número de usuários que instalam o seu app em seu _smartphone_, lembrando sempre a facilidade com que um usuário consegue baixar um novo app da AppleStore ou do Google Play para trocar pelo seu app.

### Particularidades do desenvolvimento _mobile_

Você deve lembrar que o desenvolvimento _mobile_ tem uma série de especificidades que o distingue do desenvolvimento para _desktop_ ou _web_.

![[Pasted image 20241025202358.png]]
![[Pasted image 20241025202707.png]]

Por todas essas – e outras – razões, o desenvolvimento _front-end mobile_ é bem diferente do desenvolvimento para a _web_ e _desktops_ e precisa ser estudado à parte.

### Qual plataforma?

Uma decisão importante a ser tomada é **qual será a plataforma-alvo**: Android, da Google, ou iOS, da Apple, este último de código fechado. A plataforma é o sistema operacional para _smartphones_ e dispositivos móveis. No passado, já houve muitas outras plataformas _mobile_, mas que caíram em desuso, como Windows Mobile, LG UX, One UI, Blackberry 10, etc.  

A plataforma Android é uma plataforma que utiliza um _kernel_ Linux modificado. A plataforma Android foi introduzida pela Open Handset Alliance em novembro de 2007. **A maioria das aplicações que rodam na plataforma Android é escrita na linguagem de programação Java.**  

Atualmente, o Android está instalado em mais de 95% dos _smartphones_, em parte porque foi adotado por muitos fabricantes de aparelhos, enquanto o iOS está restrito, a princípio, aos produtos da Apple.  

Por sua vez, o iOS surgiu junto com o iPhone em 2007. Desde então, foi estendido para suportar outros dispositivos Apple, como o iPod Touch e o iPad (2010). **O iOS goza de muito prestígio por causa de sua interface de usuário elegante e bem elaborada.**

![[pos-graduacao/3º Acervo de imagens (Disc 3)/stb3.png]]
### Programando apps para Android e iOS

O ideal seria poder desenvolver o aplicativo em uma única linguagem de programação que servisse para ambas as plataformas. A boa notícia é que isso existe, e já foram criados vários ambientes multiplataforma (_cross-platform_), entre eles o **Flutter**, que será visto em mais detalhes nestas aulas de desenvolvimento _front-end mobile_. Entre todos da longa lista de ambientes multiplataforma, destacam-se o React Native e o Flutter. Estes são os mais completos e robustos e, por isso, também os mais usados. O Xamarin (da Microsoft, para .Net e C#) é outro exemplo _cross-platform_, mas já foi superado pelos dois anteriores.  

A principal diferença entre o React Native (RN) e o Flutter é a seguinte:  

O código JavaScript do RN não é convertido para código nativo, e toda interação entre o JavaScript e o código nativo usa uma ponte (_bridge_), que passa a ser um gargalo na comunicação entre o JavaScript e a plataforma nativa.

![[stb4 2 1.png]]

Já o Flutter interage diretamente com as componentes e APIs da plataforma nativa.  
- Todo _widget_ (elemento da UI) é renderizado diretamente no _hardware_ do dispositivo, e apenas o Canvas da plataforma é usado.
- Assim, o aplicativo vai executar exatamente igual em todas as versões do Android e do iOS (e também de um _web browser_).
- Essa execução será mais eficiente do que no RN por estar acessando-a sem um _broker_, somente através de _widgets_ e de _platform channels_ (que veremos depois).

![[stb5 3.png]]

Deve-se notar que boa parte do Flutter é apenas um _framework_, ou seja, uma grande coleção de objetos (_widgets_) que são classes de objetos renderizáveis, extensíveis e configuráveis. São usados para compor cada tela de um aplicativo. O Flutter também contém um _mecanismo/engine_ que **sabe como devem percorrer os _widgets_ para renderizá-los na tela.**  

_Widgets_ são construídos a partir de uma estrutura moderna que é inspirada em React. A ideia básica é construir toda UI a partir de uma **composição de widgets**, cada um descrevendo uma parte ou aspecto da UI e como deve ser sua aparência e forma, dada sua configuração e seu estado atual. E todos os _widgets_, em uma app, são estruturados em uma árvore – para renderização – de acordo com o seu nível de aninhamento _inter-widget_. Quando o estado de um _widget_ muda, ele é reconstruído segundo o seu novo, cujas diferenças são usadas pelo algoritmo de renderização para gerar a nova visão.

![[stb6 1 1.png]]

A _engine_ de renderização (que está contida no Embedder, _runtime_ do Flutter), assim como os objetos _widgets_, são em grande parte implementados na linguagem Dart, que também é usada para acoplar os objetos e implementar a lógica de sua aplicação. Então, **quando se fala de Flutter, na verdade se está falando de Flutter + Dart.**

### Escolhendo o _layout_ e o estilo

O primeiro passo na concepção do seu aplicativo consiste no **projeto da interface do usuário (UI)**. Esta deve ser muito bem planejada, para que seja simples de usar, intuitiva (baseando-se em convenções e padrões de interação largamente utilizados) e tenha uma aparência bonita, com uma palheta de cores que sejam agradáveis.  

Felizmente, o Flutter já vem com dois _designs_ padrão, um de interfaces típicas Android e outro de aplicações iOS, chamados de **Material Design e Cupertino**, respectivamente. Isso significa que com poucas alterações você pode trocar o _look_ & _feel_ (a aparência e os comandos típicos) do seu aplicativo de Android para iOS, e vice-versa, e ao mesmo tempo executar o aplicativo em qualquer plataforma. Ou seja, pode-se facilmente emular um aplicativo típico de iOS em um _smartphone_ que não seja um iPhone.

**Material Design** é uma linguagem de _design_ – uma grande coleção de objetos _widgets_ e ícones – orientada ao Android criada pelo Google. Esse _design_ suporta a exibição e o arranjo de ícones na tela e o reconhecimento dos movimentos dos dedos usuais em Android e que imitam o manuseio de coisas do mundo real, como, por exemplo, a barra de _scroll_ lateral ou o _zoom-in_ e _zoom-out_ com os dedos polegar e indicador.  

Já **Cupertino** é um grande conjunto de _widgets_ de alta fidelidade para a linguagem de _design_ que também contém elementos de visualização, organização gráfica e de interação com os dedos que é típica dos aplicativos iOS. Ou seja, usando Flutter é possível dar ao seu aplicativo “uma cara” de um iOS app ou um Android app.

De forma geral, **certifique-se de que a navegação em seu _layout_ e seus _widgets_ sejam muito simples e intuitivos.** Felizmente, isso é ajudado de alguma forma pelo fato de que estes só aceitam comandos minimalistas de toque, de um ou dois dedos. É também importante que um _widget_ seja flexível.  

Como muitos usuários gostam de personalizar o visual de sua página inicial, e este precisa ficar bem apresentado em vários tamanhos de tela, certifique-se de que seu espaço seja redimensionável e que os usuários possam ajustar suas telas como quiserem.  

A seguir, vejamos as etapas iniciais para a concepção do seu aplicativo.

![[Pasted image 20241025205752.png]]
![[Pasted image 20241025205727.png]]
![[Pasted image 20241025205839.png]]

_Wireframes_ não se enquadram apenas no âmbito dos _designers_ de UI/UX. Desenvolvedores, gerentes de produto e outros interessados frequentemente usam também _wireframes_ para expressar suas ideias de _design_. Estes podem ser realizados usando ferramentas de baixa tecnologia, como lápis e papel, ou _software_, como Balsamiq, Figma, Adobe XD, Adobe Photoshop, Justinmind, uizard.io e Mockplus.

![[img_prof.png]]
Uso de wireframing para o projeto da UI, as telas e a navegação entre elas.

Nas etapas seguintes do _design_ (geralmente só feitas por _designers_ e para aplicativos que virarão produtos), faz-se um **refinamento das interfaces**, na fase dos _mockups_, e depois os **protótipos de UI**, ainda sem o aplicativo todo desenvolvido.

Os **_mockups_** são uma representação visual do _design_ de média fidelidade. Feitos na posição dos objetos delineados no estágio de _wireframing_, os _mockups_ incorporam **fontes, logotipos, tipografia, gráficos de navegação, cores, imagens e textos.**

Os _mockups_ tendem a não ser interativos, o que significa que botões e representações visuais de _links_ não podem ser clicados. Ainda assim, o _design_ estático é útil para ajudar as equipes de _design_ a determinar a estética visual de um produto. Nessa fase, também é possível **realizar testes com o usuário** para obter _feedback_ sobre quais elementos visuais podem não estar funcionando.

Já os protótipos são uma representação de alta fidelidade do aplicativo final.

Diferentemente dos _wireframes_ e _mockups_, os **protótipos simulam fielmente a experiência final** com _links_ clicáveis e outros elementos interativos, o que significa que eles são ideais para testes de usabilidade, mostrando aos interessados (clientes, usuários em potencial) como será o produto final em ação, e para identificar problemas de usabilidade que porventura podem ser dispendiosos de alterar mais tarde.

Lembrando sempre que o _mobile_ app é um _front-end_, e o que mais importa é boa usabilidade, estética agradável e rápida responsividade.

### Implementando o seu aplicativo

Antes de começar a desenvolver o app, você precisa criar o seu ambiente de desenvolvimento. Isso inclui um Integrated Development Environment (IDE). Existem inúmeros bons IDEs que servem, mas a nossa experiência mostra que o VS Code da Microsoft é um ótimo ambiente e funciona muito bem. Depois de instalar o VS code em seu computador, selecione o Flutter plugin para Virtual Studio code e reinicie o Virtual Studio Code.

Depois, você precisa instalar o Android Studio para poder usar **emuladores Android**. Se você também quiser desenvolver logo para iOS, precisará instalar o **Xcode tools** da Apple e o emulador de iOS. Se você quiser testar o seu aplicativo diretamente no seu _smartphone_, também pode. Para isso, conecte o seu aparelho por cabo USB no seu _desktop_ ou _notebook_.

Feito isso, você pode começar a implementação. No Git, no Bitbucket e em outros repositórios existem vários exemplos (em código) abertos que podem ser usados como ponto de partida para o seu. Portanto, sugiro que você pegue algum exemplo, talvez até de um tutorial do Flutter, e familiarize-se com o exemplo antes de começar a mexer nele, adaptando-o de acordo com aquilo que você imaginou para seu aplicativo.

![[Pasted image 20241025210710.png]]
![[Pasted image 20241025210643.png]]
![[Pasted image 20241025210732.png]]
![[Pasted image 20241025210751.png]]

O acesso a um serviço em _background_ é relativamente simples, especialmente através da convenção REST sob o protocolo HTTP. Nesse caso, deve-se ver como a API do serviço _back-end_ está implementada, e, naturalmente, **precisa-se seguir à risca a convenção de parâmetros de entrada e de saída do método remoto acessado**, bem como implementar um tratamento de erros do HTTP. Caso o protocolo API do _back-end_ for REST, toda a interação será na forma de comandos.

### Elaborar recursos visuais e ferramentas do aplicativo

Possivelmente, haverá a necessidade de personalizar o seu aplicativo, por exemplo, incluindo uma logomarca na tela inicial (_splash screen_), um _gif_ animado ou arquivos de recursos específicos. Todos eles são chamados de _assets_ e devem ser copiados para a pasta correspondente do seu projeto no VS Code.  

_Asset_ é um arquivo que é “empacotado” e implantado no seu aplicativo e também é acessível pelo programa do aplicativo em tempo de execução. Os tipos comuns de _assets_ incluem dados estáticos (i.e., arquivos JSON), arquivos de configuração, ícones e imagens.

Cada vez que um novo _asset_ é incluído, isso precisa também ser declarado no arquivo pubspec.yaml, localizado na raiz de seu projeto Flutter, para identificar os recursos requeridos por seu aplicativo.

Por fim, estude a documentação do Flutter para achar o _widget_ que permite o acesso a cada tipo de _asset_. Por exemplo, você pode carregar uma imagem usando a classe AssetImage em um método build() para construção do _widget._

Sem dúvida nenhuma, desenvolver um aplicativo robusto e de boa usabilidade para o usuário final é uma tarefa complexa, e, nesse sentido, ambientes multiplataforma são ferramentas muito úteis para o desenvolvedor _front-end mobile_, pois ele não precisa aprender os detalhes de cada uma das plataformas-alvo (Android, iOS, Micosoft Phone). Nos últimos anos surgiram várias desses ambientes, como o React Native, o Xamarin, o Iconic e o Flutter, sendo este último o que tem tido maior aceitação pela sua simplicidade, eficiência e versatilidade. E, por isso, também será o foco do nosso curso. Apesar do evidente benefício de ter que aprender apenas uma linguagem e ambiente, ambientes multiplataforma ainda têm que conviver com alguns problemas.  
  

O código do app tende a ser mais complexo, pois combina componentes nativos e não nativos, o que pode afetar o seu desempenho.  
  

Os aplicativos multiplataforma não conseguem suportar todas as funções e recursos nativos de dispositivos móveis, como gráficos, animações avançadas ou efeitos 3D. Por exemplo, o Flutter só consegue renderizar imagens 2D, não podendo, dessa forma, ser usado para _games_ em que o usuário percorre espaços virtuais. Portanto, isso pode restringir a funcionalidade e o _design_ da UI.  
  

Quando os fabricantes das plataformas nativas, no caso Google e Apple, adicionam novas funcionalidades às plataformas Android e iOS, as apps nativas podem usá-las imediatamente. Por sua vez, os aplicativos sobre Flutter, por exemplo, precisam esperar até que essas atualizações sejam incorporadas ao sistema Flutter. Assim, sempre haverá certo atraso na atualização dos apps multiplataforma. Felizmente, o Google tem todo interesse em atualizar também o Flutter, já que se trata de um projeto paralelo ao Android.

### Transformação de mercado

Até pouco tempo havia no mercado de trabalho “mobile Dev” duas classes de desenvolvedores _mobile_, aqueles especialistas em Android e aqueles especialistas em iOS, o que causava não só a duplicação de recursos humanos e custos para as empresas como também a grande probabilidade de versões Android e iOS acabarem não saindo iguais e apresentando pequenas diferenças. Isso, por sua vez, também causaria problemas na manutenção e na evolução do sistema como um todo. Felizmente, com a chegada dos ambientes multiplataforma, esse cenário está mudando. Isso é visível pela crescente procura de desenvolvedores Flutter e ReactNative, que, inclusive, vêm recebendo ofertas de emprego melhores do que seus colegas uniplataforma.

### Referências:

CREATING mobile app wireframes: a step by step guide. Balsamiq Wireframing Academy, c2008-2023. Disponível em: [https://balsamiq.com/learn/articles/mobile-app-wireframing-guide/](https://balsamiq.com/learn/articles/mobile-app-wireframing-guide/). Acesso em: 9 fev. 2023.

## Desenvolvimento _mobile_ (Aula 2)

Esta aula irá discutir novamente os benefícios dos ambientes multiplataforma e apresentar em mais detalhes um deles, o Flutter, que será o foco desta disciplina (módulo). Iremos ver do que são compostos o Flutter e a linguagem Dart e como eles possibilitam o desenvolvimento de aplicativos híbridos sem perda substancial de desempenho. Por fim, iremos apresentar os principais conceitos do modelo de programação Flutter e de que forma eles podem ser usados na programação de apps.

### Aplicativos nativos _versus_ multiplataforma

Aplicativos nativos contam com um _runtime_, ferramentas, _plugins_ e linguagens de programação específicas para uma plataforma. Por exemplo, Objective-C e Swift são usados para aplicativos iOS; já Java, C/C++ e Kotlin são específicos para criar soluções Android; e C# e Visual Basic são ideais para Windows Phone.

Ao criarem aplicativos nativos, os desenvolvedores são norteados pelos requisitos específicos do sistema operacional. Assim, um aplicativo nativo pode utilizar plenamente os recursos e capacidades disponíveis. A maior desvantagem é que um aplicativo nativo não é compatível com outras plataformas.

O desenvolvimento multiplataforma, por sua vez, visa a criar uma única aplicação que funcione de forma idêntica em várias plataformas. Para isso, utiliza tecnologias e linguagens agnósticas de plataforma, como HTML e CSS, e atende muitos dispositivos finais, como _smartphones_, _tablets_ e _wearables_.

Usando apenas tecnologias da programação _web_, como HTML e CSS, só é possível ter acesso limitado aos recursos dos dispositivos, em particular apenas aos recursos aos quais o _web browser_ tem acesso. Por isso, tecnicamente, tem-se uma programação _mobile web_, e não um desenvolvimento _mobile_ propriamente dito. Ambientes multiplataforma, por sua vez, mapeiam os conceitos, objetos e métodos agnósticos para os equivalentes nativos.

Os principais benefícios de usar um ambiente multiplataforma são os seguintes:  
- O principal é que desenvolver aplicações nativas separadas para cada plataforma é muito mais caro do que usar um único código compatível com as plataformas.
- A maior redução de custo se dá pela necessidade de se ter apenas uma equipe de programadores, _designers_ e testadores.
- Os aplicativos multiplataforma têm uma aparência (_look_ & _feel_) nativa, o que é ótimo para a experiência do usuário.
- Também há benefício de adoção do seu app, pois a base de usuários (clientes) irá englobar os usuários de cada uma das plataformas, e não só usuários de uma plataforma, como, por exemplo, usuários de iPhone e de _smartphones_ Android, cobrindo, assim, praticamente 100% do mercado.

Como vimos, **existe uma extensa lista de ambientes multiplataforma**, como o Xamarin, o iConic, o ReactNative e o Flutter. Estes dois últimos são os mais completos e robustos e, por isso, também os mais usados. Todos eles têm uma camada de _software_ que faz o mapeamento de conceitos do ambiente e da linguagem para a plataforma nativa: Android, iOS ou Windows Phone.

### Visão geral do Flutter

Essencialmente, o Flutter é composto de um _framework_ de _widgets_ (objetos renderizáveis), o _embedder_ e _plugins_. O _embedder_ é o _runtime_, faz o mapeamento com a plataforma (Android e iOS) e contém o renderizador de _widgets_ e o captador de eventos. No renderizador, é executado um algoritmo/mecanismo que sabe como deve percorrer os _widgets_ para renderizá-los na tela.

O _framework_ é uma grande coleção de objetos (_widgets_) relacionados, que são renderizados na tela, e são configuráveis e extensíveis. São usados para compor cada tela de um aplicativo.

O Flutter é (quase todo) implementado na linguagem de programação Dart, que também é a linguagem usada pelo desenvolvedor para criar a estrutura de _widgets_ e implementar a lógica de sua aplicação. Então, quando se fala em desenvolver em Flutter, seria mais preciso dizer em Flutter e Dart.

### Widgets

_Widgets_ são os elementos fundamentais que compõem e definem a aparência visual e o _layout_ da interface gráfica do usuário (UI).

A ideia é construir toda UI a partir de _widgets_, cada um descrevendo como deve ser sua aparência e forma. Isso é determinado pelos seus parâmetros de construção (configuração) ou atual estado interno.

Em Flutter, quase tudo é um _widget_ – incluindo os elementos que compõem os _layouts_. As imagens, os ícones e os textos que você vê em um aplicativo Flutter são todos _widgets_, assim como coisas invisíveis, como as linhas, colunas e grades que organizam, restringem e alinham outros _widgets_ visíveis, aninhados ou vizinhos.

Um _layout_ é composto por esses _widgets_ estruturantes para construir partes da UI. Diferentemente do React Native, no Flutter todo _widget_ é renderizado diretamente no Canvas (na tela) do dispositivo. Assim, o aplicativo vai executar exatamente igual em todas as versões do Android e do iOS (e também de um _web browser_). Um aplicativo Flutter (app) por si mesmo é um _widget_, e a maioria dos _widgets_ tem um método construtor de build(). Instanciando e dando _return_, um _widget_ no método build() do app exibe o _widget_ na tela.

![[01 5 2.png]]
![[02 2 2.png]]
![[03 1 3.png]]
![[04 8.png]]

Na página de documentação do Flutter pode-se obter a relação completa de todos os _widgets_ Flutter. Clique no _link_ a seguir para acessar a [página](https://docs.flutter.dev/development/ui/widgets).

#### Árvore de _widgets_

Para compor uma UI, _widgets_ são organizados em uma árvore de _widgets_ de acordo com sua relação de aninhamento _inter-widget_. E, quando o estado de um _widget_ muda, este – assim como todos os seus _widgets_ “descendentes” na árvore – é reconstruído segundo os seus novos parâmetros ou seu novo estado. O algoritmo de renderização do Flutter identifica as diferenças e realiza a rerenderização para obter a nova visão. A imagem a seguir apresenta um exemplo de árvore de _widgets_ típica.

![[stb2 4.png]]

#### BuildContext

BuildContext é uma referência para a localização de um _widget_ na estrutura em árvore dos _widgets_. Um contexto pode pertencer a apenas um _widget_. Se um _widget_ tem _widgets_ filhos, então o contexto do _widget_ pai se torna o contexto pai para os contextos de elementos filhos diretos.

O BuildContext está presente em todo o WidgetBuilder e apresenta um conjunto de funções que podem ser usadas durante a construção do _widget_.

Alguns exemplos de funções do BuildContext são: showDialog e Theme.of. Essas funções podem tanto usar o contexto atual para agir em nome do _widget_ (p. ex., showDialog) como obter informações de determinado contexto (p. ex., Theme.of, para consultar o tema definido em um _widget_ na hierarquia acima).

#### _Widgets_ com e sem estado

Essencialmente, existem _widgets_ com e sem estado, chamados de _stateful_ e _stateless widget_, respectivamente.

Um estado de um _widget_ é uma informação ou grupo de informações que podem ser alteradas ao longo da execução do aplicativo (e essa alteração deve ser exibida).

Imagine clicar sobre um botão de _like_ em um app de rede social. Assim que isso acontece, o ícone muda de transparente para colorido, e ao lado do ícone um contador é incrementado.  

Mas nem todo _widget_ ou tela precisa ter sua informação alterada em tempo de execução. Considere, por exemplo, a tela dos termos de uso, o longo texto que ninguém lê. Não há o que mudar nessa tela, pois ela é estática, e o usuário tem o poder de apenas ler o texto.

Sempre que um conteúdo, cor, forma ou posição de uma parte da tela é fixo e imutável, recomenda-se fortemente utilizar _stateless widget_ na sua construção, tendo em vista que o mecanismo de gerência de estados envolve mais trabalho do _hardware_ do que o _stateless widget_.

A atualização do estado e a renderização do _stateful widget_ requerem mais processamento e a renderização de todos os _widgets_ descendentes do _widget_ alterado na árvore de _widgets_.  

A imagem a seguir traz a comparação da renderizacão do _stateless widget_ e do _stateful widget_.

![[Pasted image 20241026181725.png]]

#### Linguagem Dart

A linguagem Dart, também criada pela Google, é a linguagem de programação usada com os _widgets_ para formar o seu aplicativo.

A linguagem Dart não é usada apenas para o desenvolvimento de aplicativos móveis; ela é uma linguagem de programação de propósito geral. É usada para programar praticamente tudo: aplicações _web_, servidores, _desktop_ e, claro, aplicações.

Na criação de um _widget stateless_, precisamos basicamente de uma classe estendendo a classe _stateless widget_. Já para os _widgets stateful_, precisamos criar mais uma coisa: precisamos também criar uma estrutura que mantenha o estado.

O estado de um elemento basicamente controla o que é mutável nele.

Sempre que uma variável, parâmetro ou similares mudam, automaticamente podemos comunicar ao Flutter que houve essa mudança através do método setState, e ele executará uma reconstrução do _widget_ alterado, atualizando a exibição do _widget_ na tela de acordo com o novo valor do estado.

#### Navegação entre telas e NamedRoute

Na maioria dos casos, um app é composto de várias telas, e, usando botões ou comandos na tela, deve ser possível ao usuário passar de uma tela a outra.  

Em Flutter, usa-se _route_ para denominar uma tela, e o _widget_ Navigator é o elemento usado para gerenciar a navegação entre telas.  

Esse _widget_ trata o conjunto de telas abertas como uma pilha, em que apenas a última tela aberta está visível, mas todas as demais telas (de aplicativos abertos) permanecem empilhadas na ordem em que apareceram na tela. As operações são push() e pop(), para empilhar, ou seja, gerar a tela nova por cima da atual ou, de forma inversa, remover a tela visível. A imagem a seguir traz um exemplo de uma sequência de mudanças de tela.

![[stb4 3 1.png]]

Uma forma bastante comum de controlar a navegação é usando NamedRoutes. Cada NamedRoute é uma tela do seu app que recebe um nome, como, por exemplo, “/A”, “/B”, etc. Então, basta registrar cada uma das _routes_ no atributo MaterialApp.routes, como mostrado a seguir.

![[stb5 2 1.png]]

SecondPage() e ThirdPage() supostamente geram os _layouts_ de cada tela. E, para fazer aparecer as _routes_ A e B (esta sobre a A), basta chamar:

![[stb6 2 1.png]]

#### _Async, await e future_

Em um aplicativo _mobile_, muitas vezes é necessário fazer alguma operação em _background_ que pode ser mais demorada, como, por exemplo, um acesso ao um banco de dados, a espera por algum sensor ou a espera pela resposta por uma chamada-requisição a um servidor remoto. No entanto, para evitar que a interação com o usuário sofra qualquer atraso (o que seria muito ruim para a usabilidade do app), o Flutter se utiliza do conceito de chamada assíncrona de funções que a linguagem Dart provê.

Uma função assíncrona é uma forma de descrever algum resultado futuro, ainda não disponível, e esperar por ele, sem ter que bloquear o fluxo principal (a _thread_) da interface gráfica.

![[stb7 1 1.png]]

Analogamente, utilizar o modelo assíncrono no Flutter significa usar as seguintes três palavras-chave: **_async, await_ e _future_**.  
- O **_async_** determina que um método será assíncrono, ou seja, não irá retornar algo imediatamente. Logo, o aplicativo pode continuar a execução de outras tarefas enquanto o processamento não é finalizado.
- O **_await_** serve para determinar que o aplicativo deve esperar uma resposta de uma função antes de continuar a execução. Isso é muito importante, pois há casos em que uma função depende do retorno de outra.
- O **_future_** determina que uma função irá retornar algo no “futuro”, ou seja, é uma função que levará um tempo até ser finalizada, e o _future_ passa a ser uma promessa de chegada futura do resultado da função.

Ao executar a chamada assíncrona, o controle permanece na UI, fazendo com que o usuário do app não note qualquer atraso ou lentidão na interação. E, quando o método em _background_ terminar, a aplicação pode continuar processando o valor retornado pelo _future_. Para usar _future_, _async_ e _await_, você precisa importar o pacote “dart:asynch”.  

A seguir, veja um exemplo de uma função assíncrona de acesso a um banco de dados.

![[stb8 1 1.png]]

No trecho de código apresentado, estamos determinando que o método getAllContacts() irá retornar uma lista de contatos no “futuro”; por isso o uso do _future_. Além disso, essa função será assíncrona; assim, precisamos indicar na assinatura do método a palavra _async_.  

Ainda, para retornar a lista de contatos, precisamos buscar esses dados de um banco de dados. No entanto, essa consulta não é imediata, levando certo tempo para ser concluída. Para que o Flutter “espere” até que alguma informação seja retornada do banco de dados, utilizamos o _await_, indicando que o restante do método só poderá ser executado quando houver um retorno do método DbUtil.getData('contacts').  

A seguir, veremos que o acesso a um servidor remoto também precisa ser uma operação assíncrona, justamente por ser bem mais demorada do que operações da UI.

#### Acesso remoto usando a API REST/HTTP

Aqui, veremos como seu app pode fazer operações RESTful em servidores remotos. E veremos como o _future_ é usado.  

Por exemplo, no trecho a seguir, é feita uma chamada GET de um elemento, a1, em um endereço _remote_.  

[Clique aqui](https://jsonplaceholder.typicode.com) para acessar o endereço remoto.  

Recebe-se como resultado um JSON que será analisado pelo método _parse_ da classe URI.

![[stb9 2.png]]

O método http.get() retorna um Futuro que vai conter a resposta da chamada. O Futuro é uma classe Dart para trabalhar com chamadas assíncronas.  

Um objeto Futuro representa um valor potencial ou erro que estará disponível em algum momento do futuro, e a classe htt.Response contém os dados recebidos de uma chamada http bem-sucedida. No entanto, trabalhar diretamente com a resposta <http.Response> não é muito prático, então é conveniente converter o http.Responde em um objeto Dart.  

E essa classe (vamos chamá-la de “Album”) deve conter todos os dados que retornam da solicitação da https. Suponhamos que as informações recebidas sejam {userld, Id, title]; assim, a classe também tem os três atributos correspondentes. A classe Album inclui ainda um constructor fabrica, Album.fromJson, que cria uma instância da classe a partir do JSON recebido como argumento (Map<String, dynamic>json).

![[stb10 1 2.png]]

Além desses mecanismos de criação de _layout_ (_widgets_), de navegação (Navigator), de comunicação assíncrona e de acesso _remote_, o Flutter e o Dart fornecem muitos outros conceitos e mecanismos, que iremos resumir a seguir.

#### _Platform channels_

Um _platform channel_ é uma API flexível de mensagens entre um aplicativo Flutter e a plataforma que hospeda o aplicativo.  

É como você pode se comunicar com APIs nativas e de terceiros, por exemplo, para acessar um recurso específico, como a informação sobre o nível da bateria, a partir da plataforma Android.

#### _Streams_

_Streams_ (fluxos) estendem a ideia de processamento assíncrono para dentro do aplicativo; são a base da programação reativa.

Essencialmente, um _stream_ é uma sequência de eventos assíncronos. É como um iterável assíncrono. Em vez de obter o próximo evento quando você solicita, o _stream_ informa que há um evento quando está pronto, e são sequências potencialmente infinitas de eventos (da UI, da rede ou dos sensores locais).  

Observe a imagem:

![[stb11 3 1.png]]

#### Gerenciamento de estados (padrão BLOC)

Os aplicativos Flutter são escritos na linguagem Dart e fazem uso de muitas das características mais avançadas dessa tecnologia. Ao escrever e depurar um aplicativo, o Flutter é executado na máquina virtual Dart, que tem um motor de execução _just-in-time_.

#### Preparando o seu ambiente

Antes de começar a desenvolver o app, você precisa **criar o seu ambiente de desenvolvimento**. Isso inclui o Flutter SDK e a escolha de uma IDE. Uma possibilidade é usar o Eclipse, mas nossa experiência diz que o Visual Studio Code, VS Code, da Microsoft, é o melhor ambiente para desenvolver com Flutter. Depois de instalar o VS Code em seu computador, selecione o Futter _plugin_ para Virtual Studio Code e reinicie o Virtual Studio Code.  

Depois, você precisa instalar o Android Studio para poder usar emuladores Android. Se você também quiser desenvolver logo para iOS, precisará instalar o Xcode Tools da Apple e o emulador de iOS. Se você quiser testar o seu aplicativo diretamente no seu _smartphone_, também pode. Para isso, conecte o seu aparelho por cabo USB no seu _desktop_ ou _notebook_.  

Feito isso, você pode começar a implementação. No Git, no Bitbucket e em outros repositórios, existem vários exemplos (em código aberto) que podem ser usados como ponto de partida para o seu. Portanto, sugiro que você pegue algum exemplo, talvez até de um tutorial do Flutter, e familiarize-se com ele antes de começar a mexer nele, adaptando-o de acordo com aquilo que você imaginou para seu aplicativo.

Lembre-se de que você deverá criar o app paulatinamente, realizando testes a cada modificação e, assim, fazendo melhorias contínuas no seu aplicativo.

Depois, escolha e conecte os _widgets_ de cada tela e, em seguida, implemente o controle de navegação entre elas (como o usuário vai de uma tela para outra). Enquanto faz essa codificação, teste sempre o que já codificou e anote as melhorias necessárias. Se for necessário, programe as notificações sobre eventos assíncronos que aconteceram e qual deve ser a ação gerada em resposta ao _click_ em uma notificação.  

Eu sempre recomendo que inicialmente o desenvolvedor se preocupe em programar bem a interação com usuário, deixando um pouco de lado a estética da UI. Então, quando tudo já estiver funcionando na versão piloto, o desenvolvedor pode consultar o especialista de interfaces de usuário e se preocupar com as questões da paleta de cores, fontes de letras e o **_theme_** em geral.  

O acesso a um serviço em _background_ é relativamente simples, especialmente através da convenção REST sob o protocolo HTTP. Nesse caso, deve-se ver como a API do serviço _back-end_ está implementada, e, naturalmente, precisa-se seguir à risca a convenção de parâmetros de entrada e de saída do método remoto acessado, bem como implementar um tratamento de erros do HTTP. Caso o protocolo API do _back-end_ for REST, toda a interação será na forma de comandos.

### Técnica Aplicada

Para começar, leia este documento sobre o que é ser um desenvolvedor Flutter.

**_What it takes to be a Flutter developer_**  

[Clique aqui.](https://www.section.io/engineering-education/becoming-a-flutter-developer/)

Depois, leia este blog sobre os diferentes ambientes multiplataforma (_cross platforms_).  

[Clique aqui.](https://www.sam-solutions.com/blog/cross-platform-mobile-development/)

E leia e reflita sobre os resultados de um teste de _performance_ entre Flutter, ReactNative e Android.  

[Clique aqui.](https://inveritasoft.com/blog/flutter-vs-react-native-vs-native-deep-performance-comparison)

Se quiser, comece a ler os tutoriais e exemplos e estude a estrutura de um projeto Flutter. [Clique aqui](https://docs.flutter.dev/).

![[Pasted image 20241026193045.png]]

![[Pasted image 20241026193057.png]]

![[Pasted image 20241026193108.png]]

![[Pasted image 20241026193135.png]]

![[Pasted image 20241026193215.png]]

![[Pasted image 20241026193233.png]]

![[Pasted image 20241026193315.png]]

![[Pasted image 20241026193326.png]]

![[Pasted image 20241026193335.png]]

### Referências:

CREATING mobile app wireframes: a step by step guide. **Balsamiq**, 2023. Disponível em: [https://balsamiq.com/learn/articles/mobile-app-wireframing-guide/](https://balsamiq.com/learn/articles/mobile-app-wireframing-guide/). Acesso em: 15 fev. 2023.

## Exemplo de uma aplicação _mobile_ cliente-server usando Flutter (Aula 3)

Durante todos os módulos anteriores, vimos diversos assuntos e tópicos práticos para entender teoricamente conceitos e formas de desenvolvimento de uma aplicação _mobile_ utilizando Flutter. Essas técnicas utilizam ferramentas de desenvolvimento com os ambientes integrados Visual Studio Code (VScode) e Android Studio para **estruturar, programar e testar sistemas e aplicativos _mobile_** destinados a usuários finais em seu dispositivo _mobile_. Os tópicos abordados nas aulas anteriores nos deram a base para que possamos, então, nesta aula desenvolver um aplicativo _mobile_ inicial.

Esta aula terá como foco o **ensino prático do desenvolvimento _mobile_ em Flutter.** Para isso, iremos criar um projeto Flutter que irá revisitar alguns dos principais conceitos vistos nas aulas anteriores, como:
- _context;_
- árvore de _widgets;_
- _widgets;_
- linguagem Dart;
- acesso a APIs REST.

Além disso, também iremos abordar uma parte importante do desenvolvimento de qualquer aplicativo _mobile_, a interação do aplicativo com um servidor _back-end_ que implementa um processamento mais pesado, mais global, e/ou fornece uma base de dados de maior capacidade. Para isso, utilizaremos um servidor _back-end_ implementado na linguagem Dart, que será capaz de se comunicar com o aplicativo por meio de requisições HTTP, por parte de uma API REST simples criada.

Esta terceira aula irá abordar a parte prática de forma iterativa. A intenção é que o aluno seja capaz de implementar em sua própria máquina partes de um código incompleto que será provido para que, dessa forma, possa exercitar os aprendizados vistos nas aulas anteriores e, no fim da aula, ter criado seu primeiro aplicativo Flutter.

### Preparando o ambiente

Nesta aula, iremos fazer um passo a passo de como:
- **configurar o ambiente de programação**, incluindo o Android Studio, o uso de _plugin_ Flutter e a instanciação de um emulador de dispositivo móvel; e
- **mostrar um exemplo de um aplicativo _mobile_ e seu serviço _back-end_ associado** e que interagem entre si através de requisições HTTP, como acontece com muitos sistemas _mobile_.

Será fornecido um código completo da parte _back-end_ e um código da parte cliente _mobile_ com algumas lacunas em branco para que o aluno se exercite ao completar e customizar e para que possa rodar esse sistema em seu computador _desktop_ e possivelmente no seu _smartphone_ (ou, então, no emulador no Android Studio). Assim, espera-se que dessa forma possa exercitar os aprendizados vistos nas aulas anteriores e, no fim da aula, ter criado seu primeiro aplicativo Flutter.

Para fazer o análogo com um dispositivo iPhone, o aluno teria que usar Xcode em seu MacBook, e haveria pequenas diferenças no cadastramento das dependências no projeto do Xcode. Por isso, iremos focar mais na execução do sistema no Android Studio.

O primeiro passo para conseguirmos executar esta aula é preparar o ambiente de desenvolvimento Flutter. Para isso, precisaremos ter os seguintes itens instalados:  
1. Flutter SDK;
2. Android Studio;
3. um emulador de dispositivo ou dispositivo real para testar a aplicação;
4. configurar o _plugin_ do Flutter no Android Studio.

Agora, vamos ao passo a passo de como preparar o ambiente de desenvolvimento Flutter.

#### Instalando o Flutter SDK

A instalação do Flutter varia em cada sistema operacional, e a documentação oficial contém bastante informação detalhada de como seguir em frente.

Você pode encontrar a documentação referente a cada sistema operacional através dos _links_:  
- Windows: [Clique aqui](https://docs.flutter.dev/get-started/install/windows)
- Linux: [Clique aqui](https://docs.flutter.dev/get-started/install/linux)
- Mac: [Clique aqui](https://docs.flutter.dev/get-started/install/macos)

#### Instalando o Android Studio

O Android Studio será a IDE usada para desenvolver o aplicativo, ou seja, através do qual iremos “codar” (escrever os códigos), o que resultará na nossa aplicação.

O Android Studio é uma IDE que já tem um suporte muito bom para criação de aplicações em Flutter, além de conter também o suporte para emuladores de dispositivos, que iremos tratar mais adiante.

Para instalar o Android Studio, é necessário baixar a ferramenta através da página oficial, independentemente do sistema operacional utilizado.  

[Clique aqui](https://www.google.com/url?q=https://developer.android.com/studio/&sa=D&source=docs&ust=1678113760251978&usg=AOvVaw1FduhKiKrbLXQfeX8QOJQ5) para acessar.

#### Criando emulador no Android Studio

Se você não tem um celular configurado para testes, um dos meios para rodarmos a nossa aplicação será através de um emulador. Para isso, o Android Studio permite a criação e o gerenciamento de emuladores dentro da IDE.

![[02 3 2.png]]
![[03 2 3.png]]
![[04 1 3.png]]
![[05 6.png]]

#### Configurando o _plugin_ do Flutter no Android Studio

Agora, para finalizarmos a preparação do ambiente, precisamos instalar o _plugin_ do Flutter no Android Studio, porque o Android Studio é uma IDE genérica, que precisa ser preparada para o uso do Flutter. Para isso, siga os passos:

![[02 4 2.png]]
![[03 3 3.png]]
![[04 2 2.png]]
![[05 1 3.png]]

#### Testando o ambiente

Para verificar se o ambiente de programação Flutter recém-instalado está bem configurado, existe um comando que poderá ser usado. Para isso, abra o seu terminal no Android Studio e execute o comando Flutter doctor.

Como resultado da verificação, todas as etapas devem estar marcadas como completas através de um símbolo _check_ verde.

É importante ressaltar que, mesmo que alguma das etapas contenha uma exclamação em amarelo “!”, isso é considerado apenas um _warning_ e **não** impede a execução da aplicação. No entanto, tanto o teste do Flutter como o do Android Studio devem ter sido aprovados.

### Desenvolvendo o servidor _back-end_

Agora, com o ambiente de desenvolvimento Flutter configurado, podemos finalmente começar a desenvolver nossa aplicação. E, para isso, vamos começar criando nosso servidor _back-end_, que será responsável por receber as requisições do nosso aplicativo mobile e responder a essa requisição com uma mensagem simples: “Hello World”.

Para facilitar, nossa aplicação _back-end_ será muito simples. Será composta apenas por um arquivo, que irá executar um código em Dart (linguagem base do Flutter). Siga os passos indicados a seguir:

![[stb3 4.png]]

Para testar o serviço, tente acessar a página [clicando aqui.](http://localhost:3000/)
#### Desenvolvendo a aplicação _mobile_

O nosso aplicativo _mobile_ também será bastante simples, apenas para “dar um sabor” de como é Flutter. O aplicativo irá conter uma interface GUI com um botão e um campo de texto, que irá exibir a resposta do nosso servidor _back-end_. A interface no final do desenvolvimento deverá ser parecida com a seguinte imagem:

![[stb4 4 1.png]]

Nesta seção, iremos escrever o código inicial e, como forma de desafio, deixaremos alguns pedaços em branco para que você possa completar.

![[02 5 2.png]]
![[03 4 2.png]]
![[04 3 1.png]]
![[05 2 1.png]]

Este será o arquivo que iremos utilizar para montar nossa aplicação. Como já sabemos, o código Flutter deve conter uma classe _main_ que irá conter o _build_ da aplicação e seu primeiro _widget_ inicial, que pertence à classe MaterialApp. Iremos chamar essa classe de MyApp e iremos colocar nela o nosso primeiro componente da nossa árvore de _widgets_, um _widget_ Scaffold.

Relembrando, Scaffold é um _widget_ que pertence à biblioteca ‘_material.dart_’, padrão de aplicações Flutter, e é composto por dois campos: appBar e body. O primeiro representa a barra superior da tela do aplicativo, que pode conter um título, botões e cores customizadas, e o campo body deverá conter todo o resto da tela e pode ser qualquer _widget_.

A seguir, disponibilizamos o código faltando o componente a ser utilizado na parte de appBar. Vamos lá?

![[stb6 4 1.png]]

E aí, conseguiu? A seguir, iremos disponibilizar as respostas de cada código faltando, mas, se você conseguiu fazer, já pode executar seu projeto através do comando Flutter run.

Com o código completo e o servidor rodando, ao executar seu aplicativo e clicar no botão Send request to server, o seu aplicativo deverá alterar o campo de texto contendo a mensagem “Hello World”, como mostra a imagem a seguir.

![[stb7 2 1.png]]

Agora, vamos às respostas.

![[stb8 3 1.png]]

Nesta aula, criamos uma aplicação real contendo dois pontos essenciais de qualquer sistema: a comunicação _front-end (mobile)_ e _back-end_ (servidor). Para esse exemplo, é possível compreender que a simplicidade da execução não exige muito no desenvolvimento, mas, se pensarmos em grandes aplicações e sistemas, existem vários pontos que podem ser levantados:  
1. Quais são as boas práticas de desenvolvimento de aplicações _mobile_?
2. Como podemos utilizar a componentização da GUI na forma de _widgets_ a nosso favor durante o desenvolvimento?
3. Como podemos tratar problemas na comunicação entre _front-end_ e _back-end_? Como tratar os erros de requisições HTTP que falharam?
4. Como podemos dividir nosso código em camadas de comunicação, interface e domínio? O conhecido modelo Model-View-Controller (MVC)  

No suporte ao desenvolvimento de aplicações _mobile_ cada vez mais vêm se desenvolvendo linguagens, conceitos e tecnologias para facilitar a tarefa do desenvolvedor e ao mesmo tempo prover maior qualidade e robustez da aplicação resultante. Acreditamos que Flutter e Dart sejam um par de tecnologias que têm atingido níveis altos nesse objetivo. O que vimos aqui no curso, através dos conceitos centrais e exemplos, é o primeiro passo para que você possa entender como esse desenvolvimento funciona. Porém, é necessário um estudo muito mais aprofundado para o desenvolvimento de aplicativos e sistemas mais complexos, utilizando as boas práticas de engenharia de _software_ e desenvolvimento, que irão ajudar você, desenvolvedor, a atingir seus objetivos de forma mais fácil e competente.

### Técnica Aplicada

Se você deseja continuar a entender mais sobre comunicação HTTP entre aplicações Flutter e servidores, poderá ler mais em:
[Clique aqui.](https://stackoverflow.com/questions/53648545/flutter-not-able-to-make-http-get-request/54915614#54915614)  
  

Para aprender a trabalhar com JSON, comumente usado nessa comunicação, leia:
JSON conversion in Flutter and Dart
[Clique aqui.](https://suragch.medium.com/parsing-simple-json-in-flutter-83ee1809a6ab)  
  

E, se você deseja entender mais sobre servidores e como fazer novos serviços em Dart, pode encontrar mais aqui:
Write HTTP servers
[Clique aqui.](https://dart.dev/tutorials/server/httpserver)

Outros tutoriais de criação de projetos em Flutter para iniciantes podem ser encontrados [clicando aqui.](https://www.devmedia.com.br/hello-world-com-flutter/40321)

Também recomendamos os tutoriais da documentação principal do Flutter, [aqui.](https://docs.flutter.dev/get-started/codelab)

### Referências:

CONHECER o Android Studio. **Google Developers**. Disponível em: [https://developer.android.com/studio/intro/](https://developer.android.com/studio/intro/). Acesso em: 17 mar. 2023.

GET-STARTED. **Flutter**. Disponível em: [https://docs.flutter.dev/get-started/install/](https://docs.flutter.dev/get-started/install/). Acesso em: 17 mar. 2023.

HELLO world com Flutter. **Devmedia**. Disponível em: [https://www.devmedia.com.br/hello-world-com-flutter/40321](https://www.devmedia.com.br/hello-world-com-flutter/40321). Acesso em: 17 mar. 2023.

MINIMAL client-server example for Flutter and server-side Dart. **Suragch**, 2019. Disponível em: [https://suragch.medium.com/minimal-client-serverexample-for-flutter-and-server-side-dart-dc4257903753/](https://suragch.medium.com/minimal-client-serverexample-for-flutter-and-server-side-dart-dc4257903753/). Acesso em: 17 mar. 2023.

PINHEIRO, F. Configurando ambiente de desenvolvimento Flutter. **Treinaweb**, 2020. Disponível em: [https://www.treinaweb.com.br/blog/configurandoambiente-de-desenvolvimento-flutter/](https://www.treinaweb.com.br/blog/configurandoambiente-de-desenvolvimento-flutter/). Acesso em: 17 mar. 2023.

