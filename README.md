Minha experiência com ponteiros, vetores, matrizes e structs em C

Sendo bem sincero, no começo eu achei essa parte de C bem confusa, principalmente ponteiros e alocação dinâmica. Parece muita coisa ao mesmo tempo e fica difícil entender só na teoria.

Mas depois que comecei a fazer os exercícios, fui entendendo melhor como funciona na prática.

Ponteiros

Primeiro tentei entender o básico: o que é um ponteiro.

Pelo que eu entendi, ele guarda o endereço de uma variável. Quando fiz p = &x, foi como se o ponteiro passasse a “saber” onde a variável está na memória.

Depois, usando *p, percebi que conseguia acessar o valor dessa variável de forma indireta. Isso foi importante para começar a entender o resto.

Alterando valores com ponteiro

Aqui ficou mais claro o uso prático.

Consegui alterar o valor de uma variável sem acessar ela diretamente, apenas usando o ponteiro, por exemplo com *p = 20.

Isso ajudou a entender como funções conseguem modificar valores fora do seu próprio escopo.

Funções com ponteiros

Nas funções de soma e troca, usei ponteiros como parâmetros.

Na soma, apenas peguei os valores apontados e armazenei o resultado em outro endereço.

Na troca, utilizei uma variável auxiliar para não perder valores durante o processo.

Foi mais questão de cuidado com a lógica do que algo muito complicado.

Vetores com ponteiros

Aqui percebi melhor a relação entre vetores e ponteiros.

Usei expressões como *(v + i) para acessar os elementos, que funciona da mesma forma que v[i].

Isso ajudou a visualizar melhor como os dados ficam organizados na memória.

Soma e maior elemento

Esses foram mais diretos.

Para somar, fui acumulando os valores em uma variável.

Para encontrar o maior elemento, comecei assumindo que o primeiro era o maior e fui comparando com os outros.

Inversão de vetor

Essa parte foi interessante.

Usei dois ponteiros: um no início e outro no final do vetor. Fui trocando os valores entre eles até se encontrarem.

Assim consegui inverter o vetor sem precisar criar outro.

Ponteiro para ponteiro

Aqui foi mais conceitual.

Criei um ponteiro que aponta para outro ponteiro, que por sua vez aponta para uma variável.

No final, usando **pp, consegui acessar o mesmo valor. Serviu mais para entender níveis de indireção.

Alocação dinâmica

Essa foi uma das partes mais importantes.

Usei malloc para criar estruturas de tamanho definido pelo usuário.

Também entendi a importância de usar free depois, para liberar a memória e evitar problemas.

Vetores dinâmicos

Fiz um vetor com tamanho definido pelo usuário, li os valores e depois imprimi em ordem inversa.

Foi uma forma simples de aplicar a alocação dinâmica.

Matrizes dinâmicas

No começo foi mais difícil.

Precisei entender que uma matriz dinâmica é feita alocando:

um vetor de ponteiros (linhas)
e depois cada linha separadamente (colunas)

Depois disso, consegui preencher e imprimir normalmente.

A transposta foi feita apenas invertendo os índices na impressão.

Matriz com números aleatórios

Aqui usei a mesma lógica da matriz, mas preenchendo com rand().

Usei também srand(time(NULL)) para evitar repetir os mesmos valores a cada execução.

Nomes e idades

Nesse exercício precisei trabalhar com strings.

Usei fgets para ler nomes completos, já que podem ter espaços.

Também tive que usar getchar() para limpar o buffer após o scanf, evitando erros na leitura.

Structs

O uso de struct ajudou a organizar melhor os dados.

Em vez de várias variáveis separadas, consegui agrupar tudo em uma única estrutura, como nome, idade e outros dados.

Também utilizei funções para manipular essas estruturas, sempre passando ponteiros.

Maior e menor com struct

A lógica foi semelhante à de vetores.

Percorri todos os elementos e fui comparando até encontrar o maior e o menor.

Sistema de turmas

Esse foi o exercício mais completo.

Trabalhei com turmas que possuem:

identificador
número de vagas
alunos

Usei ponteiros e valores NULL para controlar as posições disponíveis.

Implementei funções para:

criar turma
matricular aluno
lançar notas
calcular média
listar alunos

Esse exercício ajudou bastante a juntar todos os conceitos estudados.

Matriz 5x5 com índices

Esse foi mais simples.

Utilizei a expressão:

i * 5 + j

para preencher a matriz com valores organizados.

Conclusão

No início os conteúdos pareceram difíceis, mas com a prática foi ficando mais claro.

Principalmente em relação a:

ponteiros
alocação dinâmica
uso de structs

A prática foi essencial para entender melhor esses conceitos.

Final

Sei que ainda tenho muito a melhorar e estudar, principalmente em relação a ponteiros e alocação dinâmica, que exigem bastante prática. Mesmo assim, venho tentando evoluir no dia a dia, praticando e revisando os conteúdos para aprender cada vez mais e com mais segurança.

Todo esse aprendizado foi baseado nas aulas do professor Reudismam, além do apoio das explicações da professora Cibely, que contribuíram bastante para o meu entendimento ao longo dos exercícios.

