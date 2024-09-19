# Listas
- Estrutura de dados que representa uma coleção de objetos em sequências
- Como visto em outras cadeiras, as listas são encadeadas e seus elementos são chamados de nós
- Algumas operações básicas em listas são inserção e remoção

Listas em Haskell
- Em Haskell, as listas são estruturas de dados homogêneos
- Isto é, podemos ter uma lista de inteiros ou uma lista de caracteres, porém, é impossível criar uma lista com inteiros e caracteres
- Listas em Haskell podem conter outras listas. Estas listas também podem conter outras listas, todavia, uma lista não pode conter listas de tipos diferentes
- Strings são listas de caracteres -> "hello" é apenas outra forma de escrever ['h','e','l','l','o'] 
- Com isso em mente, qualquer operação realizada em listas serve para strings também
- Em Haskell, as listas podem ser infinitas, contanto que você não utilize toda a lista
- Criação de uma lista
  
    `lista1 = [1,2,3,4,5]`
  
    `lista_infinita = [2,4..]`
  
- A seguir, veremos algumas operações com listas em Haskell:
  - ++ -> permite juntar duas listas
    `"olá" ++ " " ++ "mundo"
    "Olá mundo"`
  - !! -> utilizado para obter um item de uma lista através de seu índice, lembrando que ele começa em 0
