# Processamento Assíncrono com Spring Batch
Este projeto ilustra a criação de um job simples utilizando Spring Batch para ler e processar dados de um arquivo CSV.

## Estrutura do Spring Batch
O Spring Batch é uma poderosa estrutura para processamento de grandes volumes de dados em lote. Ele segue a arquitetura Reader-Processor-Writer (Leitor-Processador-Escritor), onde:

- Leitor (Reader): Extrai dados de uma fonte, como um banco de dados ou um arquivo.
- Processador (Processor): Executa transformações ou validações nos dados lidos.
- Escritor (Writer): Insere ou atualiza os dados processados em um destino.

## Implementação do Processamento Assíncrono

Busquei otimizar o desempenho e reduzir a latência total do processamento de dados, aplicando a lógica de processamento assíncrono. Isso foi alcançado criando múltiplos processadores e distribuindo as tarefas em várias threads, permitindo que diferentes partes do lote sejam processadas simultaneamente.

## Conclusão
Ao aplicar a lógica de processamento assíncrono no Spring Batch, consegui criar uma solução mais rápida e eficiente para o processamento dos dados do CSV em lote. Isso não apenas reduz o tempo de execução, mas também melhora a capacidade do sistema de lidar com grandes volumes de dados.