# Sistemas Operacionais 1

Repositório contendo os arquivos de estudo e exercícios práticos da disciplina de Sistemas Operacionais 1 do curso de Ciência da Computação.

## Sobre a Disciplina

Esta disciplina aborda conceitos fundamentais de sistemas operacionais, com foco especial em programação concorrente e gerenciamento de processos. Os códigos foram desenvolvidos em C, utilizando APIs específicas de Windows e Linux.

## Estrutura do Repositório

### Exercícios - MultiThreads
Exercícios práticos sobre programação com threads no Windows:

- **Ex1.c**: Preenchimento paralelo de matriz 10000x10000 utilizando múltiplas threads para otimizar o processamento
- **Ex2.c**: Sistema de threads que imprimem números e caracteres de forma concorrente, com modificação dinâmica do caractere via teclado
- **Ex3.c**: Animação de caracteres movendo-se na tela em diferentes linhas e velocidades usando threads

### MultiProgramação
Exemplos e exercícios sobre multiprogramação e gerenciamento de processos:

#### Exercícios Linux
- **ex1.c**: Criação e gerenciamento de processos filhos com controle via PID, incluindo finalização seletiva
- **ex3.c**: Criação de processos filhos com tempo de bloqueio definido e sincronização usando `wait()`

#### Exemplo de Jogo
- **ExemploJogo.c**: Jogo de nave espacial com sistema de disparo implementado usando threads e mutex para sincronização

### Projeto Pacman
Implementação completa de um jogo Pacman em C com programação concorrente:

- Sistema de threads para movimentação do Pacman e fantasmas
- Inteligência artificial básica para os fantasmas (perseguição e movimento aleatório)
- Sincronização usando mutex para evitar condições de corrida
- Sistema de pontuação e detecção de colisões
- Interface gráfica no terminal usando caracteres ASCII

## Conceitos Abordados

### Threads e Concorrência
- Criação e gerenciamento de threads (`_beginthread`, `CreateThread`)
- Sincronização com mutex (`CreateMutex`, `WaitForSingleObject`, `ReleaseMutex`)
- Comunicação entre threads através de variáveis compartilhadas
- Condições de corrida e proteção de seções críticas

### Processos
- Criação de processos com `fork()` (Linux)
- Sincronização de processos com `wait()`
- Sinais e controle de processos (`kill`, `signal`)
- Gerenciamento de múltiplos processos filhos

### Programação de Sistemas
- Manipulação de console (cores, cursor, tamanho de tela)
- Entrada de teclado não-bloqueante (`kbhit()`, `getch()`)
- Temporização e controle de velocidade (`Sleep()`, `sleep()`)

### Aplicações Práticas
- Jogos simples com múltiplas entidades concorrentes
- Processamento paralelo de dados (matrizes)
- Sistemas interativos em tempo real

## Tecnologias Utilizadas

- **Linguagem**: C
- **APIs Windows**: `windows.h`, `process.h`, `conio.h`
- **APIs Linux**: `unistd.h`, `sys/wait.h`, `signal.h`
- **Compiladores**: GCC (Linux), MinGW ou Visual Studio (Windows)

## Observações

- Os códigos foram desenvolvidos para fins educacionais
- Alguns exemplos são específicos para Windows (usando `windows.h`) e outros para Linux (usando `unistd.h`)
- É recomendado executar os códigos no sistema operacional apropriado para cada arquivo

---

**Nota**: Este repositório serve como registro de aprendizado e não deve ser utilizado para cópia em trabalhos acadêmicos.
