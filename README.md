# prova-estrutura-de-repetição.

#[LPIA-A04] Você está desenvolvendo um programa em Python para calcular a soma dos números pares dentro de um intervalo determinado pelo usuário. 
#O programa deve solicitar ao usuário que insira dois números inteiros, representando o início e o fim do intervalo (inclusive).
#Utilize um loop 'for' para iterar sobre todos os números no intervalo e somar apenas os números pares.
#Implemente a estrutura 'else' para exibir uma mensagem indicando que não há números pares no intervalo, caso seja o caso.
#Ao final, exiba a soma dos números pares encontrados.


inicio = int(input("Digite o número inicial do intervalo: "))
fim = int(input("Digite o número final do intervalo: "))

soma_pares = 0
encontrou_par = False
for numero in range(inicio, fim + 1):
    if numero % 2 == 0:
        soma_pares += numero
        encontrou_par = True
else:
    if not encontrou_par:
        print("Não há números pares no intervalo informado.")
print("Soma dos números pares no intervalo:", soma_pares)
