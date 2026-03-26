# Sistema de Gerenciamento de Hotel em C

## Descrição do Projeto

Este projeto implementa um sistema de gerenciamento de hotel desenvolvido em linguagem C, permitindo controlar reservas, check-in, check-out e informações dos hóspedes.

O sistema simula o funcionamento básico de um hotel, utilizando uma matriz bidimensional para representar os apartamentos distribuídos em andares. Cada posição da matriz armazena o status do quarto e os dados do hóspede.

O objetivo do projeto é aplicar conceitos de estruturas de dados, manipulação de matrizes e programação estruturada.

---

## Estrutura do Sistema

O hotel é representado por uma matriz:

* **20 andares**
* **14 apartamentos por andar**
* Total: **280 quartos**

Cada quarto pode estar em um dos seguintes estados:

* `.` → Livre
* `R` → Reservado
* `O` → Ocupado

---

## Funcionalidades

* Check-in de hóspedes
* Check-out de hóspedes
* Reserva de apartamentos
* Cancelamento de reservas
* Visualização do mapa do hotel
* Consulta de informações do hóspede
* Cálculo da taxa de ocupação e reservas

---

## Funcionamento

O sistema funciona através de um menu interativo no terminal:

1. O usuário escolhe uma opção
2. Informa o andar e o apartamento
3. O sistema executa a operação desejada
4. O status do quarto é atualizado na matriz

Durante o check-in, são armazenadas informações como:

* Nome
* CPF
* Telefone
* E-mail
* Endereço

---

## Menu do Sistema

1 - Check-in de hóspede
2 - Check-out de hóspede
3 - Reservar apartamento
4 - Cancelar reserva
5 - Mapa do hotel
6 - Informações do hóspede
7 - Taxa de ocupação e reservas
8 - Sair

---

## Exemplos de Execução

### Exemplo de mapa do hotel:

```
Apto ->        1  2  3  4 ... 14

Andar 20       .  R  O  . ... .
Andar 19       .  .  O  . ... .
...
Andar 1        .  .  .  . ... .
```

---

### Exemplo de reserva:

```
Digite o andar e o apartamento: 5 3
Reserva efetuada
```

---

### Exemplo de check-in:

```
Digite o andar e o apartamento: 5 3
Nome: Maria Silva
CPF: 12345678900
Celular: 11999999999
E-mail: maria@email.com
Endereco: Rua X

Check-in efetuado
```

---

## Observações Importantes

* O sistema não utiliza banco de dados, os dados são armazenados apenas em memória
* As informações são perdidas ao encerrar o programa
* Não há validação completa de entradas (ex: formato de CPF)
* O uso da função `gets()` pode gerar problemas de segurança (buffer overflow)
* O índice da matriz começa em 0, mas o usuário interage com valores iniciando em 1

---

## Possíveis Melhorias

* Substituir `gets()` por `fgets()` para maior segurança
* Implementar persistência de dados em arquivos
* Criar interface gráfica
* Validar entradas do usuário
* Adicionar sistema de login para funcionários
* Implementar categorias de quartos

---

## Conceitos Praticados

* Matrizes bidimensionais
* Estruturas (`struct`)
* Manipulação de strings
* Entrada e saída de dados
* Lógica condicional
* Modularização com funções
* Simulação de sistemas reais
