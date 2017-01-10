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
