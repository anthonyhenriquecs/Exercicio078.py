# Exercicio078.py

listanum = list()
mai = 0
men = 0
for c in range(0,5):
    listanum.append(int(input(f'Digite um numero para a posição {c}:')))
    if c == 0:
        mai = men = listanum[0]
    else:
        if listanum[c] > mai:
            mai = listanum[c]
        if listanum[c] < men:
            men = listanum[c]
print(f'Voce digitou os valores:{listanum}')
print(f'O maior foi: {mai} nas posições ',end='')
for i, v in enumerate(listanum):
    if v == mai:
        print(f'{i}...',end='')
print()
print(f'O menor foi: {men} nas posições ',end='')
for i, v in enumerate(listanum):
    if v == men:
        print(f'{i}...',end='')
print()
