# Sistema de Atendimento — Squad

Projeto desenvolvido para a disciplina de PSC II — Engenharia de Software, com o objetivo de simular um sistema de atendimento médico utilizando estruturas de dados encadeadas em C++.

## Sobre o projeto

O sistema simula o atendimento de pacientes por médicos disponíveis.

O projeto utiliza estruturas de dados implementadas manualmente, sem o uso de estruturas prontas da STL como `vector`, `queue`, `stack` ou `list`.

## Requisitos implementados

### R1 — Fila de Pacientes

Foi implementada uma fila FIFO (First In, First Out).

Os pacientes entram no final da fila e são atendidos pela frente.

Funcionalidades:
- `enqueue()` — adiciona um paciente;
- `dequeue()` — remove o primeiro paciente;
- `frente_peek()` — consulta o próximo paciente sem removê-lo;
- `tamanho()` — informa a quantidade de pacientes na fila.

### R2 — Pilha de Histórico

Foi implementada uma pilha LIFO (Last In, First Out) para registrar os atendimentos realizados.

Funcionalidades:
- `push()` — adiciona um atendimento ao histórico;
- `pop()` — remove o último atendimento;
- `peek()` — consulta o último atendimento sem removê-lo.

### R3 — Lista de Médicos

Foi implementada uma lista encadeada para controlar os médicos disponíveis.

Funcionalidades:
- `adicionarMedico()` — adiciona um médico ao final da lista;
- `chamarMedico()` — remove o primeiro médico disponível;
- `percorrer()` — exibe os médicos disponíveis.

### R4 — Relatório de Atendimentos

Foi implementada a função `imprimirHistorico()` para apresentar os atendimentos registrados.

O histórico é preservado após a impressão utilizando uma pilha auxiliar.

## Estruturas utilizadas

- Fila encadeada (FIFO)
- Pilha encadeada (LIFO)
- Lista encadeada
- Ponteiros
- Alocação dinâmica
- `new` e `delete`

## Como compilar

No terminal, dentro da pasta do projeto, execute:

```bash
g++ -std=c++17 -Wall -o atendimento Aula16_atendimento_template.cpp