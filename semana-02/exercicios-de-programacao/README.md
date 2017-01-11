**Nesta lista de exercícios vamos praticar os conceitos vistos até agora. Cada exercício deve ser resolvido em um arquivo separado e a seguir enviado através da web. A correção automática pode demorar alguns minutos. Você pode submeter a mesma resposta mais de uma vez caso perceba que a resposta anterior tinha algum problema; a última versão é a que vale.**

**Note que a correção verifica se o resultado corresponde exatamente ao que foi pedido no enunciado. Letras maiúsculas ou minúsculas, número de espaços e pontuação diferentes do pedido são tratados como erro.**

_______________________________
## Exercício 1

Uma empresa de cartão de crédito envia suas faturas por email com a seguinte mensagem:

> Olá, Fulano de Tal

> A sua fatura com vencimento em 9 de Janeiro no valor de R$ 350,00 está fechada.

Escreva um programa que receba (entrada de dados através do teclado) o nome do cliente, o dia de vencimento, o mês de vencimento e o valor da fatura e imprima (saída de dados) a mensagem com os dados recebidos, no mesmo formato da mensagem acima. Note que o programa imprime a saída em duas linhas diferentes. Note também que, como não é preciso realizar cálculos, o valor não precisa ser convertido para número, pode ser tratado como texto.

Abaixo um exemplo de como deve ser a entrada e saída de dados do programa:

Exemplo:

- Entrada de Dados:

> Digite o nome do cliente: Fulano de Tal

> Digite o dia de vencimento: 9

> Digite o mês de vencimento: Janeiro

> Digite o valor da fatura: 350,00

- Saída de Dados:

> Olá, Fulano de Tal

> A sua fatura com vencimento em 9 de Janeiro no valor de R$ 350,00 está fechada.

### RESPOSTA:

```c
nomeclient = input ("Digite o nome do cliente: ")
contavenc = input ("Digite o dia de vencimento: ")
mesvenc = input ("Digite o mês de vencimento: ")
valorfat = input ("Digite o valor da fatura: ")

print("Olá,", nomeclient)
print("A sua fatura com vencimento em", contavenc, mesvenc, "no valor de R$"+valorfat, "está fechada." )
```
_____________________________
## Exercício 2

Faça um programa em Python que receba (entrada de dados) o valor correspondente ao lado de um quadrado, calcule e imprima (saída de dados) seu perímetro e sua área.

Observação: a saída deve estar no formato: **"perímetro: x - área: y"**

Abaixo um exemplo de como deve ser a entrada e saída de dados do programa:

Exemplo:

- Entrada de Dados:

**Digite o valor correspondente ao lado de um quadrado: 3**

- Saída de Dados:

**perímetro: 12 - área: 9**

### RESPOSTA:

```c
ladqudrado = int(input("Digite o valor correspondente ao lado de um quadrado: "))
perimetro = ladqudrado * 4
area = ladqudrado * ladqudrado

print("perímetro:", perimetro, "- área", area)
```

_____________________________________________
## Exercício 3

Desafio do vídeo "Entrada de Dados": Reescreva o programa contaSegundos para imprimir também a quantidade de dias, ou seja, faça um programa em Python que dada a quantidade de segundos, o programa "quebra" esse valor em dias, horas, minutos e segundos. A saída deve estar no formato: <b>a dias, b horas, c minutos e d segundos.</b>

Abaixo um exemplo de como deve ser a entrada e saída de dados do programa:

Exemplo:

- Entrada de Dados:

**Por favor, entre com o número de segundos que deseja converter: 178615**

- Saída de Dados:

**2 dias, 1 horas, 36 minutos e 55 segundos.**

```c
totalSeg = int(input("Por favor, entre com o número de segundos que deseja converter: "))

segRestantes = totalSeg % 3600
segundos = segRestantes % 60
minutos = segRestantes // 60
horas = (totalSeg // 3600) % 24
dias = (totalSeg // 3600) // 24

print(dias, "dias,", horas, "horas,", minutos, "minutos e", segundos, "segundos.")
```
________________________________
## Exercício 4

Faça um programa em Python que recebe um número inteiro e imprime seu dígito das dezenas. Observe o exemplo abaixo:

Exemplo 1:

- Entrada de Dados:

**Digite um número inteiro: 78615**

- Saída de Dados:

**O dígito das dezenas é 1**

Exemplo 2:

- Entrada de Dados:

**Digite um número inteiro: 2**

- Saída de Dados:

**O dígito das dezenas é 0**

<b>Dica:</b> O operador "//" faz uma divisão inteira jogando fora o resto, ou seja, aquilo que é menor que o divisor. O operador "%" devolve apenas o resto da divisão inteira jogando fora o resultado, ou seja, tudo que é maior ou igual ao divisor.

### RESPOSTA:

**RESPOSTA 1:** 
```c
numero = int(input("Digite um número inteiro: "))
digitoDezena = 0 if (numero < 10) else (numero // 10 % 10)
print("O dígito das dezenas é", digitoDezena)
```
**RESOSTA 2:**
```c
numero = int(input("Digite um número inteiro: "))
digitoDezena = 0 if (numero < 10) else (numero % 10 // 10)
print("O dígito das dezenas é", digitoDezena)
```
_________________________________
## Exercício 5

Faça um programa em Python que receba quatro notas, calcule e imprima a média aritmética. Observe o exemplo abaixo:

Exemplo:

- Entrada de Dados:

**Digite a primeira nota: 4**

**Digite a segunda nota: 5**

**Digite a terceira nota: 6**

**Digite a quarta nota: 7**

- Saída de Dados:

**A média aritmética é 5.5**

**RESPOSTA:**

```c

nota1 = int(input("Digite a primeira nota: "))
nota2 = int(input("Digite a segunda nota: "))
nota3 = int(input("Digite a terceira nota: "))
nota4 = int(input("Digite a quarta nota: "))

media = (nota1 + nota2 + nota3 + nota4) / 4

print("A média aritmética é", media)
```
_________________________________________
