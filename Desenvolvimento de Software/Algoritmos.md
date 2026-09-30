
# Algoritmos de Busca

## Big O:

A **notação O-grande**, ou **Big O notation**, é uma ferramenta matemática utilizada na análise de algoritmos para descrever o comportamento de tempo de execução ou consumo de espaço em relação ao tamanho da entrada. Essa notação fornece uma forma de classificar algoritmos com base em sua complexidade assintótica, que se refere ao seu desempenho à medida que o tamanho da entrada tende ao infinito.

### Principais Características da Notação O-grande

1. **Descreve a Complexidade Assintótica:**
    
    - A notação O-grande expressa o limite superior do tempo de execução ou do espaço necessário por um algoritmo, considerando o pior caso. Ou seja, fornece um teto para o crescimento do tempo ou espaço à medida que a entrada aumenta.
2. **Foca em Comportamentos Assintóticos:**
    
    - A análise na notação O-grande se concentra nos termos mais significativos do algoritmo, ignorando constantes e termos de ordem inferior. Isso é porque, em entradas grandes, os termos dominantes são os que mais impactam o desempenho.
3. **Simplicidade e Clareza:**
    
    - Usar a notação O-grande permite que desenvolvedores e cientistas da computação comuniquem a eficiência dos algoritmos de forma clara e concisa, independentemente da implementação específica ou do hardware.

### Como a Notação O-grande é Utilizada

- A notação O-grande é frequentemente usada para descrever o tempo de execução e o espaço necessário por um algoritmo. Aqui estão alguns exemplos comuns:
    
    - **O(1):** Tempo constante. O tempo de execução não depende do tamanho da entrada.
    - **O(log N):** Tempo logarítmico. Cresce lentamente à medida que a entrada aumenta.
    - **O(N):** Tempo linear. O tempo de execução aumenta proporcionalmente ao tamanho da entrada.
    - **O(N log N):** Tempo linear logarítmico. Comum em algoritmos de ordenação eficientes, como mergesort e heapsort.
    - **O(N²):** Tempo quadrático. O tempo de execução aumenta com o quadrado do tamanho da entrada. Comum em algoritmos de ordenação simples, como bubble sort e selection sort.
    - **O(2^N):** Tempo exponencial. O tempo de execução dobra com cada incremento no tamanho da entrada. Comum em algoritmos que resolvem problemas complexos, como o problema da mochila ou a Torre de Hanoi.
    - **O(N!):** Tempo fatorial. Cresce muito rapidamente e é comum em problemas de permutação.

### Exemplo Prático

Considere um algoritmo que percorre todos os elementos de uma lista para encontrar um elemento específico:

def busca_linear(lista, alvo):
    for elemento in lista:
        if elemento == alvo:
            return True
    return False

- **Análise:**
    - No pior caso, o algoritmo terá que percorrer todos os elementos da lista. Se a lista tem NNN elementos, a complexidade de tempo deste algoritmo é O(N)O(N)O(N).

### Conclusão

A notação O-grande é uma ferramenta crucial para a análise de algoritmos, permitindo que programadores e analistas comparem eficientemente a eficiência de diferentes abordagens para resolver um problema. Ao usar a notação O-grande, podemos entender melhor como um algoritmo se comportará à medida que o tamanho da entrada cresce, ajudando a tomar decisões informadas sobre a escolha do algoritmo mais adequado para uma determinada tarefa.

## Algoritmos de Ordenação:

### Análise dos Algoritmos

Características dos algoritmos de ordenação:

1. **Quicksort:**
    - **Pior Caso:** O(N2)O(N^2)O(N2) (ocorre em situações desfavoráveis, como quando o menor ou maior elemento é sempre escolhido como pivô).
    - **Caso Médio:** O(Nlog⁡N)O(N \log N)O(NlogN).
    
1. **Selection Sort:**
    - **Pior Caso:** O(N2)O(N^2)O(N2).
    - **Caso Médio:** O(N2)O(N^2)O(N2).
    - O Selection Sort não apresenta complexidade O(Nlog⁡N)O(N \log N)O(NlogN) no caso médio.
    
1. **Insertion Sort:**
        - **Pior Caso:** O(N2)O(N^2)O(N2).
    - **Caso Médio:** O(N2)O(N^2)O(N2).
    - Semelhante ao Selection Sort, o Insertion Sort não apresenta complexidade O(Nlog⁡N)O(N \log N)O(NlogN) no caso médio.
    
4. **Merge Sort:**
    - **Pior Caso:** O(Nlog⁡N)O(N \log N)O(NlogN).
    - **Caso Médio:** O(Nlog⁡N)O(N \log N)O(NlogN).
    - Não é o escolhido, pois não atende à condição do pior caso ser O(N2)O(N^2)O(N2).
    
1. **Heap Sort:**
    - **Pior Caso:** O(Nlog⁡N)O(N \log N)O(NlogN).
    - **Caso Médio:** O(Nlog⁡N)O(N \log N)O(NlogN).
    - Também não atende à condição do pior caso ser O(N2)O(N^2)O(N2).


| Algoritmo      | Melhor caso | Caso Médio | Pior Caso |
| -------------- | ----------- | ---------- | --------- |
| Bubble Sort    | O(N)        | O(N^2)     | O(N^2)    |
| Selection Sort | O(N^2)      | O(N^2)     | O(N^2)    |
| Insertion Sort | O(N)        | O(N^2)     | O(N^2)    |
| Merge Sort     | O(N logN)   | O(N logN)  | O(N logN) |
| Quick Sort     | O(N logN)   | O(N logN)  | O(N^2)    |
| Heap Sort      | O(N logN)   | O(N logN)  | O(N logN) |


### 1. **Selection Sort**

#### Definição:

O **Selection Sort** é um algoritmo de ordenação simples que funciona selecionando repetidamente o menor (ou maior) elemento de uma lista e trocando-o com o primeiro elemento não ordenado.

#### Funcionamento:

- Para cada posição do vetor, encontra o menor elemento na parte não ordenada e o coloca na posição correta.
- Não usa a ideia de inserção; em vez disso, realiza trocas de valores.

#### Pseudocódigo básico:

Para i de 1 até n-1 faça:
    MinIndex <- i
    Para j de i+1 até n faça:
        Se V[j] < V[MinIndex] então:
            MinIndex <- j
    Troca V[i] e V[MinIndex]
Fim Para

#### Identificação:

- Procura o menor (ou maior) elemento a cada iteração e o coloca na posição correta com uma troca.
- Sempre faz trocas, mesmo que o elemento já esteja na posição correta.
- É relativamente fácil de identificar porque faz **uma troca por iteração externa**.

### 2. **Insertion Sort**

#### Definição:

O **Insertion Sort** é um algoritmo de ordenação que constrói a lista ordenada um elemento de cada vez, inserindo cada novo elemento em sua posição correta em relação aos elementos já ordenados.

#### Funcionamento:

- Percorre o vetor da esquerda para a direita, inserindo o elemento atual na posição correta em relação aos elementos anteriores, movendo elementos maiores para a direita.

#### Pseudocódigo básico:

Para i de 2 até n faça:
    X <- V[i]
    j <- i-1
    Enquanto j > 0 e V[j] > X faça:
        V[j+1] <- V[j]
        j <- j-1
    V[j+1] <- X
Fim Para

#### Identificação:

- Muda elementos ao longo de um vetor já parcialmente ordenado, movendo os valores maiores para a direita para abrir espaço para o novo valor.
- Característico pela movimentação de múltiplos elementos e inserção na posição correta.

### 3. **Bubble Sort**

#### Definição:

O **Bubble Sort** é um algoritmo de ordenação simples que percorre a lista várias vezes, trocando os elementos adjacentes se estiverem na ordem errada, "borbulhando" os maiores valores para o final da lista.

#### Funcionamento:

- A cada passagem pelo vetor, compara pares adjacentes e troca-os se estiverem fora de ordem.
- O maior elemento "flutua" para o final em cada iteração.

#### Pseudocódigo básico:

Para i de 1 até n-1 faça:
    Para j de 1 até n-i faça:
        Se V[j] > V[j+1] então:
            Troca V[j] e V[j+1]
Fim Para

#### Identificação:

- Realiza muitas trocas adjacentes.
- O maior valor "borbulha" para o final a cada iteração.
- O vetor é percorrido múltiplas vezes, e muitos pares de elementos são comparados e trocados.

---

### 4. **Merge Sort**

#### Definição:

O **Merge Sort** é um algoritmo de ordenação baseado na técnica de **divisão e conquista**, que divide recursivamente o vetor em duas metades, ordena cada metade e, em seguida, mescla as metades ordenadas.

#### Funcionamento:

- Divide o vetor em duas metades até restarem subvetores com apenas um elemento.
- Em seguida, junta (mescla) os subvetores de maneira ordenada.

#### Pseudocódigo básico:

Se n > 1 então:
    Divide o vetor V em duas metades
    Merge Sort na primeira metade
    Merge Sort na segunda metade
    Mescla as duas metades de forma ordenada

#### Identificação:

- Divide o vetor ao meio recursivamente.
- A ordenação ocorre na fase de "mesclagem".
- Requer um espaço auxiliar para realizar as operações de mesclagem.

---

### 5. **Quick Sort**

#### Definição:

O **Quick Sort** é outro algoritmo baseado em **divisão e conquista**. Ele seleciona um **pivô**, particiona os elementos em relação a esse pivô (elementos menores à esquerda, maiores à direita) e, recursivamente, aplica o mesmo processo nas duas partes.

#### Funcionamento:

- Escolhe um pivô e rearranja o vetor de modo que todos os elementos menores que o pivô fiquem à esquerda e os maiores fiquem à direita.
- Recursivamente aplica o mesmo processo às duas partes.

#### Pseudocódigo básico:

Se o vetor tem mais de um elemento então:
    Escolha um pivô
    Particione o vetor em dois subvetores:
        - Elementos menores que o pivô
        - Elementos maiores que o pivô
    Quick Sort nos subvetores


#### Identificação:

- Sempre envolve a escolha de um pivô e a divisão do vetor com base no pivô.
- Normalmente, é identificado pela "partição" de um vetor em duas partes, sem precisar de espaço auxiliar como o Merge Sort.

### Como identificar cada algoritmo?

Aqui estão algumas dicas rápidas para identificar esses algoritmos observando seu comportamento ou pseudocódigo:

1. **Selection Sort**:
    - Procura o menor (ou maior) elemento e faz uma única troca por iteração.
    - Usa dois laços, um para cada posição e outro para encontrar o menor valor.
    - Divide a lista em uma parte ordenada e outra desordenada, e em cada iteração, seleciona o menor (ou maior) elemento da parte desordenada e o insere na parte ordenada.
    
1. **Insertion Sort**:
    - Insere cada elemento na sua posição correta no vetor já parcialmente ordenado.
    - Move elementos maiores para abrir espaço e insere o valor.
    - Estável porque, ao inserir um novo elemento na parte já ordenada, ele o faz sem alterar a ordem dos elementos iguais.

1. **Bubble Sort**:    
    - Troca elementos adjacentes se estiverem fora de ordem.
    - O maior valor "borbulha" para o final em cada iteração.
    - Muitas comparações e trocas de pares.
    - Compara pares adjacentes de elementos e troca-os se estiverem na ordem errada. Ele percorre a lista várias vezes até que não haja mais trocas a serem feitas.

1. **Merge Sort**:    
    - Divide o vetor em duas partes recursivamente.
    - O vetor é mesclado após ser dividido completamente.
    - Usa a abordagem de divisão e conquista.

1. **Quick Sort**:    
    - Escolhe um pivô e particiona o vetor em relação a esse pivô.
    - Recursivamente ordena as duas metades em torno do pivô.
    - Outro algoritmo de divisão e conquista, mas diferente do Merge Sort, pois trabalha "in-place" e faz a partição baseada no pivô.


## Padrão de Desenvolvimento

- **Chain of Responsibility:**
    - Este padrão permite que um objeto tenha mais de um manipulador para uma solicitação. O manipulador pode decidir processar a solicitação ou passar a solicitação para o próximo manipulador na cadeia. É muito útil quando você não sabe qual objeto deve lidar com uma solicitação, permitindo que você defina uma cadeia de objetos que podem processar a solicitação.
    - **Exemplo:** Imagine uma fila de processos para tratar um documento:
		1. Validação de dados
		2. Geração de relatórios
		3. Armazenamento em banco de dados
		Se a validação falhar, o documento não avança para o próximo processo.
		
- **Prototype:**
    - O padrão Prototype permite a criação de objetos clonando um protótipo existente em vez de criar novas instâncias a partir do zero. É útil quando o custo de criação de um objeto é maior do que o de clonar um objeto existente.
    - **Exemplo:** Criar cópias de um documento já existente para edição, em vez de criar um novo do zero.
    - 
- **Decorator:**
    - O padrão Decorator permite adicionar funcionalidade a um objeto dinamicamente, sem alterar a estrutura do objeto. Isso é feito através da criação de classes que "decoram" o objeto original, adicionando comportamentos adicionais.
    - **Exemplo:** Adicionar recursos de formatação a um documento (como realce de texto) sem alterar a classe base do documento.
    - 
- **Abstract Factory:**
    - O padrão Abstract Factory fornece uma interface para criar famílias de objetos relacionados ou dependentes, sem especificar suas classes concretas. Ele permite que você crie produtos sem saber suas classes concretas.
    - **Exemplo:** Criar um sistema que pode gerar diferentes tipos de documentos (PDF, Word, Excel) a partir de uma única interface.
    - 
- **Factory Method:**
    - O padrão Factory Method define uma interface para criar um objeto, mas permite que subclasses alterem o tipo de objeto que será criado. Ele encapsula a criação de objetos e permite a substituição da classe do objeto instanciado.
    - **Exemplo:** Um método que cria instâncias de diferentes tipos de documentos com base em parâmetros fornecidos (por exemplo, "documento financeiro" ou "documento legal").

### Resumo
- **Chain of Responsibility:** Encadeamento de manipuladores que podem processar uma solicitação.
- **Prototype:** Clonagem de objetos existentes.
- **Decorator:** Adição dinâmica de responsabilidades a objetos.
- **Abstract Factory:** Criação de famílias de produtos relacionados.
- **Factory Method:** Definição de uma interface para criação de objetos, permitindo que subclasses decidam a classe a ser instanciada.

