
![[img01-1.png]]
# Programação Orientada a Objetos (Disciplina 1)
## Python e orientação a objetos (Aula 1)

### Variáveis:

Os principais tipos de variáveis simples, em Python, são: _int_ (inteiro), _float_ (real), _bool_ (booleano, podendo assumir os valores _True_ ou _False_) e _str_ (_string_, ou texto).

Em Python, não existe um comando para declarar uma variável, que é criada no momento em que um valor é atribuído a ela. Também não é necessário declarar os tipos das variáveis, sendo possível, inclusive, convertê-las para outro tipo, posteriormente, por meio de um _casting_. 

Observe alguns exemplos:

![[pos-graduacao/1º Acervo de imagens (Disc. 1)/img02.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/img03.png]]
É possível, ainda, trabalhar com operações matemáticas em Python, usando os operadores básicos soma (+), subtração (-), multiplicação (*), divisão (/), potenciação ( ** ) e resto da divisão (%). Veja alguns exemplos:

![[pos-graduacao/1º Acervo de imagens (Disc. 1)/img04.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/img05.png]]

Já os operadores de igualdade permitem comparar se duas variáveis ou valores são iguais (==) ou diferentes (!=). Os operadores de comparação (>, <, >= e <=) também são muito utilizados para comparar variáveis numéricas. Há, ainda, os operadores lógicos _and_ (e) e _or_ (ou).

As possíveis respostas para os operadores de igualdade e comparação são os valores booleanos _True_ (verdadeiro) ou _False_ (falso). Veja mais alguns exemplos:

![[Pasted image 20250120203056.png]]
![[Pasted image 20250120203118.png]]

### Strings:

As _strings_ armazenam uma ou mais palavras em texto. Existem diversas operações úteis com _strings_, como:
- concatenação de duas ou mais _strings_;
- verificação do tamanho de uma _string_;
- operações envolvendo indexação e _substrings_;
- multiplicação de uma _string_ por um número;
- operador _in_;
- _escaping_;
- conversão para maiúsculas e minúsculas;
- formatação.

#### Concatenação:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/02.png]]
#### Tamanho:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/03.png]]
#### Indexação e substrings:
![[Pasted image 20240515112938.png]]
#### Operador _In_:
![[Pasted image 20240515113044.png]]
#### Formatação:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/09.png]]
#### Maiúsculas e minúsculas:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/08.png]]
#### _Escaping_:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/07.png]]
#### Multiplicação:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/05.png]]
### Coleções:
#### Listas, tuplas e dicionários:
![[Pasted image 20240515113100.png]]
![[Pasted image 20240515113108.png]]
### Condições:
#### Comando if:
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/02 1.png]]
#### Comandos if, elif (else-if) e else:
![[Pasted image 20240515113120.png]]
### Loops:
#### For:
![[Pasted image 20240515111617.png]]
![[Pasted image 20240515111623.png]]
![[Pasted image 20240515111626.png]]
#### While:
![[Pasted image 20240515111702.png]]
![[Pasted image 20240515111704.png]]

#### Break:
![[Pasted image 20240515111742.png]]
![[Pasted image 20240515111744.png]]
#### Continue:
![[Pasted image 20240515111750.png]]
### Funções:
![[Pasted image 20240515111804.png]]
### Códigos & Links:
Aula 1a - https://colab.research.google.com/drive/1XDNXGFyaX7wwHOQWU6vrop1S-r-mk0Qx#scrollTo=VPJhZYydih_M
Aula 1b - https://colab.research.google.com/drive/17VsrVQHsamvpJYooK-GjnyghdNx-P0II#scrollTo=3CNVDcSVClpq

### Referências:

BARRY, P. **Use a cabeça!**: Python. Rio de Janeiro: Alta Books, 2018.  

MUNIZ, A. _et al_. **Jornada Python:** uma jornada imersiva na aplicabilidade de uma das mais poderosas linguagens de programação do mundo. Rio de Janeiro: Brasport, 2022.    

PYTHON SOFTWARE FOUNDATION. The Python tutorial. **Python.org**, [20--?]. Disponível em: [https://docs.python.org/3/tutorial/](https://docs.python.org/3/tutorial/). Acesso em: 10 out. 2022.  

RAMALHO, L. **Python fluente**: programação clara, concisa e eficaz. São Paulo: Novatec, 2015.    

SEVERANCE, C. R. **Python para todos**: explorando dados com Python 3. [_S. I._]: Elliott Hauser e Sue Blumenberg, 2020.  

W3SCHOOLS. Python tutorial. **W3Schools**, [20--?]. Disponível em: [https://www.w3schools.com/python/default.asp](https://www.w3schools.com/python/default.asp). Acesso em: 10 out. 2022.

## Os 4 Pilares da Orientação a Objetos (Aula 2)
### **Paradigmas de programação**
![[Pasted image 20240515111834.png]]

![[Pasted image 20240515111838.png]]

![[Pasted image 20240515111843.png]]
#### Classes e Objetos
![[Pasted image 20240515111912.png]]

Podemos criar vários objetos a partir de uma mesma classe, mas, assim como cada bolo tem um sabor, cada objeto terá sua própria identidade.

![[Pasted image 20240515111921.png]]
![[Pasted image 20240515111923.png]]
É importante destacar que o comportamento de um objeto é definido por sua respectiva classe a partir de métodos, um conjunto de rotinas que operam sobre os dados.

Já o estado de um objeto é definido por sua respectiva classe a partir de variáveis de instância, que representam os dados do objeto.

![[Pasted image 20240515111958.png]]
![[Pasted image 20240515112000.png]]
Mas quais são os pilares da POO?

![[Pasted image 20240515112002.png]]
Em Python, tudo deriva de uma classe, inclusive tipos básicos, como números (por exemplo, _int_) e textos (por exemplo, _str_). Veja o que acontece quando executamos o comando help(_int_):

Observe que o tipo _int_ deriva da classe _int_, que, por sua vez, herda da classe _object_ os atributos e métodos comuns a todas as classes.

![[half-img-5.png]]
Nessa linguagem, as classes podem ser definidas em qualquer lugar, inclusive dentro de funções.
![[Pasted image 20240515112029.png]]
![[Pasted image 20240515112031.png]]
![[Pasted image 20240515112034.png]]
#### Métodos
Dentro das classes, é possível definir os métodos que representam as ações que os objetos criados a partir delas poderão realizar.

Um método recebe pelo menos um parâmetro: a instância da classe, representada pela palavra reservada _self_. Esse parâmetro permite saber a que instância se referem os atributos.

Na declaração do método, é preciso declarar _self_ explicitamente, mas, ao chamar o método em um objeto, _self_ é passado automaticamente.

O parâmetro _self_ pode ter outro nome, mas _self_ é uma convenção (padrão PEP8). Métodos podem receber qualquer quantidade de parâmetros, que podem ser obrigatórios ou não (declarados com um valor _default_).

Vamos a um exemplo?

Definimos uma classe _Pessoa_, que tem dois métodos:

- __ _init_ __ , que inicializa o atributo nome durante a criação da instância; e
- __ _str_ __ , converte uma _Pessoa_ para _string_. Observação: quando passamos um objeto para o comando _print_, este vai buscar pelo método __ _str_ __ para saber como representar o objeto na saída padrão.

![[Pasted image 20240515112059.png]]
As variáveis _pessoa_1_ e _pessoa_2_ referenciam instâncias (objetos) da classe _Pessoa_, com valores distintos para o atributo _nome_.

Para chamar um método em um objeto, basta escrever os nomes da variável que o referencia e do método separados por um ponto, passando os parâmetros cabíveis. No exemplo, estamos chamando os métodos _soma_ e _media_ no objeto referenciado por _minha_lista_.
![[Pasted image 20240515112109.png]]
#### Atributos
Existem três tipos de variáveis que podem ser declaradas dentro de uma classe:

**Atributos de Classe:**
São atributos ligados à classe, e todas as instâncias da classe compartilham o mesmo atributo.

**Atributos de Instância:**
São específicos para cada instância, podendo ter valores diferentes de uma instância para outra.

**Variáveis de métodos:**
Existem apenas enquanto a função está sendo executada.

![[Pasted image 20240515112134.png]]
![[Pasted image 20240515112136.png]]
![[Pasted image 20240515112137.png]]
#### Encapsulamento
Como vimos anteriormente, **o encapsulamento é um recurso da orientação a objetos que permite agrupar um código e os dados por ele manipulados em uma única entidade, protegendo-os de interferências externas, acesso indevido e/ou utilização/modificação inadequada** por outro trecho de código definido fora do código encapsulado.

![[Pasted image 20240515112235.png]]
Em OO, é uma boa prática tornar os atributos privados, uma vez que é responsabilidade de cada classe controlar seus atributos.

Para isso, algumas linguagens utilizam o conceito de palavras-chave para definir o nível de visibilidade, e Python considera que existem os tipos _public_ e _non-public_. Para marcar como _non-public_, usam-se dois _underscores_ (__) antes do nome do atributo ou método.

Não se usa o termo _private_ para Python, pois nenhum atributo é de fato mantido como _private_. É apenas exibido um alerta de que você não deveria estar tentando acessá-lo. Apesar de ser possível acessar e até alterar o valor de um atributo _non-public_ em Python, isso não é uma boa prática.

Vale ressaltar que as mesmas regras de acesso para atributos valem para métodos. Como boa prática, os atributos de instância são _non-public_ e a maioria dos métodos, _public_. Isso possibilita que a conversa entre objetos seja feita por troca de mensagens, ou seja, acessando seus métodos, em vez de um objeto manipular diretamente atributos que não sejam seus.

#### Herança
A herança permite que as características e os comportamentos descritos de uma classe “pai” (superclasse) sejam herdados por sua classe “filha” (subclasse).

![[Pasted image 20240515112248.png]]
Uma relação de herança significa que a subclasse herda os membros da superclasse (atributos e métodos).

Estas são as principais vantagens da utilização da herança:

- Evita código duplicado.
- Facilita a manutenção, pois há apenas um lugar para fazer alterações em caso de modificações (superclasse), sem precisar modificar as subclasses.
- Possibilita definir um protocolo comum para um grupo de classes relacionadas.
- Garante que todas as subclasses, tanto atuais como futuras, de uma superclasse tenham os mesmos métodos que serão herdados.
- Permite estabelecer um “contrato” mínimo do que as subclasses – em qualquer nível – poderão fazer.

Fique atento à utilização da herança:

![[STB9_Aula2_ImagemCustomizada.jpg]]

![[Pasted image 20240515112318.png]]
#### Polimorfismo
Para falar de polimorfismo, vamos retomar um exemplo:

![[Pasted image 20240515112324.png]]
Polimorfismo é a capacidade de um objeto poder ser referenciado de várias formas (o que não significa que o objeto pode se transformar em outro tipo).

Se tivermos um método que espera receber um objeto do tipo _Pessoa_, ele pode receber, em vez disso, um objeto do tipo _Aluno_ ou do tipo _Professor_.

O polimorfismo é um recurso que permite projetar códigos com alto nível de abstração (pensando em superclasses), sem se preocupar com níveis mais baixos (subclasses), que poderão, inclusive, ser criados posteriormente. Isso permite a criação de um código flexível, simples e de fácil manutenção. Usando o polimorfismo, é possível diminuir o acoplamento entre as classes, evitando que modificações no código resultem em modificações em outros lugares também.
#### Abstração
Ainda analisando o exemplo anterior, repare que não faz sentido termos em nosso sistema uma classe _Pessoa_, pois os usuários serão de tipos específicos, como _Aluno_, _Professor_, _Coordenador_, etc., mas nunca tão genéricos como _Pessoa_.

Entretanto, se a classe _Pessoa_ for removida do programa, perderemos duas importantes vantagens: o reuso de código entre as subclasses de _Pessoa_ e a flexibilidade de termos argumentos polimórficos nos métodos. A solução, então, é tornar _Pessoa_ uma classe abstrata, significando que ela nunca poderá ser instanciada.

Em Python, uma classe abstrata deve conter pelo menos um método abstrato, e podemos criar uma classe abstrata herdando da superclasse para classes abstratas _ABC (abstract base classes)_, do módulo _abc_. Para tal, deveremos importar este módulo no nosso código, como no exemplo a seguir.

![[Pasted image 20240515112332.png]]
Não é possível instanciar uma subclasse de uma classe abstrata sem implementar todos os seus métodos abstratos. Ao tornar um método abstrato, ele deverá ser obrigatoriamente implementado em todas as subclasses de uma classe abstrata.

#### Associação, agregação e composição
**Os conceitos de associação, agregação e composição permitem o relacionamento entre objetos.**

Para você entender melhor, vamos relembrar o exemplo da classe _Aluno_. Imagine que você queira ampliar essa classe para guardar seu professor orientador:

![[Pasted image 20240515112350.png]]
![[Pasted image 20240515112352.png]]
![[Pasted image 20240515112353.png]]
Agora, imagine que o aluno tenha um histórico de ocorrências, como data de matrícula, notas obtidas, disciplinas cursadas e reprovações, entre outras. Nesse caso, temos um exemplo de **composição.**

Tanto a agregação quanto a composição são relacionamentos todo-parte.

**Agregação -** Aqui, o objeto que compõe o todo tem uma parte do tipo de outro objeto e ambos podem existir separadamente. Por exemplo: revista e artigo.

**Composição -** Aqui, se o objeto que representa o todo deixar de existir, o objeto que é uma parte relacionada a ele também deixará de existir. Por exemplo: livro e capítulo.

### Códigos & Links:
Aula 2a - https://colab.research.google.com/drive/13Y9GYnxhQfQ_yylefIZlEZeC13Rf2GG2
Aula 2b - https://colab.research.google.com/drive/1Xs4sk20398-kUiPuS5QLdv11zN1jjtRz#scrollTo=CSZRYxDHyzAS

### Referências:

BARRY, P. **Use a cabeça!**: Python. Rio de Janeiro: Alta Books, 2018.

MUNIZ, A. _et al_. **Jornada Python**: uma jornada imersiva na aplicabilidade de uma das mais poderosas linguagens de programação do mundo. Rio de Janeiro: Brasport, 2022.

PYTHON SOFTWARE FOUNDATION. The Python tutorial. **Python.org**, [20--?]. Disponível em: [https://docs.python.org/3/tutorial/](https://docs.python.org/3/tutorial/). Acesso em: 10 out. 2022.

RAMALHO, L. **Python fluente**: programação clara, concisa e eficaz. São Paulo: Novatec, 2015.

SEVERANCE, C. R. **Python para todos**: explorando dados com Python 3. [_S. I._]: Elliott Hauser e Sue Blumenberg, 2020

W3SCHOOLS. Python tutorial. **W3Schools**, [20--?]. Disponível em: [https://www.w3schools.com/python/default.asp](https://www.w3schools.com/python/default.asp). Acesso em: 10 out. 2022.

## Boas Práticas de Orientação a Objetos e de Codificação em Python (Aula 3)
### Princípios SOLID
Os princípios SOLID têm como objetivo ajudar a realizar um bom projeto de OO para um _software_ de código flexível, escalável, sustentável e reutilizável. SOLID é um acrônimo dos cinco princípios:

- _Single responsibility principle_ (SPR) – Princípio de responsabilidade única
- _Open/closed principle_ (OCP) – Princípio do aberto/fechado
- _Liskov substitution principle_ (LSP) – Princípio da substituição de Liskov
- _Interface segregation principle_ (ISP) – Princípio de segregação de interface
- _Dependency inversion principle_ (DIP) – Princípio da inversão de dependência

_***(1ª VERSÃO)***_
#### Single-Responsibility Principle (SPR)
![[02 10.png]]
![[03 10.png]]
#### Open/Closed Principle (OCP)
![[04 7.png]]![[05 5.png]]
#### Liskov Substitution Principle (LSP)
![[06 2.png]]
![[07 2.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/08 1.png]]
#### Interface Segregation Principle (ISP)
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/09 1.png]]
![[10 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/11.png]]
#### Dependency Inversion Principle (DIP)
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/12.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/13.png]]

_***(2ª VERSÃO)***_

![[pos-graduacao/1º Acervo de imagens (Disc. 1)/02 2.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/03 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/04.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/05 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/06.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/07 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/08 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/09 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/10.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/11.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/12.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/13.png]]
### Guia de Estilos
Com a finalidade de manter seu código organizado e fácil para que outros programadores (ou até você mesmo) possam compreender e dar manutenção, recomenda-se que um bom programador siga boas práticas para escrever seus códigos. Com o objetivo de concentrar práticas recomendadas para escrever e manter códigos de forma organizada, o criador do Python - Guido Von Rossum - é o principal autor do guia de estilos da linguagem Python.
![[Pasted image 20240515120436.png]]
![[Pasted image 20240515120451.png]]
Conforme descrito na PEP-1, as PEPs podem ser:  
- **de padrões** – descrevem novos recursos ou implementações de Python;
- **informacionais** – problemas de _design_ ou orientações gerais para a comunidade;
- **de processos** – processos do Python.
É importante destacar que todas as PEPs são indexadas pela PEP-0.
Além da PEP-0, algumas outras PEPs são interessantes.

_***(1ª VERSÃO)***_
![[01 9.png]]
![[02 1 2.png]]
![[03 1 2.png]]

_***(2ª VERSÃO)***_

![[pos-graduacao/1º Acervo de imagens (Disc. 1)/01 1.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/02 3.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/03 2.png]]
### _Layout_ de códigos
O primeiro pensamento do Zen do Python é _Beautiful is better than ugly_, ou seja, bonito é melhor que feio. Isso significa que a formatação de um código está diretamente relacionada ao seu entendimento.  
![[Pasted image 20240515120627.png]]
![[Pasted image 20240515120635.png]]
![[Pasted image 20240515120644.png]]
![[Pasted image 20240515120705.png]]
### Nomenclatura
O segundo pensamento do Zen do Python é _Explicit is better than implicit_, em português explícito é melhor que implícito. Isso significa que a clareza quanto ao que queremos desenvolver em um bloco de código é muito importante, o que inclui nomear as variáveis, as funções, as classes e os pacotes de forma clara e consistente.

![[STB04 4.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/STB04.png]]

Observação: evite utilizar letras únicas como I ou O para definir uma variável, pois podem ser facilmente confundidas com 1 ou 0, por exemplo:
![linha um zero igual a sete cerquilha isto pode parecer que estamos tentando atribuir sete a zero](https://static.plataforma.grupoa.education/pucrio/pucrio/811096/1f63f487-4d65-4793-89be-344b66172df9/content/img/artesdg/texto.png)

### Comentários
Outro pensamento do Zen do Python relacionado ao guia de estilos é _If the implementation is hard to explain, it's a bad idea_, ou seja, se a implementação é difícil de explicar, é uma má ideia. 

Isso reforça a importância de o programador sempre documentar de forma objetiva e precisa o seu código, o que facilita a sua manutenção e interoperabilidade.
![[STB05-1.png]]

### Clean code
A expressão _clean code_, em português “código limpo” se popularizou com o livro de Robert C. Martin _Clean Code: A Handbook of Agile Software Craftsmanship_, publicado em 2008.

Este livro reforça que mesmo um código ruim pode funcionar, mas ele terá, provavelmente, legibilidade ruim, aumentando sua complexidade e custo de manutenção. Assim, **as boas práticas de um código limpo consistem em instruções direcionadas ao modo como escrevemos nosso código**, incluindo as técnicas identificadas como as melhores para realizar determinada tarefa.

Que tal conhecer essas boas práticas direcionadas para códigos em Python, que complementam ou reforçam as orientações de guia de estilos apresentadas anteriormente?
![[Pasted image 20240515121010.png]]
![[Pasted image 20240515121022.png]]
![[Pasted image 20240515121034.png]]
![[Pasted image 20240515121046.png]]
![[01 1 3.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 1)/01.png]]
![[Pasted image 20240515121250.png]]
![[Pasted image 20240515121252.png]]
![[Pasted image 20240515121255.png]]

### Códigos & Links:
Aula 3a - https://colab.research.google.com/drive/14RDGQxNUC4FKcoMSYCMFWJ6oBNKU0dP1
Aula 3b - https://colab.research.google.com/drive/1ysDNLXY5vYwE8B3GiAgl0FJ4LGEKlHe8
Python Enhancement Proposals (PEP 0) - https://peps.python.org/pep-0000/
Style Guide for Python Code (PEP 9) - https://peps.python.org/pep-0008/#naming-conventions
Docstring Conventions (PEP 257) - https://peps.python.org/pep-0257/
Investigating the Impact of SOLID Design Principles on Machine
Learning Code Understanding - https://arxiv.org/pdf/2402.05337

### Referências:

BARRY, P. **Use a cabeça! Python**. Rio de Janeiro: Alta Books, 2018.  

KALINOWSKI, M.; ESCOVEDO, T.; VILLAMIZAR, H.; LOPES, H. **Engenharia de Software para Ciência de Dados:** Um guia de boas práticas com ênfase na construção de sistemas de Machine Learning em Python. Editora Casa do Código, 2023.  

MUNIZ, A. _et al_. **Jornada Python:** uma jornada imersiva na aplicabilidade de uma das mais poderosas linguagens de programação do mundo. Rio de Janeiro: Brasport, 2022.  

RAMALHO, L. **Python fluente:** programação clara, concisa e eficaz. São Paulo: Novatec, 2015.  

SEVERANCE, C. R. **Python para todos:** explorando dados com Python 3. Editora Independente, 2020.  

THE PYTHON Tutorial. **Python**, c2001-2022. Disponível em: [https://docs.python.org/3/tutorial/](https://docs.python.org/3/tutorial/). Acesso em: 2 nov. 2022.

# Banco de Dados (Disciplina 2)
## Fundamentos, Modelos, Arquiteturas de Sistemas e SQL Básico (Aula 1)

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/01.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/02.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/03.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/04.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/05.png]]
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/06.png]]

### Sistemas de Bancos de Dados
É verdade que muitas pessoas se referem aos bancos de dados como um “bando” de dados: um **conjunto de dados relativamente organizado e estruturado para satisfazer algumas demandas de aplicações específicas**. É o caso de aplicações contábeis que usam muitas planilhas de cálculo ou ainda quando nos referimos à gestão de coleções pessoais de livros ou fotografias. Os bancos de dados computacionais envolvem não apenas os dados em si, mas também, e principalmente, os **Sistemas Gerenciadores de Bancos de Dados (SGBD)**, que permitem administrar, consultar e atualizar os dados com segurança, eficácia e eficiência. Podemos, assim, chamar de sistemas de bancos de dados aquelas aplicações contemplando dados e algum SGBD.

Para explicar o que são bancos de dados, é bom começar pelo conceito de modelo de dados, fundamental para a compreensão dos sistemas de bancos de dados existentes. Normalmente é dada ênfase ao modelo de dados relacional, padrão de fato e de mercado na maioria dos sistemas existentes. Entretanto, muitas das definições e termos aqui citados se aplicam aos modelos de dados em geral, inclusive os não relacionais.

Cabe observar que apenas os chamados modelos de dados lógicos, que contemplam tanto a estrutura quanto a forma de manuseio dos dados, são considerados modelos de dados por completo. É preciso contemplar as duas coisas: por exemplo, o **Modelo de Entidades e Relacionamentos (MER)**, proposto por Peter Chen em 1976 e que veremos em outro momento deste curso, é um modelo conceitual de dados, e contempla apenas a parte de representação da estrutura dos dados, sem oferecer mecanismos para seu manuseio. A figura abaixo traz um exemplo dos artefatos presentes no MER em sua representação diagramática. Temos duas entidades (Pessoas e Automóveis) e um relacionamento (Possuem), relacionando elementos (ou ocorrências) de pessoas e automóveis entre si. Os números 1 e N são cardinalidades (no caso, máximas) do relacionamento, que ajudam na compreensão dos conceitos presentes. Nesse caso, a leitura é “Pessoas podem ter mais de um (N) automóvel, mas cada automóvel pertence a apenas uma pessoa de cada vez”.
![[img01.png]]
### Modelos de Dados
No caso específico da literatura de bancos de dados, o foco recai no que se costuma chamar de **modelos lógicos de dados** **_(logical data models)_**, que podem ser efetivamente implementados em sistemas computacionais. Na maioria das vezes, quando se utiliza o termo modelo de dados, a referência é um modelo lógico de dados. Assim, exceto quando for necessária a distinção, será utilizado de agora em diante apenas o termo modelo de dados.

Podemos definir um modelo de dados como um formalismo matemático que contém duas partes:
![[Pasted image 20240515170035.png]]
### Modelo de dados relacional
O modelo relacional (_relational data model_) contempla as duas partes que compõem qualquer modelo de dados: **estrutura**, no caso relações matemáticas, e o **manuseio** por meio de linguagens (por exemplo, SQL ou álgebra relacional) projetadas para estruturas relacionais.

É importante apontar logo para uma interpretação errada que se dá ao termo “relacional” deste modelo lógico de dados. Certamente não diz respeito ao fato de que representaria os relacionamentos sobre os dados do banco, pois, na verdade, todo modelo de alguma maneira especifica a forma como os dados se relacionam. Na verdade, o modelo foi assim nomeado pois **sua estrutura se baseia em abstrações matemáticas chamadas de relações**. Além disso, acredita-se que esta incompreensão quanto ao nome do modelo também seja motivada pela ubiquidade do modelo conceitual de entidades e relacionamentos, proposto depois do modelo relacional, e pela falta de distinção que muitos fazem entre os termos relação (_relation_) e relacionamento (_relationship_).
#### Estrutura do modelo de dados relacional
A parte estrutural do modelo relacional é baseada no conceito matemático de relações, que tem, por sua vez, muitas semelhanças com o conceito matemático de conjunto. Como será visto, muitas das operações sobre relações são oriundas da teoria de conjuntos, e por isso mesmo o modelo é dito **orientado aos conjuntos** **_(set-oriented)_**.

Uma relação pode ser enxergada ou representada como uma tabela com linhas e colunas, cujos elementos são as linhas. Alternativamente, pode-se visualizar uma relação como um conjunto de colunas, quando o foco se dá nos domínios das colunas, ou atributos representados. Mais formalmente, um elemento de uma relação é chamado de **tupla**, que é representada como uma linha de uma tabela. Uma tupla é um **conjunto não ordenado de valores, um para cada coluna**. Cada valor é derivado do seu domínio apropriado. Uma relação pode ser vista como um conjunto de tuplas, ou um conjunto de linhas. Colunas numa tabela são, formalmente, **atributos** nas relações. Para facilitar a compreensão da noção das tuplas ou t-uplas, se fossem duas ou três colunas poderíamos dizer duplas ou triplas, respectivamente.
![[pos-graduacao/1º Acervo de imagens (Disc. 2)/img02.png]]
A partir deste ponto, **vamos utilizar os termos “relação” e “tabela” como sinônimos**. Pode-se dizer também que tabelas (ou o formato tabular de linhas e colunas) são uma forma de abstração adequada para representar o conceito matemático de relações. É fato que, na prática dos sistemas computacionais relacionais, a grande maioria dos desenvolvedores costuma utilizar muito mais o termo tabela do que o termo relação, pois a associação visual de certa forma facilita a comunicação. Porém, veremos que relações são tabelas com propriedades bem específicas.

Cada linha ou tupla de uma relação representa fatos que desejamos guardar ou registrar no banco de dados. As linhas, ao contrário de tabelas ou planilhas em geral, não têm identificação externa ou numeração. **Tuplas numa relação não são ordenadas**, mesmo que pareçam estar em alguma ordem quando apresentadas em sua abstração tabular. Consequentemente, não se pode falar de linha de número 1 ou 3, mesmo que possa parecer, visualmente, que uma das linhas é a primeira e a outra a terceira. É verdade que, se tivermos acesso aos detalhes internos da implementação de uma tabela, saberemos que existe alguma ordem no seu armazenamento interno. Entretanto, no mundo relacional, **qualquer tupla numa tabela pode ser considerada como a “primeira” tupla**, e seja qual for a ordem o significado daquela tabela sempre será o mesmo. Na figura abaixo, temos duas representações da mesma tabela PESSOAS. As tuplas são idênticas, com quatro linhas em ordem diferente, mas contendo essencialmente a mesma informação em cada uma delas.

![[img03-1.png]]
Os atributos de uma relação, ou as colunas de uma tabela, também não são identificados por sua ordem ou posição. É possível identificar por seu nome (de atributo ou coluna) ao qual normalmente há uma semântica associada, além de um domínio de valores válidos. A ordem das colunas é arbitrária, isto é, **há uma ordem relativa entre as colunas de uma relação, mas podemos trocar as colunas de posição sem prejuízo à interpretação de cada um dos seus elementos** (linhas ou tuplas).

A ordenação dos atributos numa relação R (A1, A2, ..., An) com N atributos pode ser qualquer, mas deve ser definida, e os valores em cada tupla t = <v1, v2, ..., vn>, onde v1 ∈ A1, ... vn ∈ An são considerados ordenados.

Na figura apresentada anteriormente, temos duas ordenações de colunas distintas, e qualquer uma das duas poderia ser usada. Uma vez definida a posição, tanto o SGBD quanto os usuários do sistema de banco de dados poderão fazer referência às ordens respectivas. Pode-se dizer, por exemplo, que Nome é a 1ª coluna, enquanto Telefone é a 3ª coluna.

#### Definindo relações
Os elementos de uma relação podem ser formados por um subconjunto do produto cartesiano dos domínios de valores associados aos atributos. Cada domínio é usado com um papel específico, muitas vezes explicitado por seu nome. Os valores de uma coluna denominada CPF, por exemplo, costumam pertencer ao domínio dos números naturais. Porém, dada a semântica particular de um CPF, apenas alguns valores devem ser considerados válidos — deve haver, por exemplo, no máximo 11 dígitos, seguindo um algoritmo específico da Receita Federal Brasileira que determina números válidos, em particular para os dois últimos conhecidos, como dígitos verificadores.

Se considerarmos outras colunas e seus domínios respectivos, como, por exemplo, nomes típicos de pessoas {‘Maria’, ‘Carla, ‘Alberto’...} e telefones com DDD {.(71) 58259-0066, (64) 25721-7650.}, juntamente com o atributo CPF, cada linha da tabela é, na verdade, formada por uma possível combinação do valor de cada domínio, representando pessoas específicas.

Logo, as linhas de uma tabela formam um subconjunto do produto cartesiano dos domínios de cada coluna. No caso da tabela PESSOAS, há um valor para Nome, outro para CPF e um valor para Telefone. Na figura abaixo, temos outros exemplos de domínios de valores para a tabela AUTOMÓVEIS. Nesta ordem, uma linha da tabela poderia ser explicitada por (Renault, Sandero, 2021, França), combinando-se alguns dos valores presentes nos domínios dos atributos neste caso.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/img04.png]]
#### Outras características de relações

As relações, assim como os conjuntos, não têm elementos repetidos. Como as linhas de uma tabela no modelo relacional não têm identificação própria, só podemos nos referir às tuplas pelos valores em seus atributos. Dadas duas tuplas, teremos valores distintos em pelo menos um dos seus atributos. Se olharmos apenas para as colunas, independentemente das tuplas, podemos ter valores repetidos. Apenas **as linhas são, e devem ser, diferentes umas das outras**.

Os valores em cada coluna de uma linha em uma tabela são todos considerados atômicos ou indivisíveis. Isto quer dizer que, para cada atributo de cada tupla, não temos representação multivalorada. Veja o exemplo na figura abaixo: se uma pessoa tem mais de um telefone, é preciso utilizar mais de uma linha para registrar esta informação na tabela, repetindo o nome e o CPF da pessoa em cada linha, que conterá apenas um dos telefones de cada vez.

Observe que podemos ter nomes completos de pessoas, incluindo os sobrenomes, mantendo a característica de atomicidade do atributo: não se trata de termos três nomes, mas sim nomes compostos de mais de uma cadeia de caracteres alfabéticos, o que é perfeitamente aceitável para tabelas no modelo relacional. É provável que haja uma quantidade máxima de caracteres permitida para os valores da coluna Nome, e essa poderia ser a única restrição verificada pelo SGBD.

![[img05 1.png]]
Todo domínio de valores no modelo relacional contém um valor especial, chamado de **NULO** **(ou** **_NULL_** **)**. Ele é usado para representar valores para colunas numa tabela que são desconhecidos, às vezes temporariamente, ou que não se aplicam ao contexto do banco de dados em utilização. No modelo de dados relacional, temos esquemas bem definidos e precisamos de valores para todos os atributos em todas as linhas da tabela. Por sinal, esta é uma das críticas do modelo por parte daqueles adeptos dos sistemas ditos NoSQL (_Not Only SQL_) ou não relacionais. Para os esquemas relacionais, podemos considerar como _NULL_ aqueles valores que não se aplicam para algumas tuplas da relação, ou que talvez não sejam temporariamente conhecidos no momento de incluir os dados na tabela.

No passado relativamente recente, por exemplo, num banco de dados envolvendo pessoas registravam-se as colunas Telefone Fixo e Telefone Celular. Entretanto, são poucas as pessoas que ainda dispõem de um número específico residencial. Assim, pode-se atribuir o valor _NULL_ nesta coluna do Telefone Fixo em cada tupla que corresponda a uma pessoa que não tem telefone fixo, tendo ela celular ou não.

Vale atentar para o fato de que **o valor** **_NULL_** **não é valor substituto para “espaço em branco”, muito menos para o número zero!** Tanto os espaços em branco quanto os zeros têm semântica própria e podem ser úteis de maneira geral, além de não serem naturalmente valores pertencentes a qualquer domínio.

Na figura abaixo, temos um exemplo para a tabela AUTOMÓVEIS, em que para uma das tuplas não sabemos o Ano e País, e há uma outra tupla contendo Fabricante, Ano e País, mas sem o detalhe do Modelo.
![[img06.png]]

### Esquemas de bancos de dados relacionais

Estamos agora em condições de definir “banco de dados relacional”: **trata-se de um conjunto de uma ou mais relações, ou tabelas, e suas restrições de integridade**.

Seja R (A1, A2, .........., An) uma relação com n atributos, ou seja, cada linha de R conterá n colunas. R é chamado de esquema da relação, enquanto uma instância de R é um conjunto específico de valores usados para popular a tabela R.

Um esquema relacional refere-se ao conjunto de esquemas de todas as tabelas de um banco de dados relacional. Basta uma única relação para o banco ser considerado relacional, mas, normalmente, temos várias tabelas compondo um banco de dados. Como visto na abaixo, por exemplo, num banco de dados sobre o mercado automobilístico poderíamos ter um esquema relacional contendo algumas tabelas envolvendo automóveis, revendedoras, pessoas e os negócios envolvendo pessoas que compram automóveis em certas revendedoras.

Na figura abaixo, temos por exemplo o esquema da relação Automóveis, com seis atributos: Código, Fabricante, Modelo, Ano, País e Preço_tabela.
![[img07 1.png]]
Para podermos saber quais tabelas temos num determinado banco de dados relacional, existe a noção de **banco de metadados**, ou **metabanco de dados**, ou ainda catálogo do banco de dados. Trata-se de um “banco de dados sobre o banco de dados”, daí o termo meta. Ele contém a descrição de todas as tabelas, com seus esquemas detalhados — colunas, domínios e restrições de integridade.

Nos metadados, também temos representados quais usuários existem, as respectivas autorizações de acesso — quais tabelas podem ser vistas ou alteradas — além de algumas estatísticas importantes, como o total de tuplas em cada relação e a distribuição de valores em cada coluna, entre outras. Em bancos de dados volumosos, o fato de termos estatísticas atualizadas sobre alguns dados relevantes pode tornar mais fácil responder algumas consultas. No caso do banco sobre mercado automobilístico (vide figura acima), por exemplo, não seria preciso acessar a instância da tabela de automóveis propriamente dita para saber quantos carros estão presentes, pois bastaria consultar o catálogo e buscar as informações da tabela.
![[img08.png]]
Cabe observar que o banco de metadados de um banco de dados relacional também é relacional, ou seja, também é composto de relações que dizem respeito aos objetos relacionais do banco de dados em si. Nos metadados do SGBD PostgreSQL (figura acima), por exemplo, encontraremos uma tabela com a lista de tabelas existentes no banco (pg_class), uma outra tabela com as colunas de cada tabela (pg_attribute), e assim por diante. A vantagem é que o manuseio do catálogo é feito da mesma maneira que para as tabelas do banco de dados em si.

#### Esquemas _versus_ instâncias

É importante diferenciar a noção de modelos de dados dos esquemas respectivos. Do ponto de vista dos modelos, um esquema é uma de suas instâncias, ou um caso particular do modelo. Assim, existe o modelo relacional, cuja estrutura é baseada em relações matemáticas ou tabelas, e existem diversos esquemas relacionais, definidos para cada aplicação distinta. Poderíamos, por exemplo, ter um esquema sobre o mercado automobilístico (vide figura), outro sobre uma universidade (com tabelas sobre cursos, alunos, turmas e professores) e ainda outro sobre empresas (tabelas representando empregados, projetos e departamentos, entre outros).

Analogamente, para cada tabela de um banco de dados relacional temos as respectivas instâncias, a saber, o conjunto de dados propriamente ditos. O esquema da tabela contempla principalmente suas colunas e domínios de valores válidos. Já uma instância desta tabela é o conjunto de dados válidos para aquele esquema naquele instante. A instância é uma relação com dados.

Na figura abaixo, temos um esquema relacional que diz respeito a cervejas, incluindo tanto pessoas que gostam de certas marcas específicas quanto os bares que vendem as determinadas marcas que podem manter a frequência das pessoas com potencial para serem seus clientes. O esquema deste banco de dados relacional não poderia ser mais simples: são duas tabelas, cada qual com duas colunas. Todos os dados são palavras ou strings (cadeias de caracteres) alfabéticos ou alfanuméricos. Para ilustrar, temos alguns dados nas duas tabelas que exibem a instância corrente para efeito de consultas.
![[img09.png]]

Normalmente, esquemas mudam menos do que instâncias. Pode acontecer de querermos acrescentar ou retirar uma coluna de uma tabela, ou ainda acrescentar novas tabelas por completo, mas mesmo assim não seria algo frequente. Já as instâncias, como representam os dados válidos, podem mudar diariamente, ou até mesmo várias vezes ao dia. Numa universidade, por exemplo, os alunos de uma turma mudam a cada trimestre ou semestre, mas o esquema da tabela de nome Alunos se mantém inalterado. No mercado automobilístico, novos carros surgem e outros tradicionais são descontinuados, e preços de tabela também mudam com o tempo, trazendo mudanças para a instância do BD Carros. Analogamente, os bares estão sempre com novidades no cardápio de cerveja, que, por sua vez, vão trazer novos apreciadores e, consequentemente, alterar a instância do BD Cervejas.

#### Manuseio de dados no modelo relacional
A preocupação inicial de Ted Codd quando propôs o modelo de dados relacional dizia respeito ao uso de relações como a estrutura de representação dos dados em alto nível, sem que fosse necessário ao usuário do sistema saber como relações seriam implementadas na prática. Porém, para que se mostrassem úteis, relações teriam que ser manuseadas de tal forma que consultas e operações sobre os dados permitissem responder perguntas relevantes e significativas sobre eles.

Assim, considerando relações como os únicos objetos existentes para representar os dados num sistema de bancos de dados relacional, mostra-se necessário dispor de uma Linguagem de Manuseio de Dados (LMD, ou _Data Manipulation Language_ — DML) fechada sobre relações. Isto é, uma linguagem relacional, em que uma ou mais relações correspondem à entrada (_input_) e a saída (_output_) seja uma nova relação.

![Esquema com três elementos, dentro de um retângulo cinza claro. À esquerda com o título Tabelas Input, três tabelas, uma abaixo da outra. Elas têm 3 colunas e 4 linhas e estão vazias. Flechas azuis direcionam para o segundo elemento. Ele é um retângulo azul na vertical. Na parte de cima: SGBD. Abaixo, um cilindro dividido em três partes na horizontal com uma engrenagem à frente. Mais abaixo: Sistema de BD. Uma flecha azul direciona para o terceiro elemento de título: Tabela Output. Abaixo uma tabela de 3 colunas e quatro linhas com os espaços vazios. Na base do esquema, ao centro, em preto, o letreiro em duas linhas: Em cima e em preto: No modelo relacional, TUDO é tabela: Embaixo e em azul: entra (input) tabela, sai (input) tabela.](https://static.plataforma.grupoa.education/pucrio/pucrio/604664/ff41610d-3bac-4ba8-839f-986883e602d8/content/img/artesdg/img10.png)

Além disso, é necessário também definir uma linguagem para lidar com a estrutura das relações em si, neste caso uma Linguagem de Definição de Dados (LDD, ou _Data Definition Language_ — DDL).

O modelo relacional originalmente se baseou em duas LMD ditas puramente relacionais: **cálculo relacional e álgebra relacional**. O cálculo, por sua vez, se apresentou em duas versões: cálculo relacional de tuplas (_tuple relational calculus_) e o cálculo relacional de domínio (_domain relational calculus_). A linguagem Álgebra Relacional contém cinco operadores básicos: União, Diferença e Produto Cartesiano, que são operadores de manuseio de relações oriundos da teoria de conjuntos; e operadores próprios de relação, chamados de Projeção (_Project_) e Seleção (_Select_). Em termos de poder de expressão computacional, ambas as linguagens são equivalentes.

Na prática dos sistemas de bancos de dados relacionais, outra linguagem se tornou padrão de fato ao longo dos anos, e assim é até hoje: **_Structured Query Language,_** **ou simplesmente SQL**. Trata-se de uma linguagem simples, mas bastante poderosa, baseada no formalismo do cálculo relacional e na lógica de primeira ordem (_first-order logic_, ou FO).

Embora a linguagem SQL faça referência apenas à fração de consultas (_query language_) num banco de dados relacional, ela se tornou padrão de linguagem em sistemas relacionais para todo tipo de manuseio, tanto LDD quanto LMD. Para não nos estendermos nas especificidades de cada linguagem, vamos aqui estudar apenas a linguagem SQL mesmo. As referências bibliográficas contêm os conteúdos necessários para aqueles que desejarem conhecer as demais linguagens, essencialmente teóricas, mas que não deixam de ser relevantes para a compreensão do modelo relacional.

O acesso e manipulação de dados através da linguagem SQL é realizado de forma **declarativa**. Ou seja, quando realizamos uma consulta com SQL, não precisamos **especificar como** o gerenciador irá obter os dados desejados. De fato, precisamos apenas **definir o que** desejamos que seja retornado a partir da consulta.

Na figura abaixo, ilustra-se de maneira simplificada o caminho percorrido por uma expressão de consulta na linguagem SQL internamente a um SGBD até retornar a resposta ao usuário. O motor de execução relacional executa a sequência de operações correspondente, seguindo um plano de execução de consulta (_Query Execution Plan_ — QEP) proposto pelo Otimizador do SGBD. Além da escolha dos operadores mais apropriados para realizar a consulta, o Otimizador gera um QEP utilizando estatísticas presentes nos metadados do banco.

![Infográfico com 3 elementos. O primeiro é um retângulo bordô com o título: Consulta SQL, localizado na parte de cima à esquerda.  O segundo, mais à direita e mais abaixo, com o mesmo título Consulta SQL, em uma figura cilíndrica azul. O terceiro, à direita, no canto direito, uma outra figura cilíndrica azul nomeada de Dados. Do primeiro e do segundo elemento saem, de cada um, uma flecha azul direcionadas para um retângulo com o texto: Processador de Consultas + Otimizador. Desse retângulo sai uma flecha azul apontada para a direita em direção a um outro retângulo com o texto: Motor relacional de execução. Desse retângulo há uma outra flecha azul apontada para o terceiro elemento: Dados.](https://static.plataforma.grupoa.education/pucrio/pucrio/604664/ff41610d-3bac-4ba8-839f-986883e602d8/content/img/artesdg/img11.png)

Na presença de múltiplas tabelas, com possivelmente múltiplas colunas cada, de fato seria muito difícil para um programador ou desenvolvedor propor ele mesmo “o caminho das pedras” para chegar aos dados desejados de maneira a cumprir os requisitos esperados de eficácia e eficiência. A facilidade de expressar consultas de maneira declarativa é compensada — de maneira interna ao SGBD e transparente aos usuários — com um Processador e Otimizador de Consultas que garante que a tarefa será executada como esperado e no menor tempo possível.

### SQL: a linguagem relacional-padrão
A linguagem SQL é uma linguagem de consultas simples, com sintaxe reduzida. Cabe lembrar que a SQL é limitada em seu poder de expressão, não sendo uma linguagem de programação completa (não pode simular uma máquina de Turing universal), e sim voltada somente para consultas no escopo do modelo de dados relacional.

Nestes exemplos, utilizaremos alternadamente o esquema relacional Carros e o banco de dados de Cervejas para ajudar a explicar a sintaxe e semântica da linguagem.

![[img12 1.png]]

Considerando então a linguagem SQL na sua fração voltada para consultas, é preciso citar logo de início a cláusula _SELECT_, que é obrigatória, devendo vir acompanhada de uma lista com uma ou mais colunas (separadas por vírgulas) da tabela cujos valores se deseja visualizar como resultado. Por ser a 1ª cláusula da SQL, muitos profissionais da área, quando querem que alguém defina e execute uma consulta, usam a expressão “faz um _select_”.

Após a lista de colunas, deve-se indicar a(s) tabela(s) que contêm os dados que buscamos. Para isso, inclui-se a cláusula _FROM_, também obrigatória, seguida do nome da(s) tabela(s). Nesta aula, com o intuito de manter um nível introdutório, vamos trabalhar com apenas uma tabela na cláusula _FROM_, o que já permite realizarmos consultas interessantes e relevantes.

O comando SQL apresentado na figura acima permite listar todos os nomes de bares que vendem alguma cerveja. Nesse comando, a coluna Bar aparece logo após a palavra _SELECT_, enquanto o nome da tabela é especificado (Vendem) após a palavra _FROM_. Expressões em SQL usam como separadores de cláusulas, nomes de tabelas e colunas apenas espaços em branco ou vírgulas. Assim, a cláusula _SELECT_ está em linha diferente da cláusula _FROM_ por questões didáticas apenas.

Considerando outro esquema relacional diferente (banco de dados Carros), temos na figura abaixo um exemplo de consulta simples usando um _SELECT_ e _FROM_, ainda sobre uma única tabela. Observe que selecionamos duas colunas da tabela Consumidores neste caso.

![[img13.png]]

Podemos identificar que o resultado de uma consulta possui somente as colunas especificadas no comando (nesse caso, Cidade e UF). Além disso, essas colunas aparecem na ordem em que foram especificadas na consulta.

Sabemos que por definição as relações persistidas no banco de dados não têm tuplas repetidas. Isto pode ser controlado por meio de regras explícitas de controle de integridade que o SGBD impõe. Entretanto, ao realizar uma consulta, mesmo sabendo que as tabelas utilizadas como entrada não têm duplicatas, o mesmo não se pode garantir quanto às tabelas obtidas na saída. Além disso, são relações temporárias e não persistidas, sem controle de integridade, em particular, de unicidade de tuplas.

Para isso, a sintaxe da linguagem SQL inclui uma cláusula adicional _DISTINCT_ que faz com que não tenhamos tuplas na tabela-resposta que sejam repetidas. Temos na figura abaixo um exemplo que ilustra esta situação e resolve a exibição de duplicatas.

![[img14.png]]

Se no esquema relacional do banco de dados tivermos uma tabela com muitas colunas, e se em alguma consulta quisermos ver todas estas colunas na saída, pode ser custoso, e sujeito a erros, precisar listá-las junto da cláusula _SELECT_. Assim, a sintaxe da linguagem SQL inclui uma maneira de simplificar esta expressão, usando o asterisco, como pode-se ver abaixo.

![[img15.png]]

#### Ordenação nos resultados de consultas

As linhas apresentadas na saída da consulta têm sido exibidas na mesma ordem em que foram listadas na representação da instância das tabelas persistidas no banco de dados. Se em alguma situação particular for necessário impor alguma ordem para visualização do resultado de uma consulta SQL, é preciso que se solicite explicitamente ao SGBD.

Para especificar a ordem em que as linhas de uma tabela devem ser apresentadas, utilizamos a cláusula adicional _ORDER BY_. Essa cláusula aparece normalmente ao final da expressão de consulta em SQL e deverá ser seguida do conjunto de colunas utilizadas para ordenação dos resultados, conforme representado na figura abaixo. Por padrão (_default_), é realizada a ordenação crescente. Esse tipo de ordenação pode ser explicitado com o uso da palavra ASC após o nome da(s) coluna(s). Caso se deseje realizar a ordenação decrescente, deve-se especificar DESC após o nome da coluna.

![Duas tabelas, de 2 colunas e 9 linhas. Tabela 1 com título: Tabela Vendem. Primeira linha: Pessoas; Cerveja. Segunda linha: Depósito; Leffe. Terceira linha:Pires; Jupiler. Quarta linha: Padoca; Ipa. Quinta linha: Pires; Gavea. Sexta linha: Padoca; Copa. Sétima linha: Depósito; Gavea. Oitava linha: Padoca; Patricia. Nona linha: Padoca; Gavea. Abaixo da Tabela 1, um retângulo com a pergunta: Quais pessoas gostam da cerveja Leffe ou Ipa? À direita em caixa alta, três palavras uma abaixo da outra, seguida de palavras correspondentes. SELECT seguida das palavras Cerveja, Bar.  FROM seguida da palavra Vendem. ORDER B seguida da palavra Cerveja. Tabela 2 com título: Resposta. Primeira linha: Cerveja; Bar. Segunda linha: Copa; Padoca.  Terceira linha: Gavea; Pires. Quarta linha: Gavea; Padoca. Quinta linha: Gavea; Depósito. Sexta linha: Ipa; Padoca. Sétima linha: Jupiler; Pires. Oitava linha: Leffe; Depósito. Nona linha: Patrícia; Padoca.](https://static.plataforma.grupoa.education/pucrio/pucrio/604664/ff41610d-3bac-4ba8-839f-986883e602d8/content/img/artesdg/img16.png)

#### Predicados para restrição e filtro nos dados

Até o momento, temos como selecionar colunas que desejamos visualizar (cláusula _SELECT_) e determinar quais tabelas estão envolvidas na consulta (cláusula _FROM_). Podemos também ordenar o resultado na saída através da cláusula _ORDER BY_. Entretanto, muitas vezes pode ser necessário filtrar dados e elementos que satisfaçam condições particulares. Para isso, basta considerar a cláusula _WHERE_, que utiliza predicados lógicos para restringir quais tuplas devem constar da resposta.

A figura abaixo traz uma situação destas: gostaríamos de expressar uma consulta em SQL que mostre pessoas na tabela Gostam, mas somente aquelas que gostam da cerveja Leffe. Percorrendo-se a tabela Gostam tupla por tupla, aparecerão na saída apenas aquelas tuplas cuja coluna Cerveja contenha o valor igual a Leffe. Neste exemplo particular, a cláusula _SELECT_ restringe também a resposta a apenas uma das colunas, o nome das pessoas que apreciam a Leffe.

![[img17 1.png]]

Estes predicados relacionais da cláusula _WHERE_ contêm expressões lógicas que serão validadas como verdadeiras ou falsas para cada instância particular do banco de dados. Naturalmente, pode ser útil utilizar conjunções (_AND_) ou disjunções (_OR_) em algumas expressões na cláusula _WHERE_.

Na figura abaixo, temos duas situações diferentes: no primeiro caso desejamos obter o nome das pessoas que gostam não somente de Leffe como também de Ipa. Podemos estender a expressão da figura com a disjunção OR e, assim, incluiríamos na resposta as pessoas que gostam tanto de Leffe quanto de Ipa. No segundo caso, com o uso da conjunção AND, temos como resposta uma tabela vazia pois nenhuma pessoa pode se chamar Ana e Carla ao mesmo tempo.

![[img18.png]]

Assim como nas linguagens de programação tradicionais, precisamos ter muito cuidado na hora de expressar consultas com operadores lógicos _AND_ ou _OR_, pois nem sempre a interpretação é clara aos usuários e desenvolvedores. Ainda na figura acima, temos um exemplo de expressão usando conjunção que retorna uma relação (ou tabela) vazia. De fato, não há valores para marcas de cerveja que tanto a Ana (cerveja Ipa) quanto a Carla (cervejas Copa e Jupiler) gostam.

As expressões da cláusula _WHERE_ envolvem de maneira geral comparações de atributos com valores, ou ainda atributos com atributos. Os símbolos de operadores de comparação como igual (=), maior (>) e menor (<), ou diferente (<> ou !=), podem ser usados nos predicados que restringem as tuplas que atendem a lógica da consulta.

Existe uma exceção do uso destes símbolos de comparação para quando se consideram os nulos. Se de alguma forma a consulta busca comparar colunas com valor _NULL_, deve-se utilizar _IS NULL_ ou _IS NOT NULL_. São fornecidos dois exemplos distintos para estas situações abaixo.

![[img19.png]]

Para concluir esta parte introdutória da linguagem SQL, precisamos explicar o importante conceito de **subconsultas aninhadas** **_(nested subqueries)_**. Como o próprio nome dá a entender, trata-se de definir consultas em SQL que contêm outras consultas SQL na mesma expressão. A figura abaixo traz um exemplo bem interessante para subconsultas: pede-se para utilizar a linguagem SQL com o objetivo de exibir na saída as cervejas que são vendidas em algum bar, mas que não as encontramos na tabela Gostam, isto é, que não são do gosto de nenhuma pessoa.

Essa operação nas linguagens relacionais é conhecida como DIFERENÇA relacional, também presente na teoria de conjuntos. Na prática, queremos saber quais cervejas estão presentes em certo conjunto (ou relação), mas não estão presentes em outro conjunto. No exemplo em particular, esta consulta permite identificar que a cerveja de marca Patrícia não é apreciada por ninguém nesta instância do banco de dados de Cervejas.

![[img20.png]]

Em termos sintáticos, usamos os termos _IN_ e _NOT IN_ para teste de pertinência de elementos aos conjuntos ou tabelas, isto é, se uma tupla pertence ou não a uma determinada relação. Assim, primeiramente identificamos quais cervejas estão presentes na tabela Gostam. Em seguida, comparamos quais cervejas na tabela Vendem não pertencem ao conjunto de cervejas presentes na tabela Gostam, para responder adequadamente à consulta.

A figura abaixo contém um exemplo de consulta SQL que utiliza o operador _IN_ para explicitar os valores de comparação utilizados em consultas com subconsultas aninhadas, em que se deseja verificar se elementos são membros ou pertencem a determinadas tabelas (ou conjuntos). Trata-se do mesmo exemplo da figura **[[img18.png]]**, mas com sintaxe simplificada, já que sabemos quais valores queremos comparar. Ou seja, nem sempre é necessário determinar os valores da tabela correspondente à subconsulta antes de executar a consulta completa. Às vezes, já conseguimos explicitar os valores de comparação desejados.

![[img21 1.png]]

Cabe observar que a linguagem SQL permite representar a diferença de conjuntos de outras maneiras, como, por exemplo, com o operador _EXCEPT_. Outros operadores de conjuntos, como _UNION_, também fazem parte da linguagem SQL.

#### Exemplo de tabela resposta servindo como entrada para outra consulta:
![[Pasted image 20240515205957.png]]

### Restrições de integridade em bancos de dados
Sabe-se que é possível determinar o modelo lógico de um banco de dados em função das duas partes do formalismo matemático escolhido: **a estrutura dos dados e a forma de manuseio deles**. No caso do modelo de dados relacional, temos como estrutura as relações, ou tabelas, e como manuseio temos as linguagens relacionais, em particular a linguagem SQL, padrão de mercado e bastante utilizada na prática. Já para determinar um esquema de um banco de dados relacional em particular, precisamos detalhar sua estrutura, a saber, as tabelas que pertencem ao banco de dados com as respectivas colunas.

Todavia, como não faz sentido termos dados incorretos ou inválidos, é importante definir algumas regras que determinem quais dados podem ser aceitos para popular as tabelas e quais não podemos aceitar, de forma que o banco de dados seja efetivamente útil para os sistemas que dele fazem uso.

Estas regras são conhecidas como **restrições de integridade** (_integrity constraints_) e, dada a importância que têm, na prática acabam fazendo parte da definição do esquema relacional de um banco de dados particular. Para qualquer modelo de dados, podemos especificar restrições chamadas estruturais — referentes ao modelo escolhido — e as restrições específicas da aplicação, também conhecidas como **regras de negócio** (_business rules_), que complementam a especificação da semântica que se espera dos dados armazenados no banco.

No caso do modelo relacional, temos restrições estruturais que dizem respeito ao fato de estarmos usando relações como estrutura de representação dos dados:

1 - restrição de chave;

2 - restrição de entidade;

3 - restrição de domínio;

4 - restrição de integridade referencial.

A ideia básica é definir conceitos e estipular condições que possam ser implementadas e controladas automaticamente pelo SGBD relacional escolhido. Desta maneira, teremos uma gestão eficaz dos dados no banco, garantindo que não serão obtidas informações inesperadas que comprometam os sistemas que se servem daqueles dados.

Nesta aula, veremos inicialmente as restrições **1 (chave)** e **4 (integridade referencial)**. Na próxima aula, as demais restrições, inclusive as regras de negócio, serão abordadas em mais detalhes.

#### Controlando tuplas repetidas com chaves primárias

Sabemos que relações não têm elementos repetidos, assim como os conjuntos. Caso contrário, não teríamos como distinguir uma linha da outra, pois os valores em todas as colunas de uma linha seriam exatamente iguais ao da outra linha.

A restrição de **integridade de chave** busca definir uma maneira de controlar esta condição de unicidade de tuplas em qualquer das tabelas de um esquema relacional. Na prática, temos a necessidade de diferenciar uma tupla da outra, pois estes representam os elementos de dados que serão utilizados no sistema computacional. Como não há identificador de linhas, cada uma das linhas de uma tabela deve conter pelo menos uma coluna, ou conjunto de colunas, que a identifica unicamente, contendo valores distintos. A isso chamamos de chave (_key_, em inglês) da tabela a coluna, ou conjunto de colunas, que permite esta identificação das tuplas em uma relação. Muitas vezes, temos colunas, ou conjunto de colunas, que naturalmente assumem valores diferentes para cada tupla e, assim, são consideradas **chaves candidatas**.

Suponhamos uma relação chamada Pessoa, contemplando atributos como nome, CPF, RG e UF (unidade federativa), data de nascimento, entre outros. Poderíamos ter uma chave candidata K1 = {CPF} e outra chave K2 = {RG, UF}. Observe que a chave K2 também é dita composta, pois contém mais de um atributo. Ademais, a lei brasileira permite números de RG iguais em estados diferentes, por isso K2 deve ser composta.

Um leitor mais atento poderia sugerir como identificador das linhas numa tabela a “chave” K3 = {CPF, Nome}. De fato, não há duas linhas na tabela com valores iguais para este par de colunas. Porém, sabemos que não há duas pessoas com o mesmo CPF, e temos em K3 um atributo adicional e desnecessário para identificação. Na teoria do relacional, K3 é dita uma super-chave (_super-key_, ou SK) da tabela. É um conceito que diz respeito a qualquer conjunto de colunas numa tabela que identifique unicamente suas linhas.


A diferença de uma chave para uma super-chave é que a primeira é dita _minimal_, no sentido de que a retirada de qualquer atributo do conjunto faz com que o mesmo deixe de ter a propriedade de identificar tuplas!


Com dois ou mais atributos, é preciso verificar se não há atributos adicionais sem necessidade. A super-chave K3 segue identificando linhas se retirarmos o atributo Nome do conjunto, explicitando o fato de que não se trata de um conjunto _minimal_; logo, não é chave candidata. Qualquer conjunto com apenas um atributo que identifique unicamente tuplas numa tabela pode ser chamado de chave (candidata) daquela tabela. O conjunto K2 é chave, pois, mesmo composta de dois atributos, tem a propriedade de ser _minimal_: somente com RG ou somente com UF não é possível identificar linhas na tabela.

Na teoria do modelo relacional, define-se que cada tabela pode ter apenas uma chave e esta pode ser definida arbitrariamente, sem prejuízo à definição de chave ou à propriedade de identificação das linhas. **Esta chave única de cada tabela é chamada de chave primária** **(** **_primary key,_** **ou PK** **)**, **e as demais chaves seguem como candidatas**. Se a chave K1 tiver sido escolhida como PK, a chave K2 segue como candidata, e vice-versa. Note que não existe a noção de chave secundária no modelo relacional: temos apenas chaves primárias ou chaves candidatas. Além disso, se a PK tem dois atributos, diz-se apenas que a PK é composta, mas não deixa de ser única — não são “duas PKs”, como muitos interpretam erroneamente.

Por definição, todos os atributos de uma relação (qualquer!) formam uma SK, já que não teremos tuplas com valores iguais ou repetidas. Quando não temos naturalmente subconjuntos do conjunto completo de atributos da tabela que permitam identificar as linhas de uma tabela, recorremos ao artifício de considerar uma **chave artificial** _(surrogate)_ para identificar as tuplas. É o caso dos identificadores como CPF, de pessoas ou contribuintes, ou mesmo o atributo Matrícula de alunos em universidades ou escolas. Como existem homônimos possíveis, busca-se simplificar a definição da PK com um único atributo que, por construção, não se repete para qualquer indivíduo. O mesmo vale para empresas (CNPJ) ou mesmo códigos de estados ou países para sistemas de telefonia (DDD ou DDI, respectivamente). Alguns desenvolvedores sugerem colunas adicionais na tabela com contadores (ou seriais) para servirem como PK. Entretanto, diferentemente dos demais exemplos que têm interpretação apropriada às aplicações particulares, atributos com números sequenciais são artifícios utilizados para, de alguma forma, referenciar tuplas como se fossem registros ordenados em arquivos, o que não é o caso.

Utilizar um conjunto muito grande de atributos como PK de uma tabela pode implicar em problemas de desempenho no sistema de banco de dados, pois o processamento que permite identificar tuplas será mais demorado. Entretanto, atributos artificiais não têm semântica própria: entendemos perfeitamente que Uruguai é um país da América do Sul, mas não é imediato associar que 598 é um código de telefonia daquele país.


Sabe-se que, na prática, em função das características particulares do sistema de banco de dados relacional que será desenvolvido, a escolha da chave primária pode não ser tão arbitrária assim. Neste caso particular de identificação de pessoas, a chave K1 poderia ser considerada primária para bancos de dados voltados mais às aplicações financeiras. Já no caso de problemas aplicados com identificação civil, a chave K2 seria mais adequada.


Por todos esses motivos relatados, o modelo relacional também é conhecido como orientado aos valores (_value-oriented_) e não orientado a linhas, tuplas ou mesmo registros, como analogia visual aos arquivos considerados pelas linguagens de programação, que são ditos orientados aos registros (_record-oriented_) ou mesmo aos objetos (_object-oriented_) com seus identificadores.

#### Integridade referencial e chaves estrangeiras

Existe uma situação particular de controle de integridade que procura estabelecer um relacionamento entre colunas de tabelas diferentes, utilizando como domínio de valores válidos para uma coluna C1 na tabela T1 os valores que estão presentes na coluna C2 da tabela T2. Como exemplo, podemos citar que os valores dos estados (coluna UF) na tabela de Pessoas deve ser igual aos valores de UF presentes numa tabela contendo apenas os estados brasileiros. Dessa maneira, garantiríamos que os códigos de UF utilizados seriam todos válidos. Analogamente, podemos citar também que os valores para marcas de cerveja presentes nas tabelas Gostam ou Vendem também seriam apenas os valores existentes numa tabela Origem, que lista marcas de cerveja e seus país de fabricação original. Ou ainda seria uma maneira de garantir que o valor Astrologia não seria aceito como o curso de um aluno da PUC-Rio, pois não existe este curso na tabela de cursos da instituição presentes no banco de dados.

Esta restrição é conhecida como **integridade referencial** exatamente por envolver valores em determinada tabela que fazem referência a valores em outra tabela. De maneira um pouco mais formal, e buscando evitar algumas possíveis inconsistências, a restrição de integridade referencial diz que os valores da coluna C1 da tabela T1 devem referenciar valores em uma coluna C2 que é necessariamente chave primária (PK) da tabela T2, ou então podem assumir valor _NULL_. A coluna C1 é definida como chave estrangeira (_foreign key_, ou FK) da tabela T1.

Cabe observar que esta definição de restrição de integridade com chaves estrangeiras referenciando chaves primárias não se aplica apenas a atributos isolados. Se a chave primária da tabela T2 for composta de um ou mais atributos, só poderemos ter chaves estrangeiras se pelo menos a quantidade de atributos for a mesma. Além disso, o domínio dos valores deve ser o mesmo para cada uma das colunas envolvidas na FK e na PK referenciada. Logo, se estamos falando da PK {RG, UF} em determinada tabela, é preciso existir um outro par de colunas {C3, C4} em alguma tabela tal que os domínios de valores em C3 e C4 sejam iguais aos domínios de RG e UF, respectivamente. A integridade referencial neste caso só seria satisfeita se valores do par {C3, C4} forem iguais a _NULL_ ou, caso contrário, iguais a valores do par {RG, UF}. Por último e não menos importante: é possível, mesmo sendo mais raro, que uma FK aponte para uma PK da mesma tabela! Ou seja, não necessariamente T1 e T2 serão tabelas diferentes.

Sabe-se que os sistemas de bancos de dados são criados e projetados para lidar com bancos de dados com grande volume (_Very Large Databases_ — VLDB) e aprende-se a lidar com estes sistemas usando linguagens como SQL declarativas, com as quais dizemos o que queremos sem entrar em detalhes de como isso será feito pelo computador. Neste momento, cabe perguntar: como saber se o resultado de uma consulta sintaticamente correta (e que, portanto, será executada!) está semanticamente correto? Se temos de fato um VLDB, é praticamente impossível validar o resultado mediante uma verificação visual ou manual.  

Outra dúvida muito comum se apresenta quando estudamos os sistemas de bancos de dados relacionais. Afirma-se que as tabelas ou relações, teoricamente, seguem a teoria dos conjuntos, e não podem conter elementos repetidos. Mas na prática as tabelas que são resultados de consultas quase sempre representam os chamados multiconjuntos (_multisets_), e tuplas repetidas podem ser exibidas como saída de uma execução de consulta SQL. **De que maneira lidamos na prática com esse problema?**

### Códigos & Links:
Aula 1 - https://colab.research.google.com/drive/19q6DKQU18crLIq5v8WnbmGokJdR1CYfL
**CODD, E.F., “A Relational Model of Data for Large Shared Data Banks”** - https://www.seas.upenn.edu/~zives/03f/cis550/codd.pdf
**CHEN, P.P.S., “The Entity-Relationship Model-Toward a Unified View of Data”.** - https://dl.acm.org/doi/epdf/10.1145/320434.320440

### Referências:

CODD, E. F. A relational model of data for large shared data banks. **Communications of the ACM**, v. 13, n. 6, p. 377-387, 1970.

COSTA, R. L. C. **SQL**: guia prático. Rio de Janeiro: Editora Brasport, 2006.

ELMASRI, R.; NAVATHE, S. B. **Sistemas de bancos de dados**: fundamentos e aplicações. 6 ed. Campinas: Pearson Universidades, 2010.

GARCIA-MOLINA, H.; ULLMAN, J. D.; WIDOM, J. **Database systems**: the complete book. Hoboken: Prentice Hall, 2008.

HEUSER, C. A. **Banco de dados relacional**. Joinville: Clube de Autores, 2019.

RAMAKRISHNAN, R.; GEHRKE, J. **Sistemas de gerenciamento de bancos de dados**. 3 ed. Porto Alegre: AMGH, 2008.

SILBERSCHATZ, A.; KORTH, H. F.; SUDARSHAN, S. **Sistema de bancos de dados**. Rio de Janeiro: Elsevier-Campus, 2012.

ULLMAN, J. D. **Principles of database and knowledgebase systems**. Ann Arbor: Computer Science Press, 1988. Vol. 1.

## Projeto Conceitual e Lógico, SQL DDL (Esquemas) e SQL LMD (Instâncias) (Aula 2)

Temos, a seguir, uma visão geral do processo envolvido no projeto de um banco de dados relacional.

![[Pasted image 20240516105009.png]]

![[Pasted image 20240516104947.png]]

![[Pasted image 20240516105048.png]]

![[Pasted image 20240516105101.png]]

![[Pasted image 20240516105111.png]]

![[Pasted image 20240516105120.png]]

### Processo de modelagem conceitual

Seguindo o processo ilustrado anteriormente, antes de projetarmos um banco de dados, para qualquer modelo lógico, não apenas relacional, sugere-se elaborar um modelo estritamente conceitual que contemple todos os dados do banco e a maneira como que esses dados se relacionam.

O modelo de entidades e relacionamentos (MER), proposto em 1976 por Peter Chen, é um dos mais utilizados pelos profissionais de mercado e, certamente, o processo de modelagem conceitual mais difundido. Na década de 1990, com a popularização do paradigma de orientação a objetos (OO) para linguagens de programação, houve um esforço para a consolidação de métodos e modelos existentes para projeto de sistemas que resultou na _Unified Modeling Language_ (UML). Especificamente, é o diagrama de classes da UML que poderia servir como arcabouço para definir adequadamente esquemas conceituais.

Tanto o MER como a UML têm recursos com muitas opções para caracterização dos conjuntos de dados e seus relacionamentos, algo necessário para a implementação de um banco de dados que dará suporte a um sistema de informações específico. De certa forma, a UML é uma linguagem bem mais complexa. Não somente é útil para modelagem de dados, mas também serve como base para desenvolvimento de programas completos. Como aqui estamos interessados apenas na modelagem conceitual com foco nos dados, **vamos considerar apenas o MER ao longo do texto.**

Vale lembrar que, como vimos na primeira aula, temos dois níveis de representação abstrata no processo de modelagem. Nesse caso, temos o **modelo** de entidades de relacionamentos, genérico e válido para projetos conceituais diversos, e podemos ter múltiplos **esquemas** de entidades e relacionamentos, que são particulares para cada problema ou aplicação em si.

#### Entidades e atributos

A modelagem por entidades e relacionamentos tem alto grau de abstração e foi proposta com o intuito de capturar a semântica de aplicações do mundo real. É um modelo simples, intuitivo, mas formal, que define como representar dados e relacionamentos entre estes, com regras e especificações que devem ser satisfeitas para que a modelagem possa ser considerada correta.

Basicamente, temos três tipos de objetos a modelar:
- as entidades;
- os relacionamentos; e
- seus atributos.

Como forma de linguagem, adota-se na prática uma representação visual conhecida como **diagrama de entidades e relacionamentos (DER)**, que facilita o uso da modelagem e as trocas entre usuários-desenvolvedores e usuários não técnicos.

Naturalmente, temos como o primeiro conceito a noção de **entidade**. Como qualquer outra abstração, definir entidade não é trivial. Podemos dizer que se trata de algo (ou uma “coisa”) que pode ser inequivocamente identificado por um conjunto de propriedades ou características em comum.

Em um DER, as entidades são representadas por meio de quadrados ou retângulos. Seja o DER da Figura [[stb02b.png]],que diz respeito a um esquema conceitual ER sobre cervejas, desenhado com o apoio da ferramenta [brModelo](https://www.brmodeloweb.com/lang/pt-br/index.html). Observe que se trata de uma versão ampliada e mais detalhada que o banco de dados das cervejas contemplado na primeira aula. Temos três entidades principais:

![[stb02a.png]]

Buscamos modelar uma aplicação em que registramos quais pessoas gostam de determinadas cervejas e quais bares vendem cervejas, de determinadas marcas (nacionais ou importadas), por preços específicos. Mais adiante comentaremos sobre as entidades Nacional e Importada, que estão diretamente associadas à entidade Cerveja.

![[stb02b.png]]

As propriedades relevantes de cada instância em uma entidade são representadas por meio de **atributos**. É fundamental entender que não existem entidades sem atributos, pois são estes que os definem, e não o nome da entidade, que serve apenas para facilitar a identificação em um diagrama. Por exemplo, como as pessoas que apreciam cervejas têm as mesmas características (atributos) que as pessoas que são proprietárias de bares, não faria sentido termos duas entidades diferentes.

Os atributos de uma entidade são representados no DER por seus nomes, dispostos na parte externa do retângulo que representa uma entidade, ao lado de pequenos círculos. Em algumas representações visuais, a lista de atributos é incluída dentro do retângulo da entidade, mas, aqui, vamos adotar a notação mais convencional, que também é utilizada pela ferramenta [brModelo](https://www.brmodeloweb.com/lang/pt-br/index.html).

Na Figura 2.02B, vemos que a **entidade Bar tem três atributos: Nome, Cidade e Estado**, que permitem especificar cada um dos bares desse banco de dados particular. Por simplificação, consideramos que não há dois bares com mesmo nome para esse sistema em construção. O atributo Nome aparece com o círculo preenchido de cor preta, significando que se trata de um **atributo identificador**, que permite identificar todas as instâncias, ou ocorrências, dessa entidade. Cada ocorrência representa um bar diferente.

Atributos identificadores têm interpretação similar à das super-chaves (SK) em tabelas do modelo relacional, ou seja, em um MER, não há exigência de minimalidade, como no caso de chaves primárias (PK), do modelo relacional.

Os demais atributos (Cidade e Estado) da entidade Bar complementam as informações sobre cada ocorrência na entidade Bar. Veja que os atributos são apresentados no DER acompanhados por dois valores entre parênteses: o primeiro informa se o atributo é opcional (valor 0) ou obrigatório (valor 1); o segundo diz respeito ao fato de ser mono (valor 1) ou multivalorado (valor N > 1). Os atributos identificadores são todos implicitamente definidos como obrigatórios e monovalorados. No caso, no exemplo da Figura 2.02B, temos que tanto Cidade como Estado, na entidade Bar, são opcionais, ou seja, podem assumir algum valor, mas também podem ser desconhecidos.

Neste DER em particular, todos os atributos, de todas as entidades, inclusive os identificadores, são monovalorados. Os atributos ditos multivalorados são aqueles que podem representar mais de um valor, de mesma natureza, em seu conteúdo. Poderia ser o caso de ocorrências na entidade Cerveja cujo atributo Tipo, por exemplo, tivesse mais de um valor.

Existe outra categoria de atributo, chamada de estruturada ou composta, que também contém mais de um valor, como a multivalorada, porém de natureza (semântica) distinta. Não temos também exemplos de atributos compostos na Figura 2.02B, mas, apenas como ilustração, é como se, no caso da entidade Pessoa, a data de nascimento não fosse representada por um único valor, e sim um atributo subdividido em três outros atributos separados: dia, mês e ano.

##### Relacionamentos e hierarquias entre entidades

Como o próprio nome diz, em um MER temos entidades e **relacionamentos**. Os losangos utilizados no DER representam os relacionamentos entre ocorrências de entidades ou, genericamente, relacionamentos entre entidades. Na Figura [[stb02b.png]], estão representados diversos relacionamentos, de tipos distintos, que serão detalhados a seguir.

Se observarmos o diagrama sobre cervejas, temos um relacionamento denominado “Dono de” entre as entidades Pessoa e Bar. Ele significa que determinada pessoa pode ser dona, ou proprietária, de algum bar. Relacionamentos são descritos adicionalmente por meio de **cardinalidades mínimas e máximas**. Nesse relacionamento “Dono de” entre Pessoas e Bares, temos a cardinalidade (0,1) próxima de Pessoa: o primeiro valor (cardinalidade mínima) é referente à obrigatoriedade (valor 1), ou não (valor 0), de se ter algum proprietário de determinado bar. Nesse caso, a modelagem explicita que bares podem não ter proprietários, ou não sabermos quem é o proprietário, por isso o valor zero. A cardinalidade máxima igual a 1 determina que, caso exista alguma pessoa proprietária daquele bar, só pode ser uma única ocorrência na entidade Pessoa. Já a cardinalidade (0,N), próxima da entidade Bar, deve ser entendida da seguinte forma: nem toda pessoa é proprietária de algum bar, mas, caso seja, ela pode ter mais de uma propriedade.

A prática de modelagem conceitual considerando o MER utiliza apenas as cardinalidades máximas para especificar os tipos básicos de relacionamentos entre entidades. Temos, de maneira geral, três situações distintas:

![[Pasted image 20240516114749.png]]
**Também chamado de “N para N” ou “muitos para muitos”**, serve para representar casos em que podemos ter mais de uma ocorrência de uma entidade se relacionando com mais de uma ocorrência da outra entidade. No caso das cervejas, temos, por exemplo, o relacionamento Gosta, que representa o fato de cada pessoa poder gostar de mais de uma cerveja e, também, que uma cerveja pode ser apreciada por mais de uma pessoa.

![[Pasted image 20240516114809.png]]
**Conhecido também como “1 para N” ou “1 para muitos”**, permite modelar casos em que apenas uma das entidades tem múltiplas ocorrências se relacionando com apenas uma ocorrência da outra entidade. Na Figura [[stb02b.png]], temos o relacionamento “Dono de” como representante dessa situação. A leitura que se faz é que uma pessoa pode ser proprietária de mais de um bar, porém cada bar pode ter apenas um proprietário.

![[Pasted image 20240516114833.png]]
Note que, assim como para as entidades, **a modelagem ER permite atributos também para relacionamentos**. No exemplo do esquema conceitual ER das cervejas, o atributo Valor do relacionamento Vende permite especificar o preço que cada bar vende suas cervejas. Esse atributo não é nem da entidade Bar, pois não faz parte dos conceitos que descrevem um bar, nem é atributo da entidade Cerveja, pois cada marca pode ter um valor de venda diferente em cada bar em que é vendida.


Há situações na modelagem conceitual em que é necessário representar um **relacionamento que ocorre entre ocorrências de uma mesma entidade**. Esse tipo de relacionamento é **chamado de “autorrelacionamento”** e é muito comum na prática. No caso do esquema ER das cervejas, vemos na Figura [[stb02b.png]] que estamos representando relacionamentos familiares na modelagem. Assim, há ocorrências de Pessoas que são filhas de outras ocorrências presentes nesse banco de dados. Analogamente, há mães e pais representados conceitualmente. Estamos supondo, por simplificação, que não temos pessoas nas diversas hierarquias familiares com mesmo nome; caso contrário, teríamos de adicionar algum atributo como CPF ou RG.

Um **conceito** complementar, presente em particular nos autorrelacionamentos, é a noção de **papel**, que ajuda na interpretação de relacionamentos. No caso do autorrelacionamento “Filho de” entre pessoas, temos os papéis de “pai-ou-mãe” e “filho” (ou filha) explicitados. Em termos de cardinalidades, a modelagem desse esquema ER em particular permite ocorrências da entidade Pessoa que não tenham vínculos familiares, isto é, não sejam pais ou filhos – cardinalidades mínimas iguais a zero. Já se alguém é mãe ou pai de alguém, pode ser de mais de uma ocorrência. Para simplificar a modelagem, estamos considerando que apenas uma mãe, ou um pai, são identificados no esquema para cada pessoa. Essa noção de papel pode ser explicitada em relacionamentos de qualquer tipo. É o caso, por exemplo, do papel de Proprietária junto da entidade Pessoa para o relacionamento “Dono de” referente a algum bar.

Para maior clareza conceitual das entidades e dos relacionamentos representados em um DER, é possível utilizar **um recurso** bem interessante **de modelagem, chamado de generalização ou especialização**. No DER, utilizamos um símbolo triangular para representar esse tipo especial de relacionamento, também conhecido por _IS-A_ (“é um”, em inglês). Na Figura [[stb02b.png]] temos um exemplo para a entidade Cerveja, especializada em duas outras entidades: Nacional e Importada.

Dizemos que Cerveja é uma generalização das entidades Nacional e Importada, ou, ainda, que uma ocorrência na entidade Nacional é uma Cerveja. O mesmo vale para a entidade Importada.

Na verdade, tudo depende de como foi o **processo de modelagem**: por um lado, se tínhamos apenas a entidade Cerveja e verificamos que, nesse exemplo, temos dados de fabricantes apenas de cervejas nacionais, para as demais que são importadas apenas os países de origem, decidimos criar as entidades especializadas. Por outro lado, podemos imaginar que o processo criou inicialmente duas entidades separadas, Cervejas Nacionais e Cervejas Importadas, com vários atributos em comum, apenas dois diferentes. Assim, generalizamos em uma entidade Cerveja tudo em comum, mantendo nas entidades especializadas o que é diferente. No final, independentemente do processo, o resultado é o mesmo.

Cabe observar que se trata de uma maneira de representar hierarquias de conceitos também. Os atributos da entidade Nacional são {Fabricante, Marca, Cor e Tipo}, e os atributos da entidade Importada são {País_de_Origem, Marca, Cor e Tipo}. O identificador (atributo Marca) é o mesmo para a entidade genérica Cerveja, assim como para as entidades especializadas. As entidades especializadas herdam os atributos da entidade genérica. Na Figura [[stb02b.png]] temos, junto ao triângulo do relacionamento _IS-A_, entre parênteses, duas letras que detalham o tipo de hierarquia representado. O primeiro valor pode usar a letra t ou p, informando que se trata de hierarquia total ou parcial. No caso, usamos a letra t, pois toda cerveja ou é nacional, ou é importada. O segundo valor pode ser igual às letras d ou c, significando disjunto ou compartilhado. Disjunto significa que uma ocorrência da entidade genérica pode assumir no máximo uma ocorrência na entidade especializada, e compartilhado indica que poderia estar em mais de uma. Neste exemplo, assumimos apenas um papel, isto é, as cervejas são ora nacionais, ora importadas.

A modelagem conceitual usando o MER prevê a possibilidade de representação de relacionamentos múltiplos envolvendo três ou mais entidades. Os relacionamentos binários – entre apenas duas entidades – são os mais comuns em um DER, mas também podem existir relacionamentos ternários, com três entidades, não representados nesse exemplo das cervejas.

Por fim, outro recurso menos comum, mas também interessante, é a possibilidade de representar “relacionamentos entre relacionamentos” por meio do conceito de entidade associativa (ou “superentidade”). É uma forma de contornar uma restrição sintática no DER, que não permite ligar diretamente um relacionamento a outro relacionamento. Suponhamos que quiséssemos representar no esquema conceitual das cervejas uma nova entidade chamada Fatura, que registraria os dados referentes às vendas de cervejas por determinado bar sempre que algum cliente do bar solicitasse. A entidade Fatura não se relacionaria com a entidade Bar apenas, pois depende da venda da cerveja. Analogamente, não é o caso de um relacionamento com a entidade Cerveja, pois a fatura depende da ocorrência na entidade Bar. Como não ocorre sempre, não seria um relacionamento ternário. Logo, teríamos que considerar o relacionamento Vende entre Bar e Cerveja como uma “superentidade” contemplando atributos em Bar, Cerveja e Vende, se relacionando com a entidade Fatura.

#### Mapeamento MER para modelo relacional

A modelagem conceitual é o primeiro passo apenas no sentido de obtermos um esquema de banco de dados relacional. Sabemos que modelos conceituais não são modelos de dados por completo pois só definem a parte estrutural de representação dos dados, mas não têm manuseio de dados, como ocorre nos modelos (lógicos) de dados.

O mapeamento de um esquema conceitual, definido pelo MER, em um esquema lógico do modelo relacional envolve transformar cada elemento de um esquema de entidades e relacionamentos (entidades, relacionamentos e atributos) em elementos equivalentes da modelagem relacional (tabelas, atributos e restrições estruturais).

Uma transformação mais detalhada e completa, envolvendo todos os componentes presentes em um MER, pode ser consultada nas referências bibliográficas. A tabela a seguir exibe uma síntese das principais transformações entre esquemas desses dois modelos.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb05.png]]

Ao aplicarmos as transformações da tabela apresentada ao esquema conceitual das cervejas na Figura [[stb02b.png]], vamos obter um esquema relacional como o ilustrado na figura abaixo. Como se trata do modelo relacional, temos agora apenas tabelas isoladas. Não há mais _links_, como temos com relacionamentos no DER.

Note que na Figura abaixo, cada tabela tem sua própria chave primária (PK), e algumas podem ter também chaves estrangeiras (FK). As PKs estão sublinhadas: no caso da tabela Cerveja, é a coluna Marca, e, para a tabela Gosta, é uma chave (composta!) das colunas Pessoa e Cerveja. Já as integridades referenciais das FKs são apontadas pelas linhas com setas indicando quais atributos referenciam ou são referenciados. Por exemplo, a coluna Cerveja é FK na tabela Vende referenciando a coluna Marca na tabela Cerveja, assim como o atributo Proprietário na tabela Bar referencia o atributo Nome na tabela Pessoa.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb06.png]]

Mas, finalmente, como chegamos ao esquema relacional a partir do esquema conceitual? Bom, inicialmente transformamos cada entidade em uma tabela com os respectivos atributos. Assim, foram criadas as tabelas Cerveja, Bar e Pessoa, inicialmente com os atributos das entidades apenas.

Ainda temos mais duas entidades, Nacional e Importada, presentes no esquema conceitual como parte do relacionamento _IS-A_ com a entidade Cerveja, e que também devem ser mapeadas para o esquema relacional. Como podemos ver na imagem anterior, optamos aqui por mapear toda a hierarquia para uma única tabela, e, assim, mais dois atributos passam a fazer parte da tabela Cerveja: País (nome simplificado para o atributo “País de Origem” no conceitual) e Fabricante.

Nesses casos, os atributos identificadores das entidades foram mapeados diretamente para as chaves primárias das respectivas tabelas no esquema relacional. Cabe observar que nem sempre esse mapeamento é direto, pois no MER os identificadores podem ser equivalentes a superchaves do modelo relacional, não sendo minimais como exigido para chaves candidatas. Se, nesse caso do esquema conceitual das Cervejas, tivéssemos como identificador da entidade Pessoa o par de atributos Nome e DataNasc, a PK da tabela não seria composta, pois, por suposição, o atributo Nome sozinho já é capaz de identificar tuplas.

Todas as entidades foram devidamente mapeadas. Vamos agora analisar os relacionamentos presentes na Figura [[stb02b.png]]. Como visto na tabela, há pelo menos duas formas de representar relacionamentos do MER no modelo relacional, dependendo de a cardinalidade ser NxN, 1xN ou 1x1.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb07.png]]

Os relacionamentos de cardinalidade 1x1 podem ser considerados casos particulares dos anteriores e são mais raros. A opção preferida, normalmente, é a fusão das entidades envolvidas no relacionamento em uma única tabela, incluindo todos os atributos, inclusive os do relacionamento. Porém, também há casos em que o procedimento para relacionamentos 1xN é mais adequado. Não temos relacionamentos 1x1 em nosso exemplo da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb06.png]]; logo, vamos nos concentrar nos outros dois casos que são mais comuns nas modelagens de aplicações reais.

Inicialmente, vamos analisar o relacionamento “Dono de” entre Pessoa e Bar. Nesse caso, por ser do tipo 1xN (cardinalidades máximas!), basta considerar a PK da tabela Pessoa como atributo adicional na tabela Bar, transformando um _link_ explícito no DER em um relacionamento orientado por valores. Optamos por chamar de Proprietário esse novo atributo, que naturalmente passa a ser FK em Bar, referenciando a PK Nome em Pessoa.

Em seguida, temos o relacionamento Vende, entre Bar e Cerveja. A cardinalidade, nesse caso, é NxN. Assim, passamos a ter a tabela Vende no esquema relacional, contendo os atributos PK oriundos das tabelas Bar e Cerveja. Como o relacionamento tem atributo, este também se transforma em coluna da tabela respectiva, mas não fará parte da PK. Para facilitar a interpretação, o atributo Nome da entidade Bar passa a se chamar Bar na tabela Vende, assim como o atributo Marca de Cerveja, que renomeamos para Cerveja. A PK da tabela Vende é o par (Bar, Cerveja), e ambos os atributos da PK são, separadamente, FKs para as tabelas Cerveja e Pessoa, respectivamente.

No caso do relacionamento Gosta, temos um procedimento similar ao relacionamento Vende, porém mais simples, pois não temos atributos presentes no relacionamento. Logo, são apenas duas colunas que, juntas, formam a PK da tabela Gosta e, separadamente, são FK para as tabelas Cerveja e Pessoa.

Por fim, temos o autorrelacionamento “Filho de” para a entidade Pessoa que precisa ser também ser mapeado para o esquema relacional. Como não deixa de ser um relacionamento 1xN, podemos seguir a mesma regra anterior de mapeamento, o que irá gerar uma situação interessante: a chave estrangeira apontará para uma chave primária na própria tabela, e não uma tabela diferente, como acontece normalmente. É necessário modificar o nome do atributo FK, senão ele teria o mesmo nome da PK. No esquema relacional Cervejas, da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb06.png]], temos a adição do atributo Genitor (nome alternativo para mãe ou pai) na tabela Pessoa, que será uma FK referenciando a PK Nome na mesma tabela.

### Criando tabelas com a linguagem SQ

Uma vez completo o mapeamento do esquema conceitual para o esquema lógico, é necessário implementar as tabelas em um SGBD utilizando a fração DDL da linguagem SQL, que permite criar os objetos do banco de dados relacional.

Um sistema de banco de dados relacional pode conter diversos objetos, como tabelas, visões e índices. Nesta aula, a ênfase é dada na construção das tabelas, que são a base de qualquer sistema relacional. Para isso, temos na imagem a seguir a sintaxe básica de criação de tabelas por meio do comando _CREATE TABLE_. Para cada tabela é preciso informar o seu nome, suas colunas com o domínio de valores válidos e, também, as restrições de integridade estruturais.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb08.png]]

Cabe, neste momento, relembrar a importância das regras ou restrições de integridade no modelo de dados relacional. Para bem definir um esquema relacional particular, e garantir que teremos no banco de dados apenas as informações úteis e desejadas, é necessário especificar restrições que controlam a integridade dos dados que se deseja representar.

Como vimos na aula anterior, existem, por um lado, os controles inerentes à estrutura do modelo de dados considerado. Por outro lado, há preocupação com regras que são mais genéricas e associadas à aplicação em si. Sendo modelo relacional o modelo lógico escolhido, as restrições são definidas em função de os dados serem representados na forma de relações ou tabelas. Já no segundo caso, contemplam-se as chamadas regras de negócio (_business rules_), que são independentes do modelo de dados lógico adotado. Podemos citar como exemplo a regra que diz que um aluno só pode fazer no máximo 30 créditos por semestre em um banco de dados acadêmico de uma universidade, ou, ainda, a restrição para um esquema relacional de uma empresa genérica que diz que nenhum empregado pode ganhar menos que o salário mínimo, nem ganhar mais do que seu chefe imediato.

#### Valores válidos nos atributos

Na aula anterior, estudamos a restrição de chave, que diz respeito ao controle de unicidade de tuplas, contemplando as noções fundamentais de chaves candidatas e primárias. Depois, foi mencionada a restrição de integridade referencial, que diz respeito às chaves estrangeiras. Entretanto, no caso do modelo relacional, temos outras restrições também consideradas estruturais: as restrições de entidade e de domínio.

A qualidade de um banco de dados relacional passa pelo controle de valores válidos em suas tuplas para cada atributo presente no esquema. Além de evitar elementos duplicados, também é possível especificar os valores esperados em função da semântica do atributo determinado pela aplicação em si.

As colunas em cada tabela estão normalmente associadas com domínios de valores válidos e esperados. Há casos relativamente simples, em que valores para o atributo Nome, em uma tabela Pessoa, não podem exceder certa quantidade de caracteres, limitando-se, em alguns casos, aos caracteres alfabéticos. Em outras situações, podemos ser bem mais específicos: a coluna Data de Nascimento deve ser necessariamente anterior à data corrente do sistema, ou, ainda, o valor atribuído às notas de uma prova deve ser numérico, porém restrito à escala de 0 a 10. Ao se definir cada tabela em um banco de dados relacional, e suas respectivas colunas, **a restrição de integridade de domínio** é aquela que busca definir as regras de valores válidos para cada atributo.

#### Regras de negócio

Também não se pode deixar de mencionar aquelas restrições que não fazem nenhuma referência à estrutura do modelo de dados em questão. No caso do modelo relacional, estamos nos referindo às regras que impõem qualidade aos dados do banco de dados, mas que não dependem do fato de termos tabelas para representá-los.

O infográfico a seguir mostra exemplos práticos de regras de negócio, que precisam ser consideradas em seus respectivos bancos de dados.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb09.png]]

Diferentemente das regras de integridade estruturais, não basta definir tabelas e atributos para impor as restrições desejadas no caso do controle semântico das aplicações particulares. Os SGBDs relacionais oferecem assertivas e outros objetos, como funções, procedimentos armazenados (_stored procedures_, ou SP) ou gatilhos (_triggers_) que permitem utilizar instruções SQL combinadas com comandos tipicamente presentes em linguagens de programação convencionais para especificar as regras de negócio. Esse assunto é considerado um tópico mais avançado no estudo de sistemas de bancos de dados e pode ser estudado consultando-se as referências bibliográficas aqui citadas.

#### Fração DDL da linguagem SQL

Voltando ao comando _CREATE TABLE_ da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb08.png]], temos que a linguagem oferece alguns tipos de dados que permitem controlar domínios de valores para cada coluna da tabela. Por exemplo, para atributos numéricos existem tipos como INTEGER e NUMERIC, que não somente garantem que apenas dígitos sejam utilizados, que expressões aritméticas possam ser usadas, mas que também podem controlar o total de algarismos, a parte inteira e decimal de um número.

Se precisamos armazenar uma cadeia de caracteres (_strings_) qualquer, envolvendo letras e números, podem-se utilizar os tipos CHAR e VARCHAR. Basicamente, a diferença diz respeito ao fato de que o tipo CHAR(10) reserva sempre 10 caracteres para representar a _string_, mesmo que tenhamos palavras com até 5 caracteres apenas, enquanto VARCHAR(10) apenas impõe um limite máximo e só ocupa, em _bytes_, o estritamente necessário. Apesar de vantajoso em termos de espaço, o manuseio de estruturas de tamanho fixo sempre é mais eficiente de maneira geral. Assim, há vantagens e desvantagens para esses dois tipos adaptados para _strings_.

Na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb08.png]] temos também exemplos das sintaxes básicas para definição de restrições estruturais, como as chaves primárias e as chaves estrangeiras. Para facilitar a compreensão, ilustramos, nas imagens a seguir, as expressões do comando _CREATE TABLE_ utilizadas para criar as tabelas do esquema relacional Cervejas, obtido a partir do processo de mapeamento do modelo conceitual para o modelo lógico.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb10.png]]

A Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb10.png]] traz os comandos de criação das tabelas Pessoa e Cerveja. Em termos sintáticos, assim como na fração DML de consultas da SQL, só é necessário ter espaços em branco entre comandos e objetos do banco de dados. Para fins didáticos, nesses exemplos temos, então, separadas as colunas de cada tabela e as demais restrições.


Para a tabela Pessoa, temos quatro colunas, e as duas colunas que fazem referência aos nomes de pessoas ocupam 50 caracteres – uma escolha arbitrária nesse caso; poderia ser mais ou menos –, mas ambas precisam ter a mesma quantidade de caracteres pela restrição de FK para PK. A coluna DataNasc (data de nascimento) é associada ao tipo DATE, que garante que valores nessa coluna serão datas válidas, além de permitir o uso de funções sobre datas que são úteis em aplicações reais. Por exemplo, é possível obter a idade de qualquer pessoa ao se comparar a data corrente do sistema com a data de nascimento. Poderemos também fazer consultas filtrando todas as pessoas que nasceram em determinado mês. Ou seja, atribuir o tipo de dado apropriado garante integridade e vantagens no manuseio daqueles valores.


A última coluna da tabela Pessoa é a Sexo, que, para esse exemplo em particular, escolhemos representar por apenas um caractere com o tipo Char(1). Entretanto, as restrições (_constraints_) definidas permitem ir além: nesse caso só seriam aceitos no banco de dados valores iguais a F, M ou X, respectivamente feminino, masculino e neutro, ou não declarado. Vale observar que, segundo a Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb10.png]], todos os atributos, exceto a PK, poderiam aceitar valores nulos, pois DataNasc e Sexo estão definidos como (0,1), logo, são opcionais. Entretanto, por motivo exclusivamente didático, optou-se na criação da tabela pela exigência de valores válidos para DataNasc, ilustrando o uso da sintaxe _NOT NULL_ no comando _CREATE TABLE_. Por _default_, o padrão é aceitar nulos, e, nesses casos, a linguagem SQL DDL não exige explicitar _NULL_ ao lado de cada atributo. De todo modo, na prática esta situação é muito comum: a modelagem lógica (relacional) acrescentar (ou relaxar) restrições presentes na modelagem conceitual (ER).

Por último, temos as definições das restrições estruturais do modelo relacional mais conhecidas: o atributo Nome é considerado a PK da tabela, e o atributo Genitor é FK referenciando a própria tabela Pessoa nesse caso, já que é oriundo de um autorrelacionamento. É recomendado, mas não obrigatório, nomear as restrições de integridade, como fazemos na Figura [[stb02b.png]]. Por exemplo, o nome da restrição _CK_pessoa_sexo_ será exibido na tela do computador sempre que algum usuário tentar colocar algum dado nessa coluna, para determinada tupla, que não satisfaça os valores F, M e X. Em um banco de dados com muitas restrições criadas, não há dúvida de que facilita termos mensagens de erros que identificam onde foi o problema.

Ainda na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb10.png]] temos o comando _CREATE TABLE_ da tabela Cerveja. Além de outras colunas e restrições particulares, com características similares às da tabela Pessoa, temos um exemplo de valor _default_ para a coluna País, associando o valor Brasil sempre que uma inclusão de tuplas na tabela não explicitar qual é o país de origem da cerveja.

Na figura a seguir, temos os comandos de criação das três tabelas restantes no esquema relacional da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb06.png]]. Cabe observar apenas o fato de que as tabelas Vende e Gosta têm, ambas, PK compostas por dois atributos. Além disso, cada atributo participante da PK também é FK para alguma PK em outras tabelas do esquema.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb11.png]]

Cabe observar que essa parte DDL (_data definition language_) da linguagem SQL é dedicada não às instâncias (os dados), e sim às estruturas que definem o esquema do banco de dados. Se estamos manuseando o esquema, vale comentar sobre dois outros comandos SQL muito usados em aplicações reais. Existe a expressão _ALTER TABLE_, que permite alterar nomes e tipos de colunas, adicionar ou retirar restrições de integridade e fazer outras modificações na estrutura das tabelas. Interessante observar que muitos comandos _ALTER TABLE_ podem ser feitos mesmo com dados já presentes nas tabelas. Podemos citar a situação particular da criação da FK Genitor, na tabela Pessoa, que referencia o atributo Nome na mesma tabela. Há SGBDs que não aceitam o comando _CREATE TABLE_ como consta na Figura [[stb10 3.png]]: é exigido primeiro criar a tabela sem chave estrangeira e, em um momento posterior, utilizar _ALTER TABLE_ para definir a integridade adequada.

Por fim, assim como criamos, podemos querer excluir tabelas do nosso esquema e, para isso, devemos utilizar o comando _DROP TABLE_. Sugerimos a leitura dos livros e manuais dos SGBDs _on-line_ para mais detalhes de cada um desses comandos.

#### Manuseio de dados nas tabelas

Com as tabelas criadas e implementadas, o próximo passo é incluir os dados propriamente ditos no banco. A imagem a seguir ilustra essa situação, com todas as tabelas do esquema relacional das cervejas contendo algumas tuplas que permitem compreender melhor o banco de dados que será disponibilizado para usuários e sistemas. Mas como foi que esses dados foram inseridos ou disponibilizados?

![[stb12a.png]]

Veremos, a seguir, os comandos SQL que viabilizam a carga dos dados em um banco relacional. Nesse ponto, voltamos a utilizar a linguagem em sua fração DML (_data manipulation language_), cujo foco são as instâncias, e não mais o esquema, como é o caso da fração DDL. Porém, diferentemente da primeira aula, não vamos praticar consultas, apenas **as instruções que nos permitem inserir, atualizar e excluir dados nos esquemas relacionais**.

O comando básico para inserir dados em um esquema relacional é o INSERT. Vamos adotar aqui a mesma metodologia de aprendizagem por exemplos, sem separar sintaxe da semântica da linguagem. A figura a seguir ilustra diversos comandos de inserção de dados com a linguagem SQL. Basicamente, é necessário escolher qual tabela deve receber dados e, pela cláusula VALUES, explicitar os valores.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb13.png]]

Um dos exemplos, com destaque em amarelo, chama a atenção para o fato de que, dependendo da implementação do SGBD em particular, valores de datas precisam respeitar o padrão da instalação feita com o SGBD. Não retorna erro, mas é importante saber disso para evitar interpretações erradas de dias e meses. No caso da imagem anterior, a intenção era inserir “24 de dezembro”. O SGBD utilizado nesses exemplos (PostgreSQL) considera datas na ordem mês, dia e ano, assim como vários outros SGBDs de mercado.

Os demais exemplos, com destaque em vermelho, têm explicitadas as situações de erro. O erro #1, por exemplo, exibe o controle de valores únicos por meio da PK, que não pode aceitar nulos (integridade de entidade). Já o erro #2 aconteceria pelo fato de a criação da tabela ter pré-definido os valores possíveis e _NULL_ não estar entre esses valores. O controle de integridade por meio de FK para cervejas inexistentes como PK em alguma tabela seria ativado no caso do erro #3. Por fim, exibimos um exemplo da vantagem de definirmos domínios apropriados aos atributos, por controlarem não só o tipo de caractere, mas também alguma semântica do dado em si. Nesse caso do erro#4, o fato de definir uma coluna como tipo DATE controla também quais datas são válidas, sem que o usuário precise desenvolver programas específicos para isso.

Usamos o comando INSERT para a carga inicial de dados e posterior manutenção do banco de dados com novas informações. Entretanto, como em qualquer sistema, pode ser necessário alterar algum dado ou mesmo excluí-lo, por conta de erros de manuseio ou adequação ao sistema em uso. Como em qualquer linguagem de programação que usa arquivos, podemos sempre proceder com alterações nos dados por meio de uma exclusão seguida de nova inserção. Entretanto, para grandes volumes em sistemas de bancos de dados, isso pode ser inviável. Assim, a linguagem SQL oferece, além do comando DELETE, que exclui tuplas, o comando UPDATE, que permite alterar dados persistidos, mantendo o controle de integridade em cada operação.

Para o esquema relacional das cervejas, temos, na imagem a seguir, alguns exemplos que ilustram a situação de atualizações de dados particulares. Mais adiante, quando colocar “a mão na massa”, o aluno poderá explorar outros casos distintos e conhecer em mais detalhes as opções sintáticas para os comandos UPDATE e DELETE e também o comando INSERT, discutido anteriormente.

![[stb14a.png]]

Nessa imagem, temos algumas expressões que seriam aplicadas ao banco de dados sem maiores problemas e outras que merecem atenção ou mesmo retornariam com erro pelo controle de integridade do SGBD. Por exemplo, ao tentarmos mudar o nome de uma cerveja em todas as tuplas da tabela Vende, teríamos uma mensagem de erro de integridade referencial caso o novo valor para cerveja (FK na tabela Vende) não conste nos valores da PK da tabela Cerveja.

Os demais casos não levantariam erro de controle do SGBD, mas, fica a dica: os comandos UPDATE e DELETE, sem cláusula WHERE, aplicam a atualização correspondente a todas as tuplas da tabela. Em particular, deve-se ter muito cuidado com o uso do comando DELETE, sobretudo em um sistema de produção. Mesmo quando a cláusula _WHERE_ está presente é preciso lembrar do _modus operandi_ dos sistemas relacionais, que são orientados aos conjuntos (_set-oriented_): mesmo que a intenção de determinado comando seja eliminar apenas uma tupla em particular, o SGBD vai aplicar o predicado lógico em todas as tuplas que validam a expressão correspondente ao _WHERE_. Na imagem anterior, esse seria o caso do DELETE para pessoas de nome “Mariana”.

Cabe comentar sobre uma situação prática que um SGBD relacional também monitora para fins de controle de integridade: se algum comando DELETE ou UPDATE excluir ou alterar o valor de alguma coluna PK de uma tabela que é referenciada por alguma FK da mesma ou de outra tabela, pode acontecer que o SGBD faça atualizações complementares automaticamente, em sequência ou “em cascata” (_delete cascade_ ou _update cascade_) após a exclusão ou alteração. Por exemplo, uma ou mais tuplas da tabela Gosta faz referência à cerveja da marca Leffe de cor Dourada na tabela Cerveja; a operação de DELETE correspondente na Figura acima implicaria o SGBD automaticamente alterar para _NULL_ todos os valores na FK da tabela Gosta, mantendo o banco de dados íntegro. O comportamento efetivo do comando SQL é definido por cada SGBD de maneira independente. Este é somente um exemplo.

### Teoria da normalização

Neste momento temos, então, um percurso de projeto de banco de dados relacional praticamente completo, saindo de um esquema puramente conceitual (MER) até um esquema relacional inteiramente definido por suas tabelas e restrições estruturais. Temos um caminho alternativo para chegar ao mesmo resultado por meio da **teoria da normalização**. Cabe observar que, historicamente, esta foi a primeira abordagem de modelagem lógica proposta e discutida pelos pesquisadores e desenvolvedores no início dos anos de 1970. A abordagem via modelagem conceitual, que acabamos de ilustrar, ganhou força apenas na segunda metade da década de 1970 após a ampla disseminação do modelo de entidades e relacionamentos.

De imediato, vamos explicar sucintamente os fundamentos e conceitos principais da teoria da normalização, a começar pela importante noção de **dependência funcional**.

Sejam:

- R (A1, A2, … An) uma relação (tabela) com N colunas;
- X e Y subconjuntos de {A1, A2, … An}, os atributos de R;
- t1,t2t1​,t2​ , ... tm as tuplas presentes em R.

Dizemos que X → Y é uma notação para representar que X determina Y

(ou, analogamente, Y depende funcionalmente de X)

Se, e somente se, t1[X] = t2[X] ⇒ t1[Y] = t2[Y], ∀ t1, t2​ em _r_ instância de R

Para o nosso esquema relacional das cervejas, temos que, por exemplo:

- (tabela Pessoas) Nome → DataNasc
- (tabela Cerveja) Marca → País, Tipo, Cor


Assim, as dependências funcionais são restrições sobre os atributos e tuplas em todas as tabelas de um banco de dados relacional que devem ser validadas para qualquer instância.

Para qualquer esquema relacional, como é o caso do esquema das cervejas, teremos um conjunto F de dependências funcionais (DF) contemplando os diversos atributos ou colunas das tabelas. Um DBA ou analista de sistemas, ou mesmo os programadores da aplicação, devem ser capazes de definir esse conjunto de DFs que vão permitir uma especificação mais precisa das regras de integridade, que devem ser verificadas permanentemente.

Vamos definir agora o conjunto F+ como o Fecho (_closure_) do Conjunto F das DFs válidas para uma ou mais tabelas de um esquema relacional. Na verdade, F+ corresponde ao conjunto de todas as DFs implicadas logicamente pelo conjunto F.

Por exemplo, se temos para uma tabela específica que:

- F: {A → B; B → C}

Podemos dizer que:

- F+: {A → B; B → C; A → C}


Por transitividade, se A determina B e B determina C, é possível inferir uma nova DF válida para a tabela contemplando os atributos A, B e C. Ou seja, não é necessário definir todas as DFs que possam ser válidas para um esquema relacional.


Para demonstrar uma utilidade da noção de DFs para o modelo relacional, estamos em condições de formalizar a noção de **chave**: sejam R (A1, A2, … An) uma tabela qualquer com N atributos; F um conjunto de DFs válidas para R; e X Í {A1, A2, …An}. Podemos dizer que X é chave de R se:

- X → {A1, A2, … An} ∈F+∈F+; e

- não existir Y Í X tal que Y → {A1, A2,… An } ∈F+∈F+.

Isto é, para ser chave, é preciso que exista uma DF em F+ com X determinando (funcionalmente) todos os demais atributos da tabela e não termos outro subconjunto Y de atributos de R, que seja, por sua vez, subconjunto de X, para o qual tenhamos também uma DF em F+ determinando todos as colunas de R. A primeira condição diz respeito à propriedade de uma ou mais colunas serem consideradas superchaves de R. Já a segunda condição é a de minimalidade, exigida para chaves candidatas e primárias.

Como vimos na primeira aula, sabemos que, se há mais de uma chave para R, elas são chamadas de “chaves candidatas”. Uma delas é escolhida arbitrariamente, ou seguindo conhecimentos da aplicação, como chave primária (PK) da tabela.

Essa formalização do conceito de chave permite definir também a noção de atributo primo (_prime_), que é qualquer atributo da tabela R que é parte de alguma chave candidata. Vimos, na primeira aula, um exemplo clássico de chaves candidatas com uma relação chamada Pessoa (que poderia ser uma extensão da relação Pessoa do esquema das cervejas), contemplando atributos como nome, CPF, RG (Registro Geral) e UF (unidade federativa, ou estado). Nesse caso, temos uma chave candidata K1 = {CPF} e outra chave K2 = {RG, UF}. Os atributos CPF, RG e UF são, então, chamados de “atributos primos”, pois são todos atributos de alguma das chaves candidatas.

Cabe observar que existem algoritmos que usam essa definição formal baseada em dependências funcionais para obter as PKs das tabelas em um esquema relacional, mas esses procedimentos estão fora do escopo desta aula.

Ao mesmo tempo, as DFs também podem ser usadas no processo de projeto de um esquema relacional, em que começamos com uma relação (universal) contendo todos os atributos envolvidos no banco de dados e vamos decompondo em tabelas menores até obter um conjunto de tabelas ditas normalizadas, que atendem especificações de qualidade conhecidas como “formas normais”.

Não é simples determinar qual é o conjunto “ótimo” de tabelas para um esquema relacional em particular. Existem muitas situações distintas do uso do sistema de banco de dados que nem sempre conseguimos contemplar integralmente. Assim, mesmo um esquema relacional normalizado, considerado de “boa qualidade”, pois atende determinado conjunto de formas normais, pode ser eficaz e correto, porém não eficiente, no sentido de desempenho. Quando discutirmos, na próxima aula, os aspectos relacionados com projeto físico, veremos que uma das técnicas mais conhecidas para obter esquemas relacionais com boa _performance_ envolve aplicar, para algumas tabelas, um processo chamado “desnormalização”.

#### Decomposição de esquemas

![[Pasted image 20240516224552.png]]

![[Pasted image 20240516224733.png]]

![[Pasted image 20240516224853.png]]

![[Pasted image 20240516224255.png]]

![[Pasted image 20240516224907.png]]

#### Formas Normais

![[Pasted image 20240516225435.png]]

![[Pasted image 20240516225449.png]]

![[Pasted image 20240516225523.png]]

### Transações em Bancos de Dados

Agora que já conhecemos a linguagem SQL tanto para consultas como para criação de tabelas e atualização de dados, podemos concluir esta aula comentando sobre o importante conceito de transações em bancos de dados relacionais.

Uma transação é considerada uma unidade básica de trabalho. Transações são tão importantes para os sistemas de bancos de dados como processos, ou tarefas, o são para os sistemas operacionais mais populares (p. ex., Linux, Windows).

Uma transação é, então, uma unidade de execução de um programa que acessa e atualiza vários itens em um banco de dados. Trata-se de um conjunto de instruções em SQL que é criado para atender determinada funcionalidade no sistema em operação. O exemplo canônico diz respeito a transações com operações bancárias: se queremos fazer uma transferência de valores entre uma conta poupança e uma conta-corrente, precisamos definir uma transação que, primeiro, retira valores da conta poupança para, em seguida, inserir valores na conta- corrente. São duas operações básicas (um DELETE, seguido de um INSERT) nas estruturas persistentes correspondentes às tabelas do banco de dados em questão.

Com o intuito de preservar a integridade, um sistema de banco de dados, com apoio de um SGBD, deve garantir as seguintes propriedades, conhecidas pelo acrônimo ACID (atomicidade, consistência, isolamento e durabilidade):

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb15.png]]

Se pudéssemos optar por oferecer um sistema de banco de dados em que cada transação (de um mesmo ou múltiplos usuários) é executada uma de cada vez, como se estivessem em uma fila de prioridade, não teríamos necessidade de gerenciar e controlar transações para manter a integridade do sistema. Entretanto, sistemas de bancos de dados foram pensados para uso de múltiplos usuários e transações simultâneas, visando ao uso efetivo dos recursos computacionais disponíveis.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb16.png]]

Na figura apresentada, ilustramos os eventos típicos que podem causar problemas em um sistema de banco de dados relacional. Os problemas de consistência e persistência têm a ver com as propriedades ACID, e, assim, os SGBDs relacionais contemplam algoritmos e técnicas para controle de concorrência e mecanismos de recuperação após falhas.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb17.png]]

Para concluir, ilustramos, na Figura acima, o “ciclo de vida” de uma transação em um banco de dados relacional. Todo bloco de operações básicas contido em uma transação é iniciado pelo comando _BEGIN_ e termina pelo comando _END_. De maneira geral, as informações importantes dizem respeito às operações que fazem acesso em leitura (_READ_) ou gravação de dados (_WRITE_) presentes em cada expressão contida na transação.

Toda transação sempre termina, com ou sem sucesso. Mesmo quando tudo dá certo e consideramos “OK”, a transação fica em um estado chamado de _COMMIT_ parcial. Em inglês, _COMMIT_ é sinônimo de compromisso, ou seja, estamos aguardando que outras transações concorrentes terminem para podermos concluir com um _COMMIT_ final com sucesso. Caso outra transação que tenha gravado valores lidos pela transação em _COMMIT_ parcial tenha terminado com falha, o estado da transação muda de _COMMIT_ parcial para FALHA. Nesses casos, a transação é abortada com operadores específicos de cancelamento ou _ROLLBACK_, uma operação da linguagem SQL que permite retornar ao estado consistente inicial do sistema de banco de dados.


A construção de um esquema relacional completo, com tabelas, atributos e restrições de integridade, é uma maneira de garantir um sistema de banco de dados de acordo com as especificações e objetivos iniciais. Entretanto, com o esquema criado, normalmente faz-se uma carga de dados massiva, para que o banco de dados tenha utilidade prática. Sabemos que com as PK definidas em cada tabela, as inserções de novos dados podem não ser rápidas, já que o SGBD precisa controlar a integridade implementada. Assim, muitos DBAs optam por “desligar” o controle de integridade no momento de popular o banco de dados. Entretanto, sem as PKs, podemos ter muitos elementos repetidos, o que contraria a teoria do modelo relacional. Pode ser até mesmo inviável reativar (“religar”) o controle de tuplas sem repetição. Se você tiver o poder de decisão na sua empresa ou projeto individual, qual seria sua estratégia? Quais são as vantagens e as desvantagens de cada alternativa?

Mais: considere uma situação em que temos que fazer 1 milhão de comandos INSERT e, para isso, iniciamos uma transação para carga no banco de dados. Suponha que, após 999 mil inserções, há um _INSERT_ que gera uma mensagem de erro, com o SGBD bloqueando a operação por conta de um valor duplicado na chave. No modelo transacional dos sistemas relacionais, temos que a propriedade de atomicidade exige “tudo ou nada”, e, nesse caso, teríamos perdido tempo e incomodado todos os demais usuários do sistema à toa, pois tudo teria de ser desfeito. Como você resolveria uma situação dessas?

### Códigos & Links:
Aula 2 - https://colab.research.google.com/drive/1xTsM4mFufQ1kh1ddmFFVrst6sbgooGqK#scrollTo=fvX2kDZYw1I8
Minha solução do exercício de Projeto Conceitual com Diagramas ER - https://app.brmodeloweb.com/#!/conceptual/66475a231775d8bd582f9dd2

### Referências:

BOOCH, G.; RUMBAUGH, J.; JACOBSON, I. **The unified modeling language for object-oriented development**: documentation set version 0.9. Santa Clara, CA: Rational Software Corporation, 1996.

CHEN, P. P-S. The entity-relationship model: toward a unified view of data. **ACM Transactions on Database Systems**, v. 1, n. 1, p. 9-36, 1976.

COSTA, R. L. de C. **SQL**: guia prático. Rio de Janeiro: Brasport, 2006.

ELMASRI, R.; NAVATHE, S. B. **Sistemas de bancos de dados**: fundamentos e aplicações. [_s.l._]: Pearson, 2010.

GARCIA-MOLINA, H. **Implementação de sistemas de bancos de dados**. Rio de Janeiro: Campus, 2001.

HEUSER, C. A. **Banco de dados relacional**: conceitos, SQL e administração. Porto Alegre: Clube de Autores, 2019.

HEUSER, C. A. **Projeto de banco de dados**. Porto Alegre: Bookman, 2008.
## Complemento SQL DML, Consultas e Visões Relacionais, Índices e Projeto Físico (Aula 3)

Até o momento, nós vimos como utilizar a linguagem SQL para consultas relativamente simples. É possível selecionar colunas que desejamos visualizar (cláusula SELECT) e determinar qual tabela será necessária (cláusula FROM). Podemos também ordenar o resultado na saída através da cláusula ORDER BY. Por fim, pode ser necessário filtrar dados e elementos que satisfaçam condições particulares. Para isso, temos a cláusula WHERE, que utiliza predicados lógicos (expressões cujo resultado é verdadeiro ou falso) para restringir quais tuplas devem constar na resposta.

Veremos, em seguida, outros exemplos de manuseios possíveis e interessantes com bancos de dados relacionais. Vamos considerar o mesmo esquema relacional das cervejas, projetado e construído na aula passada, ilustrado na seguinte figura:

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb01.png]]

Seja, também, uma instância particular da tabela Pessoa, na figura a seguir, que utilizaremos ao longo desta aula para conhecer novas sintaxes e operadores. Cabe observar que são 12 tuplas com valores fictícios, utilizados apenas para fins didáticos e de exemplo. Por exemplo, temos a informação do genitor (Diogo) da Mariana, mas não sabemos quem é o genitor do Diogo, por isso consta como NULL. Lembrar que Genitor é FK na tabela Pessoa, referenciando a coluna Nome, PK na mesma tabela. Para PKs não podemos ter nulos, mas, para FKs, isso é permitido.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb02.png]]

Se quisermos saber quais são os filhos de determinada pessoa, esta é uma consulta relativamente trivial em SQL, considerando a tabela Pessoa. No exemplo a seguir, estamos buscando os filhos da pessoa de nome Regina. Assim, segundo a instância da tabela Pessoa, mostrada na figura anterior, temos como resposta o Alexandre e a Simone.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb03.png]]

Em SQL, podemos expressar essa consulta usando todas as cláusulas consideradas até o momento, como mostrado na figura a seguir. Veja que não precisamos da ORDER BY, mas, para fins didáticos, utilizamos a ordenação nesse exemplo. Para conhecer outros filhos de outras pessoas, basta substituir o valor na cláusula WHERE por outros nomes presentes na tabela Pessoa.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb04.png]]

Por exemplo, na figura a seguir, temos uma consulta semelhante (“Quais os filhos da Carla”) e que respondemos como fizemos para a pessoa de nome Regina, simplificando apenas a expressão ao retirar a exigência de ordenação na tabela Resposta, desnecessária nesse caso. Em seguida, propomos uma consulta que pede para listarmos as soluções das duas últimas consultas simultaneamente, a saber, os filhos da Regina e os filhos da Carla, todos em uma mesma tabela.

![[stb05 1.png]]

Também não é uma consulta considerada difícil de expressar com o conhecimento básico da linguagem SQL: basta uma disjunção (OR) que resolvemos o que se pede! É exatamente o que mostramos na Figura abaixo, na solução SQL#1 proposta.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb06 1.png]]

Entretanto, aproveitamos esse exemplo simples para introduzir um novo operador na linguagem SQL oriundo da teoria de conjuntos. Como sabemos, relações e conjuntos têm muito em comum. Nesse caso, a solução SQL#2, que permite listar tanto os filhos da Carla como os filhos da Regina, utiliza a união de tabelas através do operador UNION, que tem a mesma interpretação do operador de união para conjuntos. De fato, na primeira parte da expressão SQL#2 da figura mostrada anteriormente, temos o “conjunto” dos filhos da Regina e, após a palavra UNION, temos o outro “conjunto” dos filhos da Carla.

Assim como para conjuntos, não podemos unir “laranjas com bananas”: é preciso que sejam duas tabelas com a mesma quantidade de colunas e, para cada coluna em sua posição relativa, que sejam domínios de valores compatíveis. Isso é o que se costuma chamar de “compatibilidade de tipo” (_type compatibility_).

No exemplo que estamos descrevendo, as expressões SQL geram duas tabelas com apenas uma coluna, ambas chamadas “Nome”, satisfazendo o mesmo domínio de atributos, que, na Figura acima, diz respeito a nomes de pessoas. Se fossem “nomes de bares” com “marcas de cerveja”, a união também funcionaria, pois não deixam de ser conjuntos de caracteres alfabéticos como domínios. Entretanto, semanticamente falando, poderia não fazer sentido. Cabe ao programador evitar situações que permitem a realização da operação, mas que não têm interpretação adequada.

Veremos, a seguir, outros operadores tradicionais de conjuntos que se aplicam muito bem às relações. Apenas para podermos variar os exemplos, consideraremos agora as instâncias das tabelas Gosta e Vende.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb07 1.png]]

Na prática, no entanto, nem sempre temos resultados que estão perfeitamente de acordo com a teoria. Algumas consultas podem retornar tabelas que representam multiconjuntos (_multisets_), que contêm elementos repetidos. Veja que, na figura a seguir, a consulta SQL que lista todas as cervejas na tabela Gosta poderia retornar alguns valores repetidos, como, por exemplo, Antarctica, Jupiler e Leffe. Isso só não vai ocorrer porque usamos um DISTINCT junto ao SELECT da expressão SQL. Algo similar ocorre se quisermos listar todas as cervejas vendidas em algum bar. Novamente, o uso do DISTINCT evita isso. Mas como fazer para responder em SQL uma consulta que pede as cervejas que alguém gosta ou que algum bar vende?

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb08 1.png]]

Poderíamos usar novamente o operador UNION, que, na solução SQL#1 a seguir, retornaria todas as cervejas da tabela Gosta junto com as cervejas da tabela Venda. A operação de união elimina os valores em duplicata da solução, mas aqui a eliminação de valores repetidos nem precisa ser feita, pois as duas tabelas geradas pelas expressões em SQL usam o DISTINCT. Entretanto, em SQL, existe um operador adicional chamado UNION ALL, que, explicitamente, permite duplicatas. O motivo é direto e justificado: retirar valores repetidos em tabelas com grandes volumes é uma operação custosa, que pode levar muito tempo. Como a tabela com duplicatas tem um conteúdo de semântica similar ao da tabela sem duplicatas, sendo diferente apenas na quantidade de tuplas, muitas vezes usar o UNION ALL é a alternativa preferida em termos de desempenho. Cabe observar que existe também um operador INTERSECT ALL, que, de forma análoga, retorna uma relação fruto de uma interseção com valores repetidos.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb09 1.png]]

### Junções Relacionais

Todas as consultas em SQL até as aulas anteriores contemplaram apenas uma tabela de cada vez. Sabe-se que os bancos de dados relacionais na prática contêm duas ou mais tabelas que representam o mundo real. Assim, para podermos realizar consultas nesses bancos de dados naturalmente precisamos envolver duas ou mais tabelas do esquema relacional em questão na cláusula FROM. Quando isso ocorre, o SGBD relacional considera que todas as tuplas das tabelas presentes no FROM devem ser combinadas e comparadas antes de aplicarmos os predicados de restrição.

Se não há cláusula WHERE e, consequentemente, predicados que realizam o filtro das combinações de tuplas válidas, temos como resultado um produto cartesiano das relações constantes na cláusula FROM. Sabe-se que não há semântica limitada para produtos cartesianos em si, e, assim, estes devem ser evitados. Logo, temos no modelo relacional um operador chamado de “junção” (_Join_, em inglês), que, na prática, realiza um filtro sobre a combinação de tuplas nas tabelas do FROM atendendo às condições de comparação lógica dos predicados na cláusula WHERE. Nesses casos, necessariamente teremos pelo menos uma condição de comparação entre atributos para cada par de tabelas listadas na cláusula FROM.

Na figura abaixo, temos um exemplo típico de uso do operador de junção para o esquema relacional das cervejas. Gostaríamos de expressar em SQL a consulta que retorna a lista de bares que vendem as cervejas de que determinada pessoa gosta.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb10 1.png]]

Para essa consulta, precisamos utilizar duas tabelas do esquema do banco de cervejas. Assim, na cláusula FROM, temos tanto a tabela Gosta como a tabela Vende, e, na cláusula WHERE, uma comparação de igualdade entre os valores do atributo cerveja nas duas tabelas e uma restrição adicional no nome da pessoa (Carla) usando conjunção (AND). Observe que, como os atributos têm o mesmo nome em ambas as tabelas, é preciso referenciá-los com o nome da tabela antes, caso contrário o SGBD daria mensagem de erro por conta da ambiguidade.

A junção pode ser interpretada da seguinte maneira: após combinar todas as tuplas de uma tabela com as tuplas da outra, a saída do operador corresponde apenas às tuplas que retornam como verdadeira a comparação de igualdade entre atributos que é explicitada. Ou seja, nesse caso, primeiro combinamos as tuplas de Gosta e Vende e filtramos para retornar apenas aquelas em que as cervejas têm o mesmo valor. Nesse caso, restringimos também em seguida para as tuplas com valor do atributo Pessoa igual a Carla. Finalmente, para as tuplas que atenderam essas restrições, exibimos apenas os valores da coluna Bar na saída.

Essa junção é também conhecida como equijunção (_equijoin_, em inglês), pois a comparação de atributos nas tabelas da cláusula FROM utiliza o operador de igualdade. É o caso mais comum de junção, que permite juntar dados em tabelas distintas, mas que, juntas, compõem a informação completa que o banco de dados traz. Há outras comparações usando outros operadores, mas não são muito comuns na prática.

A linguagem SQL inclui um termo para explicitar o uso de junções, e isso é ilustrado na figura a seguir. Trata-se do INNER JOIN (junção interna), que ainda exige que fiquem explicitadas na consulta as colunas que serão comparadas para realizar a junção.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb11 1.png]]

Na Figura abaixo, temos mais uma versão dessa mesma consulta utilizando o operador de NATURAL INNER JOIN (junção natural). É uma equijunção em que a comparação de igualdade é feita sobre atributos de mesmo nome nas tabelas envolvidas. Isso acontece com tanta frequência que a simplificação sintática é bastante útil. Na figura, vemos que a expressão fica bem mais simples do que as anteriores.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb12.png]]

É importante, neste momento, alertar para o fato de que em muitos esquemas relacionais temos atributos de mesmo nome que não têm a mesma semântica ou interpretação na aplicação em questão. Por exemplo, no esquema relacional das cervejas da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb01.png]], temos o atributo Nome para a tabela Pessoas e também para a tabela Bar. Normalmente não faria sentido essa comparação no caso da junção natural. É verdade que esses atributos podem até ter o mesmo domínio de valores. Nomes de bares e nomes de pessoas são, ambos, compostos de caracteres alfabéticos e podem, computacionalmente falando, ser comparados usando operadores da linguagem SQL. Seria o caso, por exemplo, de um manuseio pouco comum em uma consulta que queira saber se existe alguma pessoa nesse banco de dados que tenha o nome de algum bar.

A operação de junção interna também é normalmente chamada apenas de “junção”. Entretanto, existe outro tipo de junção, chamado de junção externa, e, por isso, a junção “normal” também é conhecida como interna. Essa junção externa (_OUTER JOIN_, do inglês) é similar à junção interna, mas considera, para fins de resultado na saída, as tuplas que se combinam na junção com outras que não se combinam.

No exemplo a seguir, temos uma consulta que pretende exibir uma lista de cervejas vendidas em algum bar e as pessoas que as apreciam. Como pode acontecer, em alguma instância, de termos cervejas para as quais não tenhamos pessoas que gostam, estas não apareceriam na junção interna. Entretanto, na junção externa são exibidas tanto as tuplas que satisfazem a condição da junção interna como as tuplas que não satisfazem. Nesse caso, complementamos o resultado com o valor NULO. Para o exemplo da base de dados de cervejas e a instância particular ilustrada, temos que não há pessoas associadas à cerveja Patricia. Logo, como não há como deixar a coluna Pessoa sem valor, é atribuído o valor NULO.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb13 1.png]]

Existem algumas variações de junções externas. Nesse caso, como visto na figura acima, utilizamos a junção externa à direita (_RIGHT OUTER JOIN_). O fato de ser à direita diz respeito apenas à posição relativa das tabelas na expressão da junção e para qual coluna é colocado o valor NULO na resposta. Por exemplo, se optássemos por começar pela tabela Vende, a resposta em SQL ficaria com a junção externa à esquerda (LEFT JOIN). Quando a junção externa permitir NULOS nas duas tabelas, ela é chamada de “junção externa completa”, ou FULL OUTER JOIN. Nesse exemplo particular, isso faria sentido se tivéssemos, além de cervejas para as quais não temos pessoas que as apreciam, cervejas de que algumas pessoas gostam, mas que não são vendidas em nenhum bar.

### Aliases ou Apelidos para Tabelas e Atributos

As expressões de consultas em SQL envolvem, de maneira geral, muitas tabelas e diversos atributos. Não somente alguns atributos têm o mesmo nome, como já vimos, mas também podemos querer visualizar na resposta de consulta as colunas de uma tabela com nomes mais apropriados para a compreensão.

Assim, a linguagem SQL permite o uso de _aliases_ (ou apelidos) tanto para desambiguar atributos como para simplificar a maneira de expressá-los nas consultas. A figura a seguir traz um exemplo duplo de utilidade dos _aliases_. Na cláusula SELECT, a coluna na tabela de resposta terá um nome bem mais claro e apropriado (Bar_da_Carla). Além disso, as tabelas Gosta e Vende são renomeadas para G e V, respectivamente. Assim, a expressão de comparação na cláusula WHERE também é facilitada.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb14.png]]

Vamos explorar um pouco mais o uso de _aliases_ nas expressões SQL. Um pouco antes, nesta aula, resolvemos a consulta de obter os filhos de alguma pessoa, por exemplo, os filhos da Regina. Como faríamos agora para obter os netos da Regina?

A tabela Pessoa (Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb02.png]]) só fala de genitores (mães ou pais) e filhos diretamente, e, por isso, a solução na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb04.png]] era imediata e simples. Agora teremos de manusear com linguagens relacionais para obter o resultado desejado com a devida interpretação sobre hierarquias familiares, como Avós, Pais, Filhos, Netos, Bisnetos, etc.

![[stb15 1.png]]

Aqui temos uma parte da instância da tabela Pessoa, com uma representação gráfica auxiliar da hierarquia familiar ali representada, envolvendo a pessoa de nome Regina. Olhando diretamente para os dados, temos como resposta que os netos da Regina são o Igor e o Leon. Mas como expressar uma consulta em SQL que permita retornar tais valores?

Uma alternativa seria “navegar” pelos dados de acordo com a semântica de uma hierarquia familiar. Para essa consulta, são apenas (e exatamente!) dois níveis na árvore, como demostrado na figura anterior: Regina é mãe do Alexandre e da Simone; Alexandre não tem filhos, mas Simone sim: ela é mãe do Leon e do Igor. Consequentemente, Regina é avó do Leon e do Igor.

Na Figura acima, temos a ilustração para essa estratégia de solução, com SQL convencional e básico, usando uma subconsulta para auxiliar na expressão. Na expressão SQL#1, temos que resolver, primeiro, a consulta SQL que retorna os filhos da Regina. De posse dessa tabela auxiliar representada pela subconsulta, a consulta mais externa pode comparar genitores com os valores na tabela dos filhos da Regina (Alexandre e Simone). Os eventuais filhos destes estarão na resposta da expressão SQL, e, como a Simone tem dois filhos, estes vão compor a tabela resposta.

![[stb16 1.png]]

Entretanto, temos outra estratégia usando junções para essa mesma consulta. Na realidade, é uma (auto)junção, pois se trata de uma junção de uma tabela (Pessoa) com ela mesma. Seria como se tivéssemos duas “cópias” da tabela Pessoa, mas, em cada “cópia”, os atributos passam a ter “papéis” diferentes. Na cópia P1, temos a pessoa Regina como avó e a pessoa Simone como filha; já na cópia P2 a Simone aparece como genitora (mãe) do Igor e do Leon, que, naturalmente, serão netos da Regina. Na figura mostrada anteriormente, ilustramos graficamente a situação, que permite compreender os efeitos da expressão SQL #2.

Algumas observações relevantes: em primeiro lugar, para (auto)junções, os _aliases_ são obrigatórios. Sem usar _aliases_ não teríamos como diferenciar as “cópias” da tabela Pessoa. Em segundo lugar, veja que podemos, para alguns SGBDs, não usar “AS” para os _aliases_, bastando um espaço em branco como separador. No exemplo, temos “Pessoa P1” em vez de “Pessoa AS P1”, o que também segue válido na linguagem SQL, claro. A maioria dos SGBDs permite isso; caso contrário, o “AS” deve ser mantido. Por fim, a estratégia que usa (auto)junção pode ser considerada mais declarativa, pois, diferentemente da primeira solução, não há necessariamente uma ordem de execução, em que a subconsulta é executada primeiro. Logo, o otimizador tem mais possibilidades de execução da consulta e gera um _Query Execution Plan_ (QEP) mais adequado e, provavelmente, mais eficiente.

Poderíamos seguir explorando a hierarquia familiar e utilizar SQL para retornar qualquer grau familiar conhecido. Se quisermos, além dos netos, os bisnetos, basta realizar mais uma operação de autojunção na tabela Pessoa, pois são três níveis hierárquicos. Na figura, teríamos na resposta da consulta a pessoa de nome Rodrigo como bisneto da Regina, pois é filho do Leon, que é seu neto já que é filho da Simone, por sua vez, filha da Regina.

![[stb17 1.png]]

E se quisermos todos os descendentes da Regina? Na figura acima, ilustramos essa situação com a árvore da hierarquia familiar, mas, se não sabemos quantos níveis temos na hierarquia, como especificar a junção? A mesma dúvida também pode ser colocada para a solução SQL#1 que utiliza subconsultas: se não sabemos quantos níveis hierárquicos existem envolvendo descendentes da Regina, em que momento paramos de criar subconsultas que permitem buscar por netos ou tataranetos?

Este é um dos limites teóricos da linguagem SQL, pois trata-se de uma linguagem baseada na lógica da 1ª ordem, o que significa que não temos nem controles de repetição, como expressões WHILE ou FOR das linguagens de programação mais conhecidas, nem sintaxe para expressar recursão.

Para resolver consultas desse tipo, sem saber quantos níveis hierárquicos precisamos percorrer, em princípio é necessário combinar SQL com linguagens de programação, como **C** ou **Python**. Existem iniciativas para incluir expressões recursivas em SQL, que poderiam resolver o problema, como é o caso da cláusula WITH com tabelas temporárias recursivas, porém é mais um artifício sintático do que aumento do poder de expressão da linguagem.

### Uso de Funções em Tabelas

Quando aprendemos a trabalhar com o modelo de dados relacional, em que temos todos os dados representados em tabelas, muitos se lembram das planilhas eletrônicas de programas como o Excel (da Microsoft) ou Sheets (do Google). No caso de SQL, também temos funções que permitem estatísticas simples sobre conjuntos de valores nas colunas de cada tabela. Podemos citar os operadores MAX (maior valor), MIN (menor valor), AVG (valor médio) e SUM (soma de valores), que atuam sobre os multiconjuntos de valores nos atributos de uma relação e retornam sempre um único valor.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb18.png]]

Nessa figura, temos um exemplo do uso do MIN para saber qual o valor da cerveja mais barata à venda em algum bar. Estamos considerando aqui as instâncias da tabela Vende da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb01.png]], cujo menor valor de cerveja à venda é de R$ 7,00. Já para a instância da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb02.png]], temos que o ano mais recente é 2002. Tendo como referência o ano de 2023, a pessoa mais nova tem, ou completa, 21 anos de idade. Usamos, nesse caso, funções particulares aplicáveis ao tipo de dados DATE, como ocorre para o atributo DataNasc. É possível extrair o ano de uma data de nascimento, permitindo fazer contas com anos.

De maneira geral, temos funções que se aplicam a dados numéricos. Na figura que segue, exemplificamos algumas utilizações do operador COUNT, que literalmente conta quantas tuplas existem na tabela referenciada, de acordo com as restrições impostas na cláusula WHERE. Cabe observar que NULOS são ora ignorados, ora considerados como zero nas contas realizadas. Mais: se não queremos contar valores repetidos, basta usar o DISTINCT junto com o COUNT, como ocorre na última consulta exemplificada na figura.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb19.png]]

As consultas da figura anterior são válidas e podem ser executadas em qualquer SGBD relacional. No entanto, sabemos que a metabase ou catálogo do banco de dados muitas vezes já mantém os valores atualizados disponíveis para consulta, como é o caso do total de pessoas na tabela Pessoa ou mesmo o total de pessoas de sexo masculino e feminino. Como normalmente temos bancos de dados volumosos, contar quantidades de tuplas de tabelas persistidas pode ser ineficiente.

Mesmo com uso das funções, sabe-se que a estratégia de manuseio de relações, ou tabelas, visando a resolver consultas aparentemente simples, nem sempre é trivial ou imediata de se expressar na linguagem SQL.

Na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb18.png]], foi apresentada a expressão para o valor da cerveja mais barata, mas como saber qual cerveja é vendida por esse valor? Na figura a seguir, por exemplo, estamos buscando obter a marca e demais informações da cerveja mais barata à venda.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb20.png]]

Mostramos, nessa figura, que uma estratégia é realizar uma subconsulta que obtém o menor valor de venda de uma cerveja, e esse valor é usado em uma expressão com comparador IN. Para isso, fazemos uma equijunção entre a tabela Cerveja (necessária para obter dados de cervejas além da marca) e a tabela Vende, comparando o valor da coluna Marca com a coluna Cerveja. Nesse exemplo, estamos aproveitando para ilustrar um aspecto sintático utilizado na cláusula SELECT. De fato, em vez de listar todas as colunas da tabela Cerveja, usamos “cerveja.*”, que facilita a expressão (para todas as colunas de uma das tabelas no FROM) para visualização da resposta da consulta. Esse artifício de uso do asterisco para representar todas as colunas de apenas uma das tabelas na cláusula SELECT pode ser usado em qualquer consulta SQL.

#### Funções e Agregados: Cláusula _Group By_

Se continuarmos buscando utilizar funções em consultas SQL, podemos ter dificuldades quando misturamos, na cláusula SELECT, funções com atributos simples.

Por exemplo, para obter uma lista de cervejas, mostrando para cada uma em quantos bares ela é vendida, e por qual valor médio de venda, não basta simplesmente “fazer um SELECT” em que associamos as cervejas aos seus valores médios de venda, e à quantidade de bares em que são vendidas, de acordo com a relação Vende. Se estamos calculando o valor médio de venda de todas as cervejas na tabela Vende, qual das cervejas mostraríamos ao lado desse valor por conta da cláusula SELECT?

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb21.png]]

Para isso, a linguagem SQL sugere utilizar uma nova cláusula, **chamada GROUP BY**. Como ilustrado na figura anterior, será possível agrupar tuplas com valores iguais em alguns atributos e considerar estatísticas para cada grupo de tuplas em separado. Nesse caso, todas as tuplas com valor igual para nomes de cerveja vão compor um grupo. Apenas a cerveja de marca Brahma é vendida em mais de um bar nessa instância. Assim, para as demais cervejas, o valor na tabela Vende é igual ao valor médio, sempre de acordo com a instância da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb01.png]].

Temos ainda a possibilidade de restringir ainda mais as tuplas que serão exibidas por atenderem à definição de uma consulta SQL envolvendo agrupamentos. Basta usar **uma nova cláusula (HAVING)** que permite expressar consultas que restringem valores sobre os grupos formados no Group By. A cláusula HAVING é um filtro nos grupos, assim como a cláusula WHERE é um filtro nas tuplas das tabelas.

A figura a seguir ilustra essa situação, em que estendemos a consulta discutida anteriormente para mostrar apenas cervejas consideradas baratas, com valor médio de venda de até 15 reais. A consulta em SQL é a mesma da Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb21.png]], com uma cláusula HAVING adicional para não considerar grupos com valor médio de venda nos bares do banco de dados maior que 15 reais. Algumas tuplas exibidas na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb21.png]] não mais aparecem na resposta por conta desse filtro HAVING. É importante observar que só podemos ter cláusula HAVING na presença de cláusula GROUP BY.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb22.png]]

Neste momento, podemos dizer que já teremos visto todas as cláusulas importantes da linguagem SQL (SELECT / FROM / WHERE / GROUP BY / HAVING / ORDER BY), com algumas variações que permitem explorar todo o poder de expressão de linguagens relacionais, e conhecer seus limites. Vamos agora explorar outros objetos que podem ser criados, e práticas aplicadas ao modelo de dados relacional, para facilitar o manuseio de esquemas relacionais de maneira geral e buscar bons desempenhos na execução de consultas.

### Visões Relacionais

Na Figura [[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb21.png]], explicamos como resolver em SQL uma consulta que exibe, para cada cerveja, em quantos bares ela é vendida e por qual valor médio. Se essa consulta é executada diversas vezes ao dia, por mais de um usuário, poderíamos de alguma maneira “salvar” essa consulta para poder reaproveitá-la outras vezes.

Existe um **objeto conhecido como visão** (ou _view_, em inglês), que permite guardar no catálogo do banco as definições de consultas para uso posterior. Na figura a seguir, ilustramos a criação de uma visão chamada Bares_e_Medias (com comando CREATE VIEW), que armazena a expressão da consulta que havíamos discutido anteriormente. Se executássemos a consulta que define a visão, obteríamos as duas tuplas exibidas na mesma figura, fruto de um acesso à visão como se a mesma fosse uma tabela, como Vende ou Cerveja.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb23.png]]

Veja que uma visão guarda apenas a expressão SQL, não os dados que são resultado da execução da consulta. Por isso, muitas vezes as visões são chamadas de tabelas virtuais, pois os dados não são armazenados, apenas a consulta que define a visão. Uma vez definida uma visão, esta pode ser usada para definir outras visões, e assim por diante.

Entre outras vantagens, a visão Bares_e_Medias pode ser manuseada exatamente como uma tabela, ocultando a expressão em SQL relativamente complicada para leigos na linguagem. É o que ilustramos na figura a seguir, em que realizamos consultas sobre a visão como se fosse mais uma tabela no esquema relacional das Cervejas. Se for mesmo uma consulta muito frequente, também temos por vantagem o fato de a expressão da consulta referente à visão já estar pré-compilada e com seu plano de execução ótimo pré-definido.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb24.png]]

As visões também podem ser usadas para ocultar atributos (ou colunas) presentes em tabelas persistidas no banco de dados, que não podem ser disponibilizadas, ou mesmo conhecidas, por uma parte dos usuários do banco. No caso da visão Bares_e_Medias, os detalhes de cada bebida, presentes na tabela Cerveja, não são exibidos, apenas a marca.

Também podemos considerar as visões para controle de integridade dos dados em um banco relacional. Nesse caso, além de criar a visão com o comando CREATE VIEW e o resto da expressão em SQL que define a consulta, é preciso adicionar a cláusula WITH CHECK OPTION ao final. Se fizéssemos isso com a visão Bares_e_Medias, e apenas essa visão fosse acessível aos usuários em geral, apenas cervejas brasileiras seriam aceitas no banco de dados por conta da restrição da cláusula WHERE igualando País ao valor “Brasil”. Esse controle seria feito diretamente no banco de dados, como parte da definição do esquema, e não precisaria mais ser incluído como trecho de código em programas e aplicações diversos.

Visões também podem ser usadas como interface para atualização de dados no banco. Há limites, mas, em alguns casos práticos, é possível trabalhar apenas com visões, evitando dar acesso direto às tabelas que estão persistidas no banco de dados, reduzindo possíveis manuseios não autorizados.

Abaixo seguem imagens, em que utilizamos um exemplo de esquema relacional simplificado das cervejas, chamado Beer, com apenas três tabelas com nomes similares, mas não exatamente com os mesmos esquemas relacionais.

![[Pasted image 20240520120828.png]]

![[Pasted image 20240520120841.png]]

![[Pasted image 20240520120917.png]]

![[Pasted image 20240520120928.png]]

![[Pasted image 20240520120940.png]]

![[Pasted image 20240520120951.png]]

![[Pasted image 20240520121014.png]]

![[Pasted image 20240520121038.png]]

![[Pasted image 20240520121104.png]]

![[Pasted image 20240520121120.png]]

![[Pasted image 20240520121134.png]]

![[Pasted image 20240520121144.png]]

![[Pasted image 20240520121153.png]]

![[Pasted image 20240520121202.png]]


Existem também visões temporárias, que são válidas apenas para consultas específicas, mas que mesmo assim são muito usadas na prática. Para isso, precisamos usar a cláusula WITH, como ilustramos na figura a seguir.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb25.png]]

Já tínhamos visto que é simples exibir o valor da cerveja mais barata, porém um pouco mais complicado expressar em SQL consultas que necessitam desse menor valor de venda nas suas soluções. Nesse exemplo, com a cláusula WITH, podemos definir uma visão temporária chamada cerveja_barata, que tem apenas uma coluna – o preço mínimo –, e utilizar essa “tabela virtual” na expressão da consulta em seguida que faz um INNER JOIN entre a tabela Vende e Cerveja_Barata.

Quando comentamos sobre limites da linguagem SQL com respeito a não contemplar controle de repetição ou recursão, como é o caso da consulta que deseja exibir todos os nomes em uma hierarquia familiar, algumas implementações em SGBDs relacionais conseguem contornar esse problema exatamente com a cláusula WITH. Como se trata de um assunto complexo e extenso, recomendamos ao aluno consultar as referências bibliográficas sugeridas para entender como consultas recursivas podem ser executadas com apoio da cláusula WITH.

### Índices em Bancos de Dados Relacionais

Terminaremos esta aula introduzindo rapidamente o conceito de índices em bancos de dados relacionais. Assim como temos índices em livros e enciclopédias, que permitem o acesso a capítulos ou páginas específicos, os esquemas relacionais também contam com índices para evitar que tenhamos de percorrer tabelas muito volumosas por inteiro, o que seria muito ineficiente.

Esse percurso completo de tabelas ou relações é conhecido como varredura sequencial (full scan, em inglês), e, sempre que possível, devemos evitar que ocorra na prática. Os índices são também objetos de bancos de dados relacionais que são criados como estruturas auxiliares de acesso aos dados.

Podemos definir os índices, de maneira simplificada, como estruturas contendo pares de valores referentes ao banco de dados: o primeiro valor é uma chave de busca (search-key), que é o valor que estamos buscando nas tabelas que compõem o esquema relacional. O segundo valor é a posição relativa (página ou bloco de disco mais registro) daquela chave de busca no arquivo que persiste os dados referentes a determinada tabela.

Na analogia com livros, a chave de busca pode ser determinado capítulo, e a posição relativa é a página em que se encontra aquele capítulo no livro. A figura a seguir ilustra essa noção de índices para o esquema das cervejas, considerando os arquivos correspondentes às tabelas Cerveja e Bar.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb26.png]]

No caso de bancos de dados relacionais, temos, basicamente, dois tipos de índices: os índices primários e os índices secundários. Os índices são estruturas de acesso sempre ordenadas pelo campo chave de busca. Índices fazem referência aos arquivos em que os dados de tabelas são persistidos.

Para os índices primários, os arquivos referenciados pelo índice também são ordenados pela chave de busca, que, nesse caso, são únicos e não se repetem, coincidindo com a definição de chave no modelo relacional – chave candidata ou chave primária (PK). Na Figura abaixo, temos um exemplo que ilustra de maneira simples um índice primário para o caso da tabela (e arquivo) Cerveja, em que constam os números de posição relativa de registros que implementam as tuplas de uma tabela. Não à toa índices primários remetem à ideia da existência da PK de uma tabela, que é o atributo Marca no caso da tabela Cerveja. Para criar um índice primário, basta definir uma PK com o comando **CREATE TABLE**.

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb27.png]]

Já os índices secundários também são estruturas ordenadas que referenciam arquivos que não são ordenados pelo campo chave de busca, e podemos ter valores repetidos. A Figura abaixo ilustra um índice secundário da mesma tabela (arquivo) com dados de cervejas, considerando agora a coluna País como referência de indexação. Enquanto índices primários são criados indiretamente na hora da criação de tabelas, os índices secundários são criados explicitamente por um comando **CREATE INDEX**. Neste exemplo, o comando respectivo poderia ser CREATE INDEX IDX-PAIS ON Cerveja (País).

![[pos-graduacao/1º Acervo de imagens (Disc. 2)/stb28.png]]

Os índices, primários ou secundários, podem ser simples ou compostos. São considerados simples quando apenas uma coluna é referenciada, e compostos nos demais casos.

Existem também os chamados **índices multinível**, que são formados de estruturas de índices que referenciam outros índices. Se temos um arquivo muito grande que representa uma tabela, um índice também pode ser muito grande, precisando de **“um índice para o índice”**. As estruturas do tipo árvore B (_B-tree_) são índices multinível que são utilizados em diversos SGBDs comerciais para implementar os índices primários e secundários.

Quando um sistema de banco de dados apresenta problemas de desempenho, muitas vezes o _database administrator_ (DBA), ou analista responsável, opta pela criação de índices para que as consultas e transações, de maneira geral, executem em menor tempo ou em maior quantidade na mesma quantidade de tempo (vazão ou _throughput_). É esperado que o otimizador do SGBD leve em consideração tais índices, visando à melhoria do sistema como um todo.

Criar índices é uma das tarefas mais comuns que DBAs ou usuários especialistas em bancos de dados realizam na manutenção de um banco de dados. Ajustar um sistema de banco de dados que está em produção, buscando maior eficiência, é uma atividade também conhecida por sintonia fina de banco de dados (_database tuning_).

Sabemos que no projeto conceitual e no projeto lógico de um banco de dados a ênfase é atender aos requisitos de dados e funcionais. No projeto físico, a prioridade é a _performance_, e é nesse momento que os índices são considerados, assim como as visões.

Cabe observar que uma das estratégias mais utilizadas para melhoria de desempenho em bancos relacionais é a desnormalização. Esse termo é usado para fazer referência ao processo de normalização de um banco de dados, visto na segunda aula. Desnormalizar significa, em geral, reunir duas ou mais tabelas que foram criadas separadamente em uma única tabela, evitando a execução de junções, que são operações frequentes e muito caras. Daí a importância de conhecer o processo de projeto usando formas normais, pois, caso contrário, o ato de desnormalizar um esquema relacional não faria sentido.

Sabemos que podemos ter somente um índice primário para cada relação, pois este define a ordenação da tabela. Entretanto, é possível disponibilizar vários índices secundários. Os índices evitam buscas sequenciais, algo fundamental quando lidamos com grandes volumes de dados. Assim, seria natural imaginar que deveríamos criar a maior quantidade de índices possível, pois eles serão úteis para melhorar o desempenho de acesso ao banco de dados. Algo similar é feito pelos buscadores na _web_, como Google ou Bing, que, em seus sistemas de recuperação de informações (_information retrieval_), criam diversos índices para que se possa chegar rapidamente aos resultados das buscas pelas palavras-chave entradas pelos usuários. Entretanto, muitos analistas de sistemas e programadores costumam dizer que “índices são bons para fazer consultas, mas ruins para atualizações”. Você concorda com essa afirmação?

### Códigos & Links:

Aula 3 - https://colab.research.google.com/drive/1SoCb1igfHy1IDiCXiTIcyd5gP2rz8zVj#scrollTo=LjwzX0mllZ6T

### Referências:

COSTA, R. L. de C. **SQL**: guia prático. Rio de Janeiro: Brasport, 2006.

ELMASRI, R.; NAVATHE, S. B. **Sistemas de bancos de dados**: fundamentos e aplicações. [_s.l._]: Pearson, 2010.

GARCIA-MOLINA, H. **Implementação de sistemas de bancos de dados**. Rio de Janeiro: Campus, 2001.

HEUSER, C. A. **Banco de dados relacional**: conceitos, SQL e administração. Porto Alegre: Clube de Autores, 2019.

RAMAKRISHNAN, R.; GEHRKE, J. **Sistemas de gerenciamento de bancos de dados**. Porto Alegre: McGraw-Hill, 2008.

SILBERSCHATZ, A.; KORTH, H. F.; SUDARSHAN, S. **Sistema de bancos de dados**. Rio de Janeiro: Elsevier-Campus, 2012.

# Desenvolvimento Full Stack Básico (Disciplina 3)

## Primeiros passos no desenvolvimento de um sistema web (Aula 1)

Com a criação da rede mundial de computadores, e sua grande adoção, foi necessário criar um caminho a ser seguido para dar continuidade a expansão da rede, de forma que a infraestrutura pudesse acompanhar .

Dito isso, em 1993, Roy Fielding, cofundador do Apache HTTP Server Project, propôs que a escalabilidade da _web_ fosse governada por um conjunto de _key constraints_ (restrições/limitações-chave). Segundo ele, a continuidade da expansão seria possível se cada uma dessas restrições fosse atendida de forma igual.  
  
Essas restrições/limitações ainda são válidas e devem ser observadas e atendidas no desenvolvimento de qualquer sistema _web_ (COOKSEY, 2014). Fielding as categorizou em seis grupos:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/stb-03.png]]

#### Cliente-Servidor

Essa restrição é relativa à separação de responsabilidades na _web_ entre aplicações cliente e servidor. Elas têm responsabilidades diferentes, mas complementares. Além disso, podem ser implementadas e publicadas separadamente, independentemente das tecnologias utilizadas em seu desenvolvimento, desde que existam interfaces uniformes de comunicação entre elas. Portanto, não importam a linguagem, a tecnologia ou o comportamento interno, desde que haja uma forma conhecida de comunicação. Descubra mais a seguir:

Cenário de interação entre três aplicações: browser que acessa a web, servidor que mantém a aplicação e servidor de dados. Este é um cenário comum e ao longo do curso iremos explorar esses e outros cenários.

![[Pasted image 20240522155716.png]]

1. No contexto desta aula, esta imagem também ilustra como pode se dar o relacionamento cliente/servidor.
2. Na imagem, o servidor da aplicação serve ao cliente (browser) um conteúdo web, ao mesmo tempo em que assume o papel de cliente para servidor de dados. Ou seja, nesse cenário, o servidor da aplicação consome informações da base de dados e as retorna para o usuário final via browser (cliente da aplicação).

#### Uniformidade de interfaces

Como ilustrado na restrição de arquitetura cliente/servidor, a comunicação entre aplicações depende da uniformidade de suas interfaces, ou seja, a forma de comunicação deve ser conhecida entre as partes. Esse ponto é tão crucial que vários padrões foram e ainda são definidos para auxiliar essa uniformização. Fielding destaca quatro pontos que devem ser observados:

![[Pasted image 20250120223509.png]]

1. Identificação de recursos:  
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02.png]]

2. Manipulação de recursos via representações:
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/03.png]]

3. Uso de mensagens autodescritivas:
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/04.png]]

4. Hipermídia como motor de estados da aplicação (Hateoas):
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/05.png]]

#### Sistema em Camadas

Essa restrição de arquitetura da _web_ existe para permitir que serviços intermediários possam ser criados para atuar entre o cliente e o servidor sem impactar a experiência do cliente. O sistema intermediário é transparente para a aplicação cliente. Um exemplo prático e simples é o _proxy_, que age como um intermediário entre cliente e servidor. Uma vez configurado o _proxy_, o serviço se torna transparente e o cliente acessa o recurso de interesse sem que seja nítida sua presença.  
  
A restrição de arquitetura em camadas também pode servir para outros propósitos. Por exemplo, na imagem a seguir, temos um sistema em três camadas: o cliente (representado pelo _browser_) está na camada 0; o servidor da aplicação está na camada seguinte; e o acesso aos dados só é possível na terceira camada. Nessa arquitetura, o cliente não tem acesso direto aos dados, pois não estão em camadas vizinhas. Ainda assim, é transparente para o cliente a existência da terceira camada. Veja a seguir:

![[stb-06.png]]

#### Cache

Esse é um dos pontos mais importantes da arquitetura _web_. O objetivo dessa restrição é exigir da aplicação servidor que declare se o dado enviado em uma resposta a uma requisição é “cacheável”, ou seja, se pode ser armazenado em memória para evitar que outra requisição que o peça seja feita em curto prazo de tempo.

O _cache_ de uma resposta pode ajudar na “percepção de latência” do cliente, aumentando a disponibilidade de um recurso e reduzindo a carga do servidor da aplicação.

O cliente que precisa acessar um mesmo recurso mais de uma vez vai perceber rapidez na resposta, quando, na verdade, o recurso foi guardado no _cache_ do _browser_ ou em qualquer outro servidor/provedor de internet que possa existir no caminho até o servidor. Do outro lado, foram várias requisições do cliente, mas para o servidor da aplicação foi apenas uma resposta. Isso representa uma economia de recurso e maior disponibilidade para atender a outras requisições e clientes.

#### Stateless (Ausência de Estado)

Essa restrição de arquitetura determina que um servidor _web_ não necessita memorizar os estados da aplicação cliente. Como resultado, o cliente deve incluir toda informação de contexto que possa ser considerada relevante na requisição, para qualquer iteração com o servidor. Livre dessa preocupação, um servidor pode atender a diferentes clientes de forma ágil.

Quanto mais complexo o contexto e maior a informação enviada, menor a capacidade de atendimento do servidor. Balancear esses dois fatores é importante para contribuir com a escalabilidade da aplicação servida.

#### Code-On-Demand

Essa restrição de arquitetura da _web_ permite que servidores possam enviar pequenos trechos executáveis de código, como _scripts_ e _plug-ins_, para clientes. O objetivo é permitir que a aplicação servidora possa oferecer um meio para a aplicação cliente interpretar um dado enviado. Com isso, o código enviado habilitaria o cliente a interpretar o dado enviado pelo servidor.

Essa restrição é a única que pode ser considerada opcional entre todas as apresentadas. Ela é muito comum quando se utilizam tecnologias como Java Applets e JavaScripts.

### O Protocolo HTTP

Como apresentado no tópico anterior, os trabalhos de Fielding e Berners-Lee pavimentaram o caminho para o crescimento da _web_, que continua em plena expansão. Neste curso, vamos nos restringir ao desenvolvimento de sistemas que atuam no ambiente web e utilizam o protocolo HTTP para comunicação.

A comunicação em HTTP reside no conceito de **ciclo de requisição e resposta**: o cliente envia uma requisição para o servidor com a expectativa de receber uma resposta (BIEHL, 2011).

Para fazer uma requisição em HTTP a aplicação cliente precisa informar:

![[Pasted image 20250120223625.png]]

1. URL (Localizador padrão de recursos, ou uniform resource locator):
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02 1.png]]

2. Método:
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/03 1.png]]

3. Cabeçalho:
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/04 1.png]]

4. Corpo da requisição:
![[pos-graduacao/1º Acervo de imagens (Disc. 3)/05 1.png]]

Depois que o servidor receber a requisição, irá tentar fazer o que foi solicitado e retornar uma resposta. Essa resposta terá uma estrutura similar à da requisição, mas, em vez do URL e do método, informará o _status code_, que, como já mencionado, é um valor numérico que representa uma mensagem autodescritiva que informa o estado final da execução do que foi solicitado. Veja um resumo dos diferentes códigos e seus significados:

![[stb-08.png]]

O cabeçalho também é alterado na resposta do servidor, passando informações relevantes para a construção da representação da resposta. Por exemplo, o dado _Content-type_ informa o tipo de dado retornado para indicar ao cliente como interpretá-lo. A imagem a seguir apresenta um resumo comparativo da estrutura de requisição e resposta:

![[stb-09.png]]

#### Padrões de Arquitetura em Sistemas Web

Um sistema _web_ é um _software_ e, sendo assim, sua arquitetura deve ser bem planejada para facilitar seu desenvolvimento, manutenção e evolução. A importância de uma boa arquitetura é fácil de justificar, pois define a base para o desenvolvimento da aplicação, influenciando diretamente diferentes aspectos do sistema, como mostrado por Biehl (2011). Veja a seguir, clicando nos títulos:

![[Pasted image 20240522164323.png]]

O projeto da arquitetura deve ser guiado com base nos objetivos esperados para a aplicação. Como a importância de cada um desses aspectos pode variar com o projeto, a arquitetura do sistema deve ser aderente a seus objetivos. No entanto, vale ressaltar que ela também pode evoluir. Sendo assim, a evolução da aplicação é mais um aspecto a ser considerado.  
  
Com isso, não há um padrão de arquitetura, mas vários, e a escolha vai depender das necessidades e objetivos do sistema. Neste curso, por ser um módulo básico, vamos focar uma estratégia simples de arquitetura _web_ de apenas três camadas. Vamos explorar a separação de responsabilidade e o respeito às restrições de arquiteturas mencionadas anteriormente. Veja como será destacado na arquitetura deste sistema:

![[stb-11.png]]

Nessa proposta de arquitetura, duas aplicações do lado do servidor, em duas camadas diferentes, tratarão de responsabilidades específicas: uma servirá a apresentação (_front-end_) e a outra fará a execução de lógicas de negócio e o envio de dados.  
  
Essa simples separação de responsabilidades pode ser suficiente para a construção de um sistema _web_ escalável. A persistência e a leitura de dados em banco geralmente têm um custo elevado de tempo, pelas consultas realizadas. Por outro lado, a construção da representação, da página final que será respondida ao _browser_, tem, geralmente, um custo bem menor de tempo e processamento. Com isso, essa separação permite que, em um cenário de alta demanda, seja possível publicar mais de uma instância do servidor de dados, para aumentar a disponibilidade geral do lado deste.

**Supondo um cenário de alta demanda**

![[Pasted image 20240522171737.png]]

Para mais de uma instância de um mesmo servidor publicado na _web_, é necessário um componente para o balanceamento de cargas, o **_load balancer_**. Graças às restrições de ausência de estados e de sistemas em camada, o _load balancer_ é transparente para o cliente (assim como um _proxy_) e age como um gerenciador de fluxos. Ele recebe a requisição do cliente e a encaminha para uma instância do servidor que está disponível. Depois de processada a requisição, a resposta é enviada para o _load balancer_ e encaminhada para o cliente.

![[image-text-5.jpg]]

### Padrão MVC

Uma preocupação recorrente no projeto de arquitetura de um sistema _web_ é a separação de responsabilidades e a uniformização das interfaces. Nesse sentido, o modelo visualização e controlador (MVC – _model-view-controller_) é um padrão de projeto de arquitetura de _software_ muito aderente ao desenvolvimento _web_.  
  
Em termos de flexibilidade, não importa de onde o conteúdo vem ou como é enviado, mas, sim, o **modelo** do dado, como ele é representado. Sabendo como é a estrutura do dado, o conteúdo pode ser transformado em uma representação (ou **visualização**), de acordo com o mecanismo de controle (o **controlador**) encarregado de selecionar o dado, definir o modelo e escolher a melhor visualização (SHKLAR; ROSEN, 2009). Confira nesta imagem:

![[stb-13.png]]

#### Estudo complementar

Para ampliar seus conhecimentos, leia o capítulo “Construção do modelo MVC de um cenário real”, você vai aprender a desenvolver o modelo MVC no respectivo cenário, em conjunto com um banco de dados.

Para ler este livro, busque o _link_ no _card_ **leituras**, dentro da disciplina no AVA.

Livro: Programação _back-end_ II

### Técnica Aplicada

Agora que já temos um bom conhecimento sobre a teoria, vamos exercitar um pouco implementando um servidor de aplicação _web_. Vamos explorar seu desenvolvimento, utilizando Python, Flask e SQLite. Aqui, vamos apresentar duas versões de um mesmo sistema: um único servidor de aplicação, como apresentado em (A); e um servidor de dados, como apresentado na camada 2 de (B). Observe com atenção:

![[stb-14.png]]

O objetivo de apresentar da técnica é a implementação de rotas com os verbos mais do HTTP e mostrar dois diferentes cenários: um servidor que retorna HTML e outro que retorna JSON. Com isso, mostra-se a transição de um sistema monolítico para um com divisão de responsabilidades que faz uso de uma API para acesso à camada de dados.

![[Pasted image 20240523155542.png]]

### Referências:

BERNERS-LEE, T. _et al._ Uniform resource identifier (URI): generic syntax. **Datatracker**, 2005. Disponível em: [https://datatracker.ietf.org/doc/html/rfc3986](https://datatracker.ietf.org/doc/html/rfc3986). Acesso em: 28 ago. 2022.  
  
BIEHL, M. **REST API design rulebook:** designing consistent RESTful web service interfaces. Sebastopol: O'Reilly Media, 2011.  

COOKSEY, B. **An introduction to APIs**. [_S. I._]: Bryan Landers and Danny Schreiber, 2014. Disponível em: [https://zapier.com/learn/apis/](https://zapier.com/learn/apis/). Acesso em: 23 out. 2022.  

FIELDING, R. _et al._ Hypertext transfer protocol: HTTP/1.1. **Datatracker**, 1999. Disponível em: [https://datatracker.ietf.org/doc/html/rfc2616](https://datatracker.ietf.org/doc/html/rfc2616). Acesso em: 28 ago. 2022.  

MASSE, Mark. **Rest API Design Rulebook**: Designing Consistent Restful Web Service Interfaces. O'Reilly Media. 1ª edição. 2011. ISBN-10: 1449310508.  

UNIVERSITY OF OXFORD. Share of the population using the internet. **Our World In Data**, 2020. Disponível em: [https://ourworldindata.org/grapher/share-of-individuals-using-theinternet](https://ourworldindata.org/grapher/share-of-individuals-using-theinternet). Acesso em: 28 ago. 2022.  

SHKLAR, L.; ROSEN, R. **Web application architecture**: principles, protocols and practices. 2. ed. Hoboken: John Wiley & Sons, 2009.

## Implementando um Projeto de Interface (Aula 2)

### HTML

Tim Bernes-Lee, além de criador da _web_, criou também o HTML, a linguagem de marcação de hipertexto (ou _HyperText Mark-up Language_). **O termo “hipertexto”** é utilizado para descrever um texto que contém _links_ para outros textos, e **o HTML** é uma linguagem de marcação utilizada para produzir textos (documentos) que são interpretados por navegadores. Esse tipo de documento permite estruturar a informação que será exibida para o usuário, como títulos, parágrafos e listas.

- O HTML é uma combinação de textos com códigos especiais (_tags_ ou etiquetas).
- As _tags_ possibilitam a estruturação do conteúdo do documento e dão instruções ao navegador sobre o que deve ser feito.
- Elas são declaradas entre parênteses angulares (‘<’ e ‘>’), e a maioria das _tags_ tem sua correspondente de fechamento (que terá uma barra comum: < /nomedatag >).

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02 2.png]]

Um documento HTML tem sua estrutura básica definida por _tags_. O HTML5 (uma versão mais atualizada do HTML) é atualmente suportado por todos os navegadores, e uma página _web_ (um documento) padrão tem a seguinte estrutura:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/STB02.png]]

O significado de cada uma das _tags_ no Código 1 é apresentado na tabela a seguir:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/STB03.png]]

Ao abrir esse conteúdo em um navegador (antes seria necessário salvá-lo com a extensão “.html”, por exemplo, index.html), ele será interpretado, e o resultado será apresentado como podemos ver na imagem a seguir:

![[STB04 2.png]]

Esse resultado é um primeiro passo, mas ainda falta estilo. E é nesse ponto que entra o CSS (_Cascading Style Sheets_).

Vale destacar que apenas executamos o arquivo HTML utilizando o _browser_. Não houve qualquer interação com um servidor, apenas a construção de uma representação com base nos comandos escritos no arquivo HTML. Observe que, em vez da URL, no navegador, aprece apenas o caminho para o arquivo.

### CSS

O CSS é uma linguagem de folha de estilo que é aplicada para definir como os elementos HTML devem ser apresentados em uma página da _web_ em termos de _design_, _layout_ e variações para diversos dispositivos com diferentes tamanhos de tela.

O CSS possibilita personalizar fontes, cores, margens, linhas, alturas, larguras, imagens de fundo, posicionamentos e outras tantas características a elementos de documentos codificados em HTML. De forma geral, o CSS é uma coleção de regras (cada regra é direcionada para uma _tag_ específica ou elemento do HTML). Confira:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02 3.png]]

No código a seguir, temos um exemplo de como declarar a cor vermelha para as _tags_ de parágrafo. Neste exemplo, é apresentado um seletor de elemento. Entretanto, existem outros tipos de seletores, como de classe, que inicializa com ponto antes do nome da classe (._nomeClasse_), e _id_, que inicializa com _hashtag_ antes do nome do _id_ (#_nomeId_). Vamos ver o exemplo:

![[STB06 2.png]]

- O CSS pode ser incorporado dentro do código HTML, porém geralmente, e por boas práticas, ele é escrito em um arquivo ._css_, facilitando a manutenção.

- Para introduzir esse arquivo no Código 1, é necessário adicionar a _tag_ <_link_> e seus atributos dentro da <_head_>. Essa _tag_ define o relacionamento entre o documento atual e um recurso externo.

- Todos os elementos HTML podem ser considerados como caixas no CSS. Para esse encapsulamento que é utilizado para _design_ e _layout,_ temos a expressão “modelo de caixa” (_model box_).

Ele consiste em margens, bordas, preenchimento/espaçamento e o conteúdo real. Uma caixa funciona como um contêiner, ou seja, permite que existam, dentro de si, outras caixas (caixas descendentes). Por meio dessa estruturação de caixas, é possível organizar a apresentação de diferentes elementos ao longo do documento HTML. Vamos conferir na imagem abaixo, que apresenta cada elemento do modelo de caixa:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/01.png]]

![[Pasted image 20240524160134.png]]

![[Pasted image 20240524160153.png]]

![[Pasted image 20240524160209.png]]

![[Pasted image 20240524160230.png]]

Embora o CSS permita definir todos os valores, caso eles não sejam explicitamente definidos, serão renderizados de acordo com as propriedades padrão de cada navegador.

![[STB09 3.png]]

As unidades de medida comumente utilizadas são:  
- **%:** porcentagem do tamanho disponível;
- **em:** relativo (multiplicador) ao tamanho da fonte do elemento;
- **cm/mm/in:** tamanho em centímetros, milímetros ou polegadas, respectivamente;
- **pt:** pontos, sendo que um ponto equivale a 1/72 polegadas;
- **px:** _pixels_, tamanho do _pixel_ do dispositivo onde a página foi renderizada;
- **vh:** _viewport height_ (altura visível), em que 100vh representa o tamanho total e 1vh representa 1% desse tamanho;
- **vw:** _viewport width_ (largura visível), em que 100vw representa o tamanho total e 1vw representa 1% desse tamanho.

### JavaScript

O JavaScript (ou apenas JS) é a linguagem de programação mais utilizada para o desenvolvimento de interfaces de usuário para a _web_. Ele possibilita que os desenvolvedores adicionem interatividade e comportamentos dinâmicos aos seus _sites_, como reações de eventos do usuário, carregamento de dados de serviços da _web_, exibição ou ocultação de elementos em uma página, controles deslizantes de imagem, _pop-ups_ e muito mais. O JavaScript também é o responsável por fazer a comunicação com o _back-end_ do sistema (caso exista um).

Segundo a Mozilla Foundation, atual nome da antiga Netscape Communications Corporations, empresa responsável pela criação do JS:

**“JavaScript é uma linguagem de programação leve, interpretada, orientada a objetos, baseada em protótipos e em _first-class functions_ (funções de primeira classe), mais conhecida como a linguagem de _script_ da internet.”**

Como uma linguagem de programação dinâmica, o JavaScript não precisa ser executado por meio de um compilador. O navegador efetivamente lê o código da mesma maneira que nós, humanos, e o interpreta em tempo real. O JavaScript é interpretado pelo navegador (que tem um interpretador JavaScript embutido).

Com isso, o navegador recebe o conteúdo da página HTML, interpreta o código JavaScript e o executa. Esse processo é feito de forma síncrona. O Código 3 é um exemplo de código JavaScript que exibe um pedido de confirmação ao usuário em uma caixa de diálogo, sendo executado sem necessidade de comunicação com o _back-end_. Veja um exemplo:

![[STB08 2.png]]

O código JavaScript também pode ser incorporado dentro do código HTML. Porém, da mesma forma que o CSS, recomenda-se utilizar em um arquivo .js separado e introduzi-lo com a _tag_ <_script_> (usada para incluir ou referenciar um _script_ executável) e seus atributos dentro da _tag_ <_body_>. Assim, facilita a legibilidade do código e possibilita a reutilização em múltiplos arquivos HTML.

**É importante destacar que um uso muito comum do JavaScript é modificar dinamicamente HTML e CSS para atualizar uma interface do usuário sem que seja necessário recarregá-la, por meio da API do _Document Object Model_ (DOM).**

O DOM é uma interface de programação para os documentos HTML e XML. Ele interpreta a página para que o JavaScript possa modificar a estrutura, o estilo e o conteúdo. O DOM representa o documento como nós e objetos. Dessa forma, as linguagens de programação podem se conectar à página. A estrutura do DOM é uma estrutura de árvore. Então, é possível, a partir do acesso ao nó raiz _Document,_ acessar todos os nós filhos, além de acessar também os objetos dos nós, como os atributos, por exemplo. De forma sucinta, o conteúdo da página é armazenado no DOM e pode ser acessado e manipulado via JavaScript. Confira:

![[STB09 2.png]]

Em relação ao _front-end_, HTML, CSS e JavaScript continuam sendo linguagens base para o desenvolvimento de interfaces, porém muitas outras ferramentas e estruturas surgiram ao longo do tempo.

A figura apresenta uma visão simplificada das principais tecnologias existentes atualmente. Vamos verificar:

![[STB10 2.png]]

### Frameworks e Bibliotecas

_Frameworks_ são modelos para criar um _site_ ou uma aplicação _web_. Eles fornecem uma estrutura (como um esqueleto ou andaime) para organizar todo o projeto. Enquanto a estrutura define os modelos de página, eles constroem a estrutura com áreas alocadas específicas para incorporar um código de estrutura.

Um _framework_ JavaScript é um conjunto completo de ferramentas para a construção completa de páginas ou aplicações _web_. Principais _frameworks_: [Vue](https://vuejs.org/) e [Angular](https://angular.io/).

Por sua vez, bibliotecas são conjuntos de trechos de códigos pré-escritos que visam a auxiliar o desenvolvimento e que podem ser usados e reutilizados para implementar os principais recursos do **JavaScript.** Assim, as bibliotecas são ferramentas especializadas para necessidades específicas de codificação, não uma máquina multifuncional para preparar todo o projeto existente.

Principais bibliotecas:
- [**React**](https://reactjs.org/)
- [**jQuery**](https://jquery.com/)

O **React não é um _framework_**. Assim, para todas as coisas que o desenvolvedor quiser fazer que não tenham a ver com a renderização do _front-end_, será necessário instalar uma biblioteca de terceiros. Isso é uma vantagem, pois só é preciso instalar o que é necessário para a aplicação, deixando-a mais leve.

### React

Em maio de 2013, em uma conferência de JavaScript nos Estados Unidos, uma nova biblioteca revolucionária, chamada React, foi apresentada. Essa biblioteca foi criada por Jordan Walke, engenheiro de _software_ que trabalha para o Facebook. Essa biblioteca foi desenvolvida para superar problemas com o manipulador de eventos no _site_ do Facebook.

O ReactJS foi desenvolvido para seguir o fluxo de dados unidirecional, geralmente conhecido como vinculação de dados unidirecional. A vinculação de dados unidirecional fornece mais controle sobre o aplicativo como um todo.

Por apresentar grande eficiência, nos anos seguintes o React foi integrado à interface de outras redes sociais do grupo, como o Instagram, e em 2013 seu código foi aberto à comunidade, que iniciou sua popularização. Atualmente, o React é uma das bibliotecas JavaScript mais populares do mercado.

Um dos objetivos do React é facilitar a conexão entre diferentes partes de uma página, havendo, assim, um funcionamento por meio de componentes.

Os componentes do React são escritos usando uma extensão para JavaScript chamada JSX, que permite combinar código JavaScript e HTML.

Os componentes podem ser compostos juntos para criar elementos de interface do usuário complexos e aplicativos inteiros. Esses componentes são utilizados para reaproveitamento de código e padronização de interface.

Como mencionado anteriormente, as páginas de um _site_ ou aplicativo são efetivamente atualizadas por meio do DOM. No entanto, o React usa um ambiente chamado DOM virtual (uma representação na memória de um DOM) para atualizar uma página. Isso ocorre porque o manuseio de um DOM virtual é muito mais rápido que a manipulação de um DOM real, ou seja, a página que está sendo atualizada.

### Gerenciador de Pacotes

Outro aspecto importante do _front-end_ são as tecnologias responsáveis pelo gerenciamento e execução desses pacotes e dependências. Elas permitem que você utilize pacotes e dependências existentes em um projeto, trazendo maior facilidade ao desenvolvimento, assim como o uso do React, que vem apenas com o necessário, e, dependendo da necessidade, novas bibliotecas precisam ser instaladas.

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/STB11.png]]

Além da instalação de bibliotecas em diferentes ambientes, também é possível:  
- **publicar uma biblioteca desenvolvida;**
- **compartilhá-la com outros desenvolvedores.**

Outra funcionalidade é que os pacotes permitem executar _scripts_ que podem ser utilizados para executar testes, análise e compilação de códigos.

Uma vantagem do uso do NPM é o fato de ele já vir instalado automaticamente com o Node.js, o que facilita muito sua utilização.

O Node.js é um ambiente de tempo de execução JavaScript _open-source_ e multiplataforma. Por meio dele é possível desenvolver pequenas e grandes aplicações.

Atualmente, muitas das ferramentas de _front-end_ e _back-end_ são baseadas em Node.

### Bibliotecas de Componentes

As bibliotecas de componentes são coleções de componentes que podem ser usados e modificados para montar uma aplicação. Algumas delas implementam apenas os componentes mais comuns, como botões e menus suspensos, e outras também fornecem utilitários para criar _layouts_ responsivos complexos. Esses componentes já têm um estilo visual próprio, mas é possível personalizá-los para atender às necessidades do projeto. Destacamos as bibliotecas mais populares para uso em um projeto React. Veja:

![[Pasted image 20240524163807.png]]

O Bootstrap e o Material UI têm ajudado os desenvolvedores a construírem interfaces há anos, e, como ambos são gigantes na indústria, há sempre a questão de qual é o melhor. Alguns consideram que o Bootstrap ajuda os desenvolvedores a tornarem os _sites_ responsivos mais rápidos e que o Material UI é focado em criar uma experiência melhor do usuário com os elementos da interface. No entanto, em geral, não existe uma resposta certa para essa pergunta. Ela depende da preferência dos desenvolvedores ou dos requisitos de cada projeto.

### Front-End e a Inteligência Artificial

Ao prosseguirmos esta aula, somos capazes de fazer uma relação entre _front-end_ e inteligência artificial. O sistema IA GPT-3 (_Generative Pre-Training Transformer 3_ – Transformador Generativo Pré-Treinado 3) é uma inteligência artificial especializada na produção de texto desenvolvida pela OpenAI que se baseia em técnicas de aprendizado profundo para conseguir produzir conteúdo a partir de instruções mínimas.  

Esse sistema tem a capacidade de, a partir de textos com alguns requisitos básicos de _layout_, gerar código com estrutura semelhante ao JSX do React e estilos com ligeira fidelidade ao que foi pedido. Com isso, a discussão sobre a possibilidade de as inteligências artificiais substituírem programadores, principalmente desenvolvedores _front-end_, voltou à tona.

Em uma publicação da Tableless intitulada [“O fim da profissão _front-end_”](https://tableless.com.br/carreira-de-front-end-vai-morrer/), alguns pontos são abordados, o que nos leva às seguintes indagações:
- **O que diferencia uma pessoa _front-end_ de uma ferramenta?**
- **Até que ponto uma ferramenta conseguiria realizar o trabalho de um desenvolvedor _front-end_?**

**Papel do usuário no processo de desenvolvimento _front-end_**:

Tanto o desenvolvedor _back-end_, quanto o _front-end_, não podem esquecer que estão desenvolvendo aplicações para pessoas. Pensar no perfil de usuários é parte importante em qualquer desenvolvimento, veja o exemplo abaixo:

![[STB13 3.png]]

O objetivo da aplicação é facilitar a vida do cliente na contratação de serviços. No entanto, para alcançar esse objetivo, ela precisa saber comunicar ao usuário todas as funcionalidades que apresenta. **Pensando nisso, qual seria o papel do cliente no desenvolvimento _front-end_?**

### Referências:

DUCKETT, Jon. **HTML & CSS**: design and build websites. Indianapolis, IN: Wiley, 2011.  
  
FLANAGAN, David. **JavaScript**: o guia definitivo. Bookman Editora, 2004.  
  
MELONI, Julie C.; KYRNIN, Jennifer. **HTML, CSS, _and_ JavaScript All in One, Sams Teach Yourself**: Covering HTML5, CSS3, and ES6, Sams Teach Yourself. Sams Publishing, 2018.  
  
ROBBINS, Jennifer Niederst. **_Learning web design_**: A beginner's guide to HTML, CSS, Javascript, and web graphics. “ O'Reilly Media, Inc.”, 2012.  
  
WIERUCH, Robin. **_The road to react: Your journey to master plain yet pragmatic react. js_**. Robin Wieruch, 2017.  
  
Projeto colaborativo. MDN Web Docs, 2005. **Documentação de tecnologias da web, incluindo CSS, HTML e JavaScript**. Disponível em: [https://developer.mozilla.org/pt-BR/](https://developer.mozilla.org/pt-BR/). Acesso em: agosto de 2022.

## Documentação e Deploy (Aula 3)

### Conectando as partes: conectando camadas via API

Ao fim da primeira aula, foi apresentado o desenho feito em Python de um pequeno servidor para uma API utilizando bibliotecas comuns de mercado. Já ao fim da segunda aula, mostramos o desenvolvimento do _front-end_ que iria usar a API vista na primeira aula. Agora, é a vez de conectar essas pontas. Observe a imagem:

![[Pasted image 20240527153620.png]]

Para essa conexão, o _front-end_ fará chamadas via JavaScript para a API. É necessário lembrar que o JavaScript permite adicionar dinamismo ao que deveria ser estático (no início da _web_, a ideia era somente servir páginas HTML, ou seja, conteúdo estático). A seguir, temos um trecho de código que ilustra uma forma de fazer essa conexão:

![[STB02 3.png]]

Na Aula 1, vimos que o método GET é utilizado para requisitar um recurso. Em nosso exemplo, o resultado esperado para essa requisição é um dado no formato JSON (linha 11).

### Documentação

Em uma breve definição, podemos afirmar que um _software_, seja qual for a sua natureza, é representado por uma coleção de códigos (comandos). O código, por sua vez, é um texto escrito seguindo um padrão definido por uma linguagem de programação.

Podemos ir além nessa definição: independentemente da linguagem, todo código é também um meio de comunicação, não só entre programadores, mas entre programadores e usuários. Programadores precisam trabalhar em colaboração entre si, tendo como finalidade atender à necessidade de um usuário. Por esse ângulo, o código é o meio pelo qual o programador conversa com o usuário. Como em todo processo de comunicação, para ser eficaz, é necessário garantir a compreensão entre as partes do processo.

#### Para permitir a evolução do sistema

Por ora, vamos focar o cenário em que o código pode ser visto como meio de comunicação entre programadores. A preocupação com a legibilidade do código não deve estar apenas na escolha dos nomes dos módulos, classes, funções e variáveis.

A documentação do código tem papel importante na garantia da legibilidade. É nela que parâmetros de entradas e saídas serão explicados e exemplificados, funções e classes terão suas existências justificadas e descrições de testes serão adicionadas. Tudo isso para garantir o máximo de informação para uma boa compreensão do código, permitindo o desenvolvimento colaborativo do _software_.

Como ressalta Guido van Rossum, criador da linguagem Python, **“código é muito mais lido que escrito”.** Você pode passar até dias programando um trecho de código para uma funcionalidade importante, como o módulo de autenticação de usuários, mas pode ter certeza de que terá que voltar ao código e lê-lo novamente. Enquanto esse código existir, você terá que ir novamente ao arquivo e relembrar quais são as regras de negócios, como cada uma delas foi implementada e por quê.

Essa preocupação não se justifica apenas como facilitadora no desenvolvimento do _software_, mas a própria evolução deste pode ser facilitada com a qualidade da documentação. Um cenário muito comum no cotidiano de um programador é deparar-se, na manutenção de um código legado, com uma completa falta de clareza sobre o que está sendo feito. Entenda melhor:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/STB03 1.png]]

#### No contexto do desenvolvimento ágil

É importante ressaltar que a documentação não existe somente para o código, mas também para a arquitetura, dados, testes e instalação do _software_. Ela deve estar presente em todas as etapas de desenvolvimento do _software_, que não se limitam à codificação. Todas as decisões relativas às funcionalidades do _software_ devem ser documentadas, desde o levantamento de requisitos até a avaliação com o usuário. Veja:

![[STB04 3.png]]

### Comentários e Documentação de Código

Para qualquer linguagem de programação, deve haver pelo menos uma forma de documentação de código. Para Java, por exemplo, há o JavaDoc, que define uma coleção de diretivas que auxiliam o processo de documentação durante a programação. Veja este exemplo:

![[STB05 2.png]]

Segundo Martin (2009), o propósito por trás do uso de comentários é compensar a falha do programador em explicar a si mesmo em código. Ele também diz que a necessidade de comentários se justifica porque não somos sempre capazes de nos expressar somente em código. No entanto, afirma que nem todo comentário é relevante.

"Comentários imprecisos são piores do que nenhum comentário. Eles confundem, te levam a falsos entendimentos e criam expectativas que nunca serão realidade."                 - (MARTIN, 2009, p.54)

São vários os motivos que justificam o uso de comentários em código. No livro _Clean Code_, Martin destaca seis aplicações importantes dos comentários em código. Veja cada uma delas:

![[Pasted image 20240527171157.png]]

Aqui, reforçaremos a importância do comentário como ferramenta de documentação. Além dessas seis aplicações, comentários também podem ser utilizados para a geração automatizada de documentação. A grande vantagem dessa abordagem é a garantia de que a documentação do sistema estará sempre atualizada em relação ao que está escrito no código, como você pode ver na imagem a seguir. Observe que, em Python, há duas formas de se escreverem comentários:

![[STB07 3.png]]

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/01 1.png]]
1. SQLAlchemy -> https://www.sqlalchemy.org/

Assim como existem estilos convencionados que definem boas práticas para a codificação, também há convenções para a definição de comentários e documentação.

Em Python, o estilo mais comum para codificação é definido pelo [PEP 8](https://peps.python.org/pep-0008/), que tem, entre seus autores, Guido van Rossum. Para o uso de comentários para propósito de documentação, existe o [PEP 257.](https://peps.python.org/pep-0257/)

Vamos examinar alguns exemplos de códigos em HTML e JavaScript:

![[STB08 3.png]]

No tópico a seguir, vamos juntar a documentação de código com a documentação de sistema.

### Documentação de API

No caso das APIs, a expectativa é o retorno de uma informação estruturada como resposta para toda e qualquer requisição, incluindo requisições que podem levar a erro. Lembre-se do papel das mensagens autodescritivas e do uso do _status code_.  
  
Mas como saber quais são os recursos disponibilizados por uma API? Quais são as rotas possíveis? Qual é a estrutura da resposta? Como uma aplicação cliente pode interpretar a resposta da API?

Como uma API é uma aplicação _web_, espera-se que siga todas as restrições e limitações de arquitetura discutidas na primeira aula. Retornando ao tema padrão MVC, a visualização é a parte do sistema que sabe manipular modelos para gerar visualizações coerentes com aquilo que foi definido pelo controlador.

Cabe também à visualização receber os _inputs_ do usuário. No contexto da API, a visualização tem foco no sistema que irá se comunicar com a API. Em um sistema de comunicação entre máquinas, a visualização pode parecer de pouca relevância, mas é fundamental para quem programa do lado cliente.  

No caso das APIs, a documentação tem como objetivo entregar para o cliente (quem irá desenvolver o sistema que consome da API) conhecimento suficiente e atualizado sobre como consumir os recursos disponibilizados pela API.

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/01 2.png]]

1. API fornecida pelo Twitter -> https://developer.x.com/en/docs/api-reference-index
2. Documentação -> https://developer.x.com/en/docs/twitter-api/tweets/filtered-stream/api-reference/get-tweets-search-stream

#### OpenAPI

Quando o assunto são APIs, há muitos estilos e boas práticas de programação. Para APIs desenvolvidas em Python, alguns padrões de estilos mais comuns são: Swagger, ReDoc e RapiDoc. São vários, mas o importante é ter um.

A [OpenAPI](https://www.openapis.org/) é uma especificação que define um padrão para a construção de interfaces de descrição de APIs HTTP. Seu objetivo é definir um padrão de visualização de documentação que possa ser compreendido por pessoas e computadores, permitindo que homem e máquina entendam os serviços disponibilizados pela API sem precisarem acessar o código-fonte desta.

As especificações da OpenAPI são definidas pela Iniciativa OpenAPI, que é parte da [Linux Foundation Collaborative Project.](https://www.linuxfoundation.org/projects)

Criar esse tipo de documentação é fácil, quando se utilizam as ferramentas corretas. No caso, vale destacar a biblioteca [Python Flask-OpenAPI3](https://luolingchun.github.io/flask-openapi3/). Essa biblioteca é um _framework_ baseado no Flask, e utiliza uma biblioteca Python específica para verificação de dados e geração automatizada de documentação, a [Pydantic](https://pydantic-docs.helpmanual.io/). A Flask-OpenAPI3 é uma das opções de _frameworks_ disponíveis para esse tipo de atividade. Uma outra opção de _framework_ é a [FastAPI](https://fastapi.tiangolo.com/). Vamos verificar o Flask-OpenAPI3 e entender como é possível gerar a documentação de uma mesma API para três padrões diferentes:

![[Pasted image 20240527173803.png]]

![[Pasted image 20240527173838.png]]

![[Pasted image 20240527173852.png]]

### Publicação de uma aplicação e próximos passos

A publicação, ou _deploy_, é um processo em que, no final, a aplicação é disponibilizada para o cliente. Geralmente, contém muitas etapas. No entanto, vamos ver uma versão simplificada desse processo, com apenas quatro etapas.

Para exemplificar uma aplicação que lida com dados financeiros, foram inseridas etapas extras para verificação automatizada de vulnerabilidade de código e de segurança. Observe cada etapa detalhadamente:

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02 1 1.png]]

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/03 2.png]]

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/04 2.png]]

![[05 3.png]]

Não entregamos a aplicação recém desenvolvida diretamente para o cliente. Para chegar até o cliente é esperado que a aplicação tenha sido pelo menos testada e homologada. Com isso, antes de ser entregue ao cliente, ou seja, posto em um ambiente de produção (PRD), a aplicação tem que ser antes testada em outros dois ambientes: teste (TST) e homologação (HMG).

![[pos-graduacao/1º Acervo de imagens (Disc. 3)/02 2 1.png]]

![[pos-graduacao/Acervo de Imagens/03 5.png]]

![[04 4.png]]

Essa prática é comum em todo e qualquer projeto de aplicação _Web_. A proposta é que, a cada nova funcionalidade ou atualização do _software_, uma nova versão da aplicação seja definida e passe por todo esse processo até a entrega ao cliente final.

### Referências:

BIEHL, M. **REST API design rulebook**: designing consistent RESTful web service interfaces. California. Reilly Media, 2011.  
  
FOWLER, M. **Refatoração**: aperfeiçoando o _design_ de códigos existentes. 2. ed. São Paulo: Novatec, 2020.  
  
MARTIN, R. C. **Código limpo**: habilidades práticas do Agile Software. Rio de Janeiro: Alta Books, 2009.  
  
Martin, Robert C. **_Clean Code. A Handbook of Agile Software Craftsmanship_**, Illustrated Edition, Pearson Education, Massachusetts, 2008.  
  
PYTHON DEV TEAM; ROSSUM, G. V. **Python 3.6 language reference**. Colorado. Samurai Media Limited, 2016.