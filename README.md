# Desafio Bootcamping Inter Java Develops
> Projeto baseado nos desafios propostos pelo Bootcamping Inter Java Develops.
<a name="ancora"></a>

|       Desafio                  |            Tema do Desafio                   |  Nível do Desafio |                   Respostas                     |
|--------------------------------|----------------------------------------------|-------------------|-------------------------------------------------|
|      [Desafio 1](#ancora1)     |    Solucionando problemas básicos em Java    |      Básico       |      [Resolução](src/desafios/Desafio1.java)    |   
|      [Desafio 2](#ancora2)     |    Solucionando problemas básicos em Java    |      Básico       |      [Resolução](src/desafios/Desafio2.java)    |   
|      [Desafio 3](#ancora3)     |    Solucionando problemas básicos em Java    |      Básico       |      [Resolução](src/desafios/Desafio3.java)    |   
|      [Desafio 4](#ancora4)     |        Praticando programação em Java        |   Intermediário   |      [Resolução](src/desafios/Desafio4.java)    |   
|      [Desafio 5](#ancora5)     |        Praticando programação em Java        |   Intermediário   |      [Resolução](src/desafios/Desafio5.java)    |   
|      [Desafio 6](#ancora6)     |        Praticando programação em Java        |   Intermediário   |      [Resolução](src/desafios/Desafio6.java)    |   
|      [Desafio 7](#ancora7)     |        Praticando programação em Java        |   Intermediário   |      [Resolução](src/desafios/Desafio7.java)    |   
|      [Desafio 8](#ancora8)     |        Praticando programação em Java        |   Intermediário   |      [Resolução](src/desafios/Desafio8.java)    |   
|      [Desafio 9](#ancora9)     |         Desafios Aritméticos em Java         |     Avançado      |      [Resolução](src/desafios/Desafio9.java)    |   
|      [Desafio 10](#ancora10)   |         Desafios Aritméticos em Java         |     Avançado      |      [Resolução](src/desafios/Desafio10.java)   |   
|      [Desafio 11](#ancora11)   |         Desafios Aritméticos em Java         |     Avançado      |      [Resolução](src/desafios/Desafio11.java)   |   
 
  
# <a id="ancora1"></a>[Desafio 1](#ancora)
Você receberá dois valores inteiros. Faça a leitura e em seguida calcule o produto entre estes dois valores. Atribua esta operação à variável PROD, mostrando esta de acordo com a mensagem de saída esperada (exemplo abaixo). 

## Entrada
A entrada contém 2 valores inteiros.

## Saída
Exiba a variável PROD conforme exemplo abaixo, tendo obrigatoriamente um espaço em branco antes e depois da igualdade.

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           3           |      PROD = 27      |    
|           9           |                     |  

# <a id="ancora2"></a>[Desafio 2](#ancora)
Desenvolva um código que leia um valor E. Este E será o tamanho de um vetor X[E]. A seguir, leia cada um dos valores de X, encontre o menor elemento deste vetor e a sua posição dentro do vetor, mostrando esta informação.

## Entrada
A primeira linha de entrada contem um único inteiro E (1 < E < 1000), indicando o número de elementos que deverão ser lidos em seguida para o vetor X[E] de inteiros. A segunda linha contém cada um dos E valores, separados por um espaço.

## Saída
A primeira linha apresenta a mensagem “Menor valor:” seguida de um espaço e do menor valor lido na entrada. A segunda linha apresenta a mensagem “Posicao:” seguido de um espaço e da posição do vetor na qual se encontra o menor valor lido, lembrando que o vetor inicia na posição zero.

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           10          | Menor Valor:-5      |    
| 1 2 3 4 -5 6 7 8 9 10 | Posição:4           |


# <a id="ancora3"></a>[Desafio 3](#ancora3)
Leia um valor inteiro X (1 <= X <= 1000). Em seguida mostre os ímpares de 1 até X, um valor por linha, inclusive o X, se for o caso.

## Entrada
O arquivo de entrada contém 1 valor inteiro qualquer.

## Saída
Imprima todos os valores ímpares de 1 até X, inclusive X, se for o caso.

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           8           |          1          |    
|                       |          3          |
|                       |          5          |
|                       |          7          |

# <a id="ancora4"></a>[Desafio 4](#ancora)
Leonardo é um nômade digital e viaja pelo mundo programando em diferentes cafés das cidades por onde passa. Recentemente, resolveu criar um blog, para compartilhar suas experiências e aprendizados com seus amigos.

Para criação do blog, ele optou por utilizar uma ferramenta pronta, que há um limite de caracteres que se pode escrever por dia, e Leonardo está preocupado que essa limitação, afinal, irá impedir de contar suas melhores experiências. Para contornar esse problema, decidiu usar um sistema de abreviação de palavras em seus posts.

O sistema de abreviações é simples e funciona da seguinte forma: para cada letra, é possível escolher uma palavra que inicia com tal letra e que aparece no post. Uma vez escolhida a palavra, sempre que ela aparecer no post, ela será substituída por sua letra inicial e um ponto, diminuindo assim o número de caracteres impressos na tela.

Por exemplo, na frase: “hoje eu programei em Python”, podemos escolher a palavra “programei” para representar a letra ‘p', e a frase ficará assim: “hoje eu p. em Python”, economizando assim sete caracteres. Uma mesma palavra pode aparecer mais de uma vez no texto, e será abreviada todas as vezes. Note que, se após uma abreviação o número de caracteres não diminuir, ela não deve ser usada, tal como no caso da palavra “eu” acima.

## Entrada
Haverá diversos casos de teste. Cada caso de teste é composto de uma linha, contendo uma frase de até 10⁴ caracteres. A frase é composta de palavras e espaços em branco, e cada palavra é composta de letras minúsculas ('a'-'z'), e contém entre 1 e 30 caracteres cada.

O último caso de teste é indicado quando a linha dada conter apenas um “.”, o qual não deverá ser processado.

## Saída
Para cada caso de teste, imprima uma linha contendo a frase já com as abreviações escolhidas e aplicadas.

Em seguida, imprima um inteiro N, indicando o número de palavras em que foram escolhidas uma letra para a abreviação no texto. Nas próximas N linhas, imprima o seguinte padrão “C. = P”, onde C é a letra inicial e P é a palavra escolhida para tal letra. As linhas devem ser impressas em ordem crescente da letra inicial.

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|   abcdef abc abc abc  |   a. abc abc abc    |    
|                       |          1          |
|                       |   a. = abcdef       |

# <a id="ancora5"></a>[Desafio 5](#ancora)
Nesse algoritmo você deverá descobrir se um conjunto de palavras é bom ou ruim. Por definição, um conjunto é bom quando nenhuma palavra desse conjunto é um prefixo de outra palavra. Caso contrário, é considerado um conjunto ruim.

Por exemplo, {dbc, dae, dbcde} é um conjunto ruim, pois dbc é um prefixo de dbcde. Quando duas palavras são idênticas, definimos como uma sendo prefixo da outra.

## Entrada
A entrada contém vários casos de teste. A primeira linha de cada caso de teste terá um inteiro N (1 ≤ N ≤ 10⁵), que representa a quantidade de palavras no conjunto. Segue então N linhas, cada uma tendo uma palavra de no máximo 100 letras minúsculas. A entrada termina quando N = 0 e não deve ser processada.

## Saída
Para cada caso de teste, você deverá imprimir "Conjunto Bom", ou "Conjunto Ruim", conforme explicado acima.

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           3           |    Conjunto Ruim    |    
|          abc          |    Conjunto Bom     |
|          dae          |                     |
|         abcde         |                     |
|           2           |                     |
|          abc          |                     |
|          def          |                     |
|           0           |                     |

# <a id="ancora6"></a>[Desafio 6](#ancora)
Encontre a maior substring comum entre as duas strings informadas. A substring pode ser qualquer parte da string, inclusive ela toda. Se não houver subseqüência comum, a saída deve ser “0”. A comparação é case sensitive ('x' != 'X').

## Entrada
A entrada contém vários casos de teste. Cada caso de teste é composto por duas linhas, cada uma contendo uma string. Ambas strings de entrada contém entre 1 e 50 caracteres ('A'-'Z','a'-'z' ou espaço ' '), inclusive, ou no mínimo uma letra ('A'-'Z','a'-'z').

## Saída
O tamanho da maior subsequência comum entre as duas Strings.

|   Exemplos de Entrada    |  Exemplos de Saída  |    
|--------------------------|---------------------|
|        abcdef            |          2          |    
|        cdofhij           |          1          |
|          TWO             |          0          |
|          FOUR            |          7          |
|      abracadabra         |                     |
|          open            |                     |
|  Hey This java is hot    |                     |
|  Java is a new paradigm  |                     |

# <a id="ancora7"></a>[Desafio 7](#ancora)
A nutricionista Juliana Alcantra é uma excelente profissional de sua área. Em determinado dia, ela foi entrevistada ao vivo para um jornal da cidade. No entanto, ficou um pouco nervosa na hora, e diante da situação, sua fala ficou um pouco distorcida, repetindo o final de cada palavra após dizer a mesma. Para que isso não aconteça novamente, ela precisa da sua ajuda para escrever um programa que omita a parte repetida, de modo que as palavras sejam pronunciadas como deveriam ser.

Escreva um programa que, dada uma palavra errada, a mesma seja corrigida.

## Entrada
Haverá diversos casos de teste. Cada caso de teste é formado por uma palavra, de, no máximo, 30 caracteres, dita da forma errada. A entrada termina com fim de arquivo.

## Saída
Para cada caso de teste, escreva a palavra devidamente corrigida. Analise os exemplos para verificar o padrão, de modo a consertar todos os casos.

|   Exemplos de Entrada    |  Exemplos de Saída  |    
|--------------------------|---------------------|
|      sanduicheiche       |      sanduiche      |    
|       barrilarril        |        barril       |
|         ratoato          |         rato        |
|          sol             |         sol         |
|        coliseueu         |       coliseu       |
|        queijoijo         |        queijo       |
|       astroastro         |        astro        |
|           a              |          a          |

# <a id="ancora8"></a>[Desafio 8](#ancora)
Pedro e Fernando são os desenvolvedores em uma stratup e vão desenvolver o novo sistema de cadastro, e pediram a sua ajuda. Sua task é fazer o código que valide as senhas que são cadastradas, para isso você deve atentar aos requisitos a seguir:

A senha deve conter, no mínimo, uma letra maiúscula, uma letra minúscula e um número;
A mesma não pode ter nenhum caractere de pontuação, acentuação ou espaço;
Além disso, a senha pode ter de 6 a 32 caracteres.

## Entrada
A entrada contém vários casos de teste e termina com final de arquivo. Cada linha tem uma string S, correspondente a senha que é inserida pelo usuário no momento do cadastro.

## Saída
A saída contém uma linha, que pode ser “Senha valida.”, caso a senha tenha cada item dos requisitos solicitados anteriormente, ou “Senha invalida.”, se um ou mais requisitos não forem atendidos.

|      Exemplos de Entrada      |  Exemplos de Saída  |    
|-------------------------------|---------------------|
|   Digital Innovation One      |   Senha invalida.   |    
|         AbcdEfgh99            |    Senha valida.    |
|   DigitalInnovationOne123     |    Senha valida.    |
|   Digital Innovation One 123  |   Senha invalida.   |
|           Aass9               |   Senha invalida.   |
|          Aassd9               |    Senha valida.    |

# <a id="ancora9"></a>[Desafio 9](#ancora)
Paula simplesmente adora matemática. Seu maior passatempo é ficar inventando jogos ou atividades que a envolvam para brincar com seus amiguinhos. Obviamente, nem todos eles não são tão apaixonados assim por matemática e têm muita dificuldade para resolver as brincadeiras propostas por ela. Agora Paula inventou um pequeno passatempo que envolve 3 caracteres: um dígito numérico, uma letra e outro dígito numérico.

Se a letra for maiúscula, deve-se subtrair o primeiro dígito do segundo. Se a letra for minúscula, deve-se somar ambos os dígitos e se os DÍGITOS forem iguais, deve-se desconsiderar a letra e mostrar o produto entre os dois dígitos. Ela pediu para seu amigo Marcelo, que é bom em programação, para criar um programa para que encontre a solução para cada uma das sequências que Paula lhe apresentar.

## Entrada
A entrada contém vários casos de teste. A primeira linha da entrada contém um inteiro N, indicando o número de casos de teste que virão a seguir. Cada caso de teste é uma sequência de três caracteres criada por Paula. Esta sequência contém na primeira posição um caractere de '0' a '9', na segunda posição uma letra maiúscula ou minúscula do alfabeto e na terceira posição outro caractere de '0' a '9'.

## Saída
Para cada caso de teste, deve ser impressa uma linha com um valor inteiro que representa a solução da sequência proposta por Paula.

|  Exemplos de Entrada   |  Exemplos de Saída  |    
|------------------------|---------------------|
|           5            |                     |    
|          4A5           |          1          |
|          3A3           |          9          |
|          4F2           |          6          |
|          2G4           |          2          |
|          7Z1           |          -6         |
# <a id="ancora10"></a>[Desafio 10](#ancora)
Neste problema você é solicitado a escrever um simples programa de conversão de base. A entrada será um valor hexadecimal ou decimal. Você deverá converter cada valor da entrada. Se o valor for hexadecimal, você deve convertê-lo para decimal e vice-versa. O valor hexadecimal inicia sempre com “0x” ou também, é aquele valor cuja segunda casa contém a letra 'x'.

## Entrada
A entrada contém vários casos de teste. Cada linha de entrada, com exceção da última, contém um número não-negativo, decimal ou hexa. O valor decimal será menor ou igual a 231. A última linha contém um número negativo que não deve ser processado, indicando o encerramento do programa.

## Saída
Para cada linha de entrada (exceto a última) deve ser produzido uma linha de saída. Todo número hexadecimal deve ser precedido na saída por '0x' (zero xis).

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           4           |         0x4         |    
|           7           |         0x7         |
|          44           |         0x2C        |
|       0x80685         |         525957      |
|         -1            |                     |
# <a id="ancora11"></a>[Desafio 11](#ancora)
Você tem em mãos dois cabos circulares de energia. O primeiro cabo tem raio R1 e o segundo raio R2. Você precisa comprar um conduite circular (veja a imagem abaixo que ilustra um conduite) de maneira a passar os dois cabos por dentro dele:

Qual o menor raio do conduite que você deve comprar? Em outras palavras, dado dois círculos, qual o raio do menor círculo que possa englobar ambos os dois?

## Entrada
Na primeira linha teremos um inteiro T (T ≤ 10000), indicando o número de casos de teste.

Na única linha de cada caso teremos dois números inteiros R1 e R2, indicando os respectivos raios. Os inteiros serão positivos e todas as contas caberão em um inteiro normal de 32 bits.

## Saída
Em cada caso, imprima o menor raio possível em uma única linha

|  Exemplos de Entrada  |  Exemplos de Saída  |    
|-----------------------|---------------------|
|           3           |                     |    
|          1 1          |         2           |
|          2 8          |         10          |
|          8 2          |         10          |
 

