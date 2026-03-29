# Alu - 8 bits
# 🧠 ALU de 8 bits

Projeto de uma Unidade Lógica e Aritmética (ALU) de 8 bits desenvolvido utilizando lógica digital.

## 📖 Sobre o projeto

Este projeto consiste na implementação de uma ALU capaz de realizar operações aritméticas e lógicas utilizando circuitos digitais.

A ALU trabalha com dois operandos:
- **AC (Acumulador)** – registrador principal
- **N (Entrada)** – segundo operando

Além disso, utiliza:
- **MQ** – registrador auxiliar para multiplicação e divisão

---

## ⚙️ Operações implementadas

A ALU é capaz de realizar as seguintes operações:

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

## 🧩 Estrutura do projeto

A ALU foi construída de forma modular, dividida nos seguintes componentes:

### 🔹 Somador
Implementado inicialmente em 1 bit e expandido para 8 bits.

### 🔹 Subtrator
Baseado em complemento de dois utilizando o somador.

### 🔹 Multiplicador
Realiza multiplicação de 8 bits, separando resultado em:
- AC → parte menos significativa (LSB)
- MQ → parte mais significativa (MSB)

### 🔹 Divisor
Responsável por calcular:
- MQ → quociente
- AC → resto

### 🔹 Operações lógicas
- NAND
- XOR

### 🔹 Shift lógico
- Shift left (desloca bits para esquerda)
- Shift right (desloca bits para direita)

### 🔹 Seletor de operação (MUX)
Responsável por escolher qual operação será executada.

### 🔹 Registradores
- AC (Acumulador)
- MQ (Multiplicador/Quociente)

---

## 🔄 Funcionamento da ALU

A ALU recebe:
- Dois operandos (AC e N)
- Um seletor de operação

Com base no seletor:
1. A operação é escolhida
2. O circuito correspondente é ativado
3. O resultado é enviado para AC ou MQ

---

## 🖥️ Ferramenta utilizada

Projeto desenvolvido utilizando simulador de circuitos digitais.

- Digital

---

## 🎥 Vídeo explicativo

📌 Assista ao vídeo explicando o funcionamento da ALU:
https://youtube.com/seu-video

---

## 🚀 Como executar

1. Abra o simulador
2. Carregues o circuito
3. Insira valores(1 ou 0)
4. Escolha a operação no seletor
5. Observe o resultado nos registradores

---

## 📌 Observações

- O projeto foi feito de forma modular para facilitar entendimento
- O foco principal foi entender o funcionamento interno de uma ALU

---

## 👨‍💻 Autor

Desenvolvido por:
- Kaian Moura
