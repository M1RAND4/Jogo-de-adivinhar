# Jogo de adivinhação

from random import randint
computador = randint (0, 10)
print('Sou seu computador... Acabei de pensar um número entre 0 e 10. ')
print('Será que Você consegue adivinhar qual foi? ')
acertou = False
palpite = 0
while not acertou:
    jogador = int(input('Qual seu palpite? '))
    palpite += 1 
    if computador == jogador:
        acertou = True
    else:
        if jogador < computador:
            print('Mais... Tente mais uma vez ')
        elif jogador > computador:
            print('Menos... Tente mais uma vez ')
print(f'Acertou... Com {palpite} palpites Parabêns...')