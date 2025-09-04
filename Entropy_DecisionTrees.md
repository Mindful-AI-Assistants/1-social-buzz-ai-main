

<br>

## 🇺🇸 In the context of decision trees, entropy is a measure of the impurity or randomness of a set of data within a node.

<br>


### Think of it this way:

* Pure Nodes: If a node contains only samples from a single class (for example, all samples in that node result in "Compra" - Buy), that node is considered pure. The entropy for a pure node is zero.
* Impure Nodes: If a node contains a mix of samples from different classes (for example, some samples result in "Compra" and others in "Não Compra" - Don't Buy), that node is considered impure. The more mixed the classes are, the higher the entropy. Entropy is maximum when the classes are equally distributed (for example, 50% "Compra" and 50% "Não Compra").

<br>

### Why is entropy important in decision trees?

Decision tree building algorithms (like the one used in your code, with criterion="entropy") aim to split the data at each node in a way that reduces entropy as much as possible in the child nodes. The goal is to create child nodes that are purer than the parent node, meaning they contain samples that predominantly belong to a single class.
By reducing entropy at each split, the tree is essentially learning to separate the classes effectively. The algorithm chooses the variable and the split point that result in the greatest "information gain," which is the reduction in entropy after the split.
In summary, entropy is a mathematical tool used to quantify how "mixed" the classes are in a node, and the decision tree algorithm tries to minimize this mixture at each step to create branches that lead to clear predictions.


<br><br>

## 🇧🇷 No contexto de árvores de decisão, a entropia é uma medida da impureza ou aleatoriedade de um conjunto de dados em um nó.

<br>


### Pense da seguinte forma:

* Nós Puros: Se um nó contiver apenas amostras de uma única classe (por exemplo, todas as amostras naquele nó resultam em "Compra"), esse nó é considerado puro. A entropia para um nó puro é zero.
* Nós Impuros: Se um nó contiver uma mistura de amostras de diferentes classes (por exemplo, algumas amostras resultam em "Compra" e outras em "Não Compra"), esse nó é considerado impuro. Quanto mais misturadas as classes, maior a entropia. A entropia é máxima quando as classes estão distribuídas igualmente (por exemplo, 50% "Compra" e 50% "Não Compra").

<br>

### Por que a entropia é importante nas árvores de decisão?

Os algoritmos de construção de árvores de decisão (como o usado no seu código, com criterion="entropy") buscam dividir os dados em cada nó de forma a reduzir a entropia o máximo possível nos nós filhos. O objetivo é criar nós filhos que sejam mais puros do que o nó pai, ou seja, que contenham amostras que pertençam predominantemente a uma única classe.
Ao reduzir a entropia em cada divisão, a árvore está essencialmente aprendendo a separar as classes de forma eficaz. O algoritmo escolhe a variável e o ponto de divisão que resultam na maior "ganho de informação", que é a redução na entropia após a divisão.
Em resumo, a entropia é uma ferramenta matemática usada para quantificar o quão "misturadas" estão as classes em um nó, e o algoritmo da árvore de decisão tenta minimizar essa mistura a cada passo para criar ramos que levem a previsões claras.


