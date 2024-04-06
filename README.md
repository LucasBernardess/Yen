# Algoritmo de Yen para encontrar os K menores caminhos em um grafo sem ciclos

Este repositório contém uma implementação do algoritmo de Yen em C para encontrar os K menores caminhos em um grafo sem ciclos.

## Instruções de Uso

### Compilação

Para compilar o código, você pode usar o seguinte comando:

```
make
```

### Execução

Para executar o programa, use o seguinte formato de linha de comando:

```
./main -i <arquivo_de_entrada> -o <arquivo_de_saida>
```

- `-i`: Especifica o arquivo de entrada contendo as informações do grafo.
- `-o`: Especifica o arquivo de saída onde os resultados serão salvos.

## Estrutura do Código

O código fonte está dividido em vários arquivos para facilitar a organização e manutenção:

- `file_io.h`: Funções para processamento de entrada e saída de arquivos.
- `graph.h`: Estruturas e funções relacionadas ao grafo.
- `paths.h`: Definições de tipos e funções para caminhos no grafo.
- `yen.h`: Implementação do algoritmo de Yen.
- `dijkstra.h`: Implementação do algoritmo de Dijkstra utilizado pelo algoritmo de Yen.

## Como Utilizar

1. Compile o código usando o comando fornecido acima.
2. Execute o programa especificando o arquivo de entrada e de saída.
3. Verifique o arquivo de saída para visualizar os K menores caminhos encontrados.

## Exemplo de Uso

Suponha que você tenha um arquivo de entrada chamado `input.txt` com as informações do grafo. Você pode executar o programa da seguinte maneira:

```
./main -i input.txt -o output.txt
```

Isso processará o arquivo de entrada e salvará os resultados no arquivo `output.txt`.

## Licença

Este código é disponibilizado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---
Autor: Lucas Bernardes

