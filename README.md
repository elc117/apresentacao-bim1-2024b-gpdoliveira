# Listas
- Estrutura de dados que representa uma **coleção** de objetos em sequências
- Como visto em outras cadeiras, as listas são encadeadas e seus elementos são chamados de nós
- Algumas operações básicas em listas são inserção e remoção

# Listas em Haskell
- Em Haskell, as listas são estruturas de dados **homogêneos**
- Isto é, podemos ter uma lista de inteiros ou uma lista de caracteres, porém, é impossível criar uma lista com inteiros e caracteres
- Listas em Haskell podem **conter** outras listas. Estas listas também podem conter outras listas, todavia, uma lista não pode conter listas de tipos diferentes
- **Strings** são listas de caracteres -> "hello" é apenas outra forma de escrever ['h','e','l','l','o'] 
- Com isso em mente, qualquer operação realizada em listas serve para strings também
- Em Haskell, listas podem ser **infinitas**, contanto que você não utilize toda a lista
- Criação de uma lista
  
    `lista1 = [1,2,3,4,5]`
  
    `lista_infinita = [2,4..]`
  
- A seguir, veremos algumas operações com listas em Haskell:
  - **++** -> permite juntar duas listas

     `"olá" ++ " " ++ "mundo"`
    
    `"Olá mundo"`
  - **!!** -> utilizado para obter um item de uma lista através de seu índice, lembrando que ele começa em 0

    `"Steve Buscemi"!! 6`

    `'B'`
  - **< , <= , > e >=** -> utilizadas para realizar comparações entre listas, desde que sejam de tipos comparáveis
 
    `[3,2,1] > [2,1,0]`
    
    `Verdadeiro`

- Além disso, existem algumas funções que podem ser utilizadas com listas em Haskell
  - *head* pega uma lista e retorna seu head
  - *tail* pega uma lista e retorna sua cauda
  - *last* pega uma lista e retorna seu último elemento
  - *init* pega uma lista e retorna tudo, exceto seu último elemento
  - *length* pega uma lista e retorna seu comprimento
  - *null* verifica se uma lista está vazia
  - *reverse* inverte uma lista.
  - *take* pega número e uma lista. Ele extrai essa quantidade de elementos do começo da lista
  - *drop* remove o número de elementos do início de uma lista.
  - *maximum* pega uma lista de coisas que podem ser colocadas em algum tipo de ordem e retorna o maior elemento.
  - *sum* pega uma lista de números e retorna sua soma
  - *produto* pega uma lista de números e retorna seu produto.

  ![image](https://github.com/user-attachments/assets/9bedcc75-d748-4cff-834c-da4cc7aec38e)

- **Compreensões de lista** permitem aplicar funções matemáticas à criação de uma lista:
  
  `[x*2 | x <- [1..10], x*2 >= 12]`

    `[12,14,16,18,20]`
  
  O acima exemplo cria uma lista dos números de 1 a 10 multiplicados por 2 que são maiores que 12
- Ao lidar com listas em Haskell devemos considerar uma característica da linguagem: **sua avaliação preguiçosa**
- Isto quer dizer que o Haskell irá **postergar** a execução de qualquer cálculo até que ele seja necessário!

# Listas em outras linguagens de programação
- **C**: uso de structs, listas heterogêneas, listas simplesmente encadeadas, listas duplamente encadeadas, filas, pilhas
- **Python**: listas, dicionárias, funções básicas como append, remove, insert
