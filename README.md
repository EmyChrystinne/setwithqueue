# setwithqueue
Miniprojeto 1-01 ESTD - Emylle, Jardel e Arthur

Mini-projeto 1: Implementação de um Conjunto Usando Fila Integrantes da Equipe; Emylle Chrystinne, Arthur Passos e Jardel Cleyson

Descrição do Projeto Este projeto consiste na implementação de uma estrutura de dados SetWithQueue utilizando uma fila (FilaArray). A estrutura visa criar um conjunto que garanta que não haja elementos duplicados, utilizando operações de adição, remoção, verificação de existência, tamanho e listagem dos elementos.

Estrutura do Projeto

Classe FilaArray: Implementa uma fila usando uma lista (array). Oferece operações básicas como:
enqueue(item): Adiciona um item ao final da fila.
dequeue(): Remove o item do início da fila.
isEmpty(): Verifica se a fila está vazia.
size(): Retorna o tamanho atual da fila.
top(): Retorna o elemento no início da fila sem removê-lo.
list(): Retorna uma lista com todos os elementos da fila.
Classe SetWithQueue: Implementa um conjunto utilizando a FilaArray e um set para garantir a unicidade dos elementos.
Métodos:

add(element): Adiciona um elemento ao conjunto se ele não estiver presente.
remove(element): Remove um elemento do conjunto. Lança uma exceção (ValueError) se o elemento não estiver presente.
contains(element): Retorna True se o elemento estiver presente no conjunto e False caso contrário.
size(): Retorna o número de elementos no conjunto.
list(): Retorna todos os elementos do conjunto na forma de uma lista, mantendo a ordem de inserção.
Como Executar o Código Certifique-se de ter Python instalado em sua máquina. Baixe ou clone o repositório com o código fonte. Salve os arquivos do código em uma pasta local. Execute o arquivo .py principal para ver os testes e operações do SetWithQueue em funcionamento.

Materiais Consultados Documentação oficial do Python https://docs.python.org/3/ Real Python - Tutorial sobre listas e conjuntos. https://realpython.com/queue-in-python/

Comentário da Equipe Status do Projeto: O projeto foi concluído conforme solicitado, incluindo a implementação da classe SetWithQueue e seus métodos obrigatórios. Todos os testes propostos foram realizados com sucesso.

Dificuldades Encontradas: A principal dificuldade foi garantir a remoção correta dos elementos sem alterar a ordem de inserção na fila. A implementação foi ajustada para criar uma fila temporária durante o processo de remoção, o que manteve a integridade dos dados.

Possíveis Problemas Identificados: Nenhum problema significativo foi encontrado na lógica, mas há uma oportunidade de otimização no processo de remoção. Como a fila é reconstruída em cada operação de remoção, o tempo de execução pode ser melhorado.

Discussão sobre o Desempenho das Operações

add(element): Complexidade: O(1) para verificar e adicionar ao set, e O(1) para adicionar à fila. A operação de adição é eficiente devido ao uso do set para verificar duplicidade.
remove(element): Complexidade: O(n), onde n é o número de elementos na fila, pois é necessário percorrer todos os elementos da fila para criar uma nova fila sem o elemento a ser removido.
contains(element): Complexidade: O(1), pois utiliza um set para verificar a presença de um elemento.
size(): Complexidade: O(1), já que retorna o tamanho da estrutura usando o método size da fila.
list(): Complexidade: O(n), onde n é o número de elementos na fila. Retorna uma lista com todos os elementos em ordem de inserção
