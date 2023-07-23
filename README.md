# Projeto CPU-RISCV-EEL580
CPU RISC-V de 32 Bits (com e sem vetorização) – Projeto da disciplina Arquitetura de Computadores (EEL580) da UFRJ

## Descrição

O projeto descreve o desenvolvimento de uma CPU RISC-V de 32 bits (RV32I) implementada em VHDL, com uma microarquitetura baseada em um pipeline de ao menos 5 estágios. O projeto foi realizado utilizando o simulador Logisim Evolution. A CPU é capaz de executar instruções inteiras e foi dividida em duas partes: Parte 1 (P1) e Parte 2 (P2).

## Parte 1 (P1) - Implementação Base da CPU

Na Parte 1, a CPU RISC-V foi projetada e implementada com suporte para um pipeline de 5 estágios. Foram utilizados blocos VHDL para a construção dos módulos e do pipeline. As memórias de instruções e dados foram projetadas separadamente e entregam uma palavra por ciclo. Para garantir a correta operação durante a carga de dados, as memórias foram modificadas para permitir carga assíncrona. A CPU foi adaptada para não operar durante esse processo e possui um sinal de reset. A parte 1 suporta um subconjunto da ISA RV32I, incluindo as seguintes instruções: add, addi, auipc, sub, and, andi, or, ori, xor, xori, sll, slli, srl, srli, lw, lui, sw, jal, jalr, beq e bne.

## Parte 2 (P2) - Suporte a Instruções Vetoriais

Na Parte 2, o projeto original da CPU RISC-V foi estendido para suportar o uso de instruções vetoriais. A CPU continua utilizando o pipeline de 5 estágios e as memórias de instruções e dados com carga assíncrona. A implementação das instruções vetoriais foi realizada utilizando blocos VHDL. Além das instruções vetoriais baseadas na atividade prática AVX, a CPU P2 também mantém o suporte ao subconjunto da ISA RV32I presente na Parte 1. As instruções vetoriais suportadas incluem: add, addi, auipc, sub, sll, slli, srl e srli.

## Arquivos .circ

Os arquivos .circ contêm os módulos implementados em VHDL e os circuitos correspondentes. Eles devem ser abertos utilizando o software Logisim Evolution, uma ferramenta de simulação e projeto de circuitos digitais. O Logisim Evolution permite visualizar e testar a implementação da CPU RISC-V em um ambiente de simulação interativo, possibilitando a análise do funcionamento dos circuitos e a verificação de sua correta operação.

## Autores

Este projeto foi desenvolvido em conjunto por Carolina Santiago, Gustavo Roxo e Zuilho Segundo. O trabalho foi realizado como parte da disciplina Arquitetura de Computadores (EEL580) da UFRJ.

