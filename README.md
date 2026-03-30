# ALU de 8 bits

Projeto de uma Unidade Lógica e Aritmética (ALU) de 8 bits desenvolvido utilizando lógica digital.

## Sobre o projeto

Este projeto consiste na implementação de uma ALU capaz de realizar operações aritméticas e lógicas utilizando circuitos digitais.

A ALU trabalha com dois operandos:
- **AC (Acumulador)** – registrador principal
- **N (Entrada)** – segundo operando

Além disso, utiliza:
- **MQ** – registrador auxiliar para multiplicação e divisão

---

## Operações implementadas

| Operação       | Descrição |
|----------------|----------|
| Soma           | AC + N |
| Subtração      | AC - N |
| Multiplicação  | AC * N |
| Divisão        | AC / N |
| NAND           | AC NAND N |
| XOR            | AC XOR N |
| Shift Left     | Deslocamento lógico para esquerda |
| Shift Right    | Deslocamento lógico para direita |

---

## Estrutura do projeto

### 🔹 Somador
Implementado inicialmente em 1 bit e expandido para 8 bits.

### 🔹 Subtrator
Baseado em complemento de dois utilizando o somador.

### 🔹 Multiplicador
- AC → parte menos significativa (LSB)
- MQ → parte mais significativa (MSB)

### 🔹 Divisor
- MQ → quociente
- AC → resto

### 🔹 Operações lógicas
- NAND
- XOR

### 🔹 Shift lógico
- Shift left
- Shift right

### 🔹 Seletor de operação (MUX)
Responsável por escolher qual operação será executada.

### 🔹 Registradores
- AC
- MQ

---

## Funcionamento da ALU

A ALU recebe:
- Dois operandos (AC e N)
- Um seletor de operação

Com base no seletor:
1. A operação é escolhida
2. O circuito correspondente é ativado
3. O resultado é enviado para AC ou MQ

---

## 🧠 Fundamentação lógica

### Mapa de Karnaugh (XOR)

| A | B | Saída |
|---|---|------|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

Equação:
S = A'B + AB'

---

### Mapa de Karnaugh (NAND)

| A | B | Saída |
|---|---|------|
| 0 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

Equação:
S = (AB)'

---

## Exemplos matemáticos

### Soma
AC = 00000001  
N  = 00000011  
Resultado = 00000100  

### Subtração
AC = 00000101  
N  = 00000011  
Resultado = 00000010  

### Multiplicação
AC = 00000011  
N  = 00000010  
Resultado = 00000110  

### Divisão
AC = 00000110  
N  = 00000010  
MQ = 00000011  
AC = 00000000  

### XOR
AC = 10101010  
N  = 11001100  
Resultado = 01100110  

### NAND
AC = 10101010  
N  = 11001100  
Resultado = 01011111  

### Shift Left
AC = 00001101  
Resultado = 00011010  

### Shift Right
AC = 00001101  
Resultado = 00000110  

---

## Vídeo

https://youtu.be/8wgfl1krLK4

---

##  Como executar

1. Abra o simulador
2. Carregue o circuito
3. Insira valores
4. Escolha a operação
5. Observe o resultado

---

## Autor

Kaian Moura
