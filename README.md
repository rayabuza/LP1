# Problema da Mochila - Algoritmo de Programação Dinâmica
Este código implementa uma solução para o **problema da mochila (knapsack problem)** utilizando a abordagem de programação dinâmica. O problema da mochila consiste em determinar **a combinação de itens de maior valor que pode ser colocada em uma mochila, considerando que cada item possui um peso e um valor associado, e a mochila possui uma capacidade máxima**.

# Estrutura de Dados
 O código utiliza a seguinte estrutura de dados para representar um item:

```c
Copy code
typedef struct {
  int peso;
  int valor;
} Item;
```
Cada item possui um peso (inteiro) e um valor (inteiro).

# Funções Principais
 O código possui as seguintes funções principais:

**int maximo_valor(int valor1, int valor2)**: 
Retorna o valor máximo entre dois valores inteiros.

**void mochila(Item *lista, int quantidade, int capacidade)**: 
Resolve o problema da mochila utilizando programação dinâmica. Recebe como parâmetros um array de itens, a quantidade de itens e a capacidade da mochila. A função preenche uma tabela com os valores máximos alcançáveis em diferentes capacidades e quantidades de itens. Ao final, imprime a combinação de itens com o maior valor e chama a função buscar_escolhidos para encontrar e imprimir os itens escolhidos para a mochila.

**void buscar_escolhidos**(**int** **tabela_R, int capacidade, int N_itens, Item *lista)**: 
Função recursiva que encontra os itens selecionados para a mochila com base na tabela preenchida pela função mochila. Recebe como parâmetros a tabela preenchida, a capacidade da mochila, a quantidade de itens e o array de itens. A função percorre a tabela de forma recursiva, identificando os itens que foram incluídos na solução e imprimindo suas informações.

**void encontrar_erros(int casos)**: 
Imprime mensagens de erro correspondentes a diferentes casos de erro e encerra o programa.

**void ler_arquivo(char *nome)**: 
Lê as informações sobre os itens e a capacidade da mochila de um arquivo. Recebe como parâmetro o nome do arquivo a ser lido. A função abre o arquivo em modo de leitura, realiza a leitura das informações e chama a função encontrar_erros em caso de erros.

**int main()**: 
Função principal do programa. Solicita ao usuário o nome do arquivo a ser lido, chama a função ler_arquivo com o nome do arquivo e retorna 0 no final.

# Como Utilizar
 Compile o código utilizando um compilador C compatível.

 Execute o programa gerado.

- O programa solicitará o nome do arquivo a ser lido. Digite o nome do arquivo, incluindo a extensão .txt, e pressione Enter.

- O programa executará o algoritmo de programação dinâmica para resolver o problema da mochila com base nas informações contidas no arquivo.

- O programa imprimirá a combinação de itens com o maior valor possível e as informações sobre cada item selecionado.

- O programa encerrará sua execução.

 # Considerações Finais 
 Certifique-se de fornecer um arquivo de entrada válido no formato especificado pelo programa. O arquivo deve conter as informações sobre os itens e a capacidade da mochila, seguindo a estrutura correta.

Este código implementa uma **solução eficiente para o Problema da Mochila usando programação dinâmica**, o que garante uma abordagem **otimizada** para encontrar a combinação de itens de **maior valor**. No entanto, é importante observar que o **desempenho do algoritmo pode ser afetado pelo número de itens e pela capacidade da mochila**. Caso enfrente problemas de desempenho com entradas muito grandes, é possível explorar técnicas adicionais, como a otimização de memória ou o uso de algoritmos alternativos.

Certifique-se de compreender o problema e o algoritmo implementado neste código antes de aplicá-lo a outros cenários ou fazer modificações. Você pode adaptar e estender este código de acordo com suas necessidades, como adicionar funcionalidades adicionais ou integrá-lo a outros sistemas.

Este código foi fornecido como uma solução básica para o Problema da Mochila usando programação dinâmica. Se você tiver requisitos específicos ou necessidades mais complexas, pode ser necessário adaptar ou utilizar abordagens diferentes.

Esperamos que este código seja útil para compreender e resolver o Problema da Mochila, bem como para estudar e explorar conceitos relacionados à programação dinâmica em algoritmos.

Se você tiver alguma dúvida ou encontrar algum problema ao utilizar este código, sinta-se à vontade para entrar em contato para obter suporte adicional.
 
