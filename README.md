# Jogo-jokenpo-Em-Python
Jogo jokenpo Em Python

from random import randint
from time import sleep

itens = ('Pedra', 'Papel', 'Tesoura')
computador = randint(0,2)
print('''Suas opções :
[0] PEDRA
[1] PAPEL
[2] TESOURA''')

jogador = int(input('Qual É A Sua Jogada: '))
print('JO')
sleep(1)
print('KEN')
sleep(1)
print('PO')
sleep(2)
print('-=' * 11)

print(f'computador jogou: {itens[computador]}')
print(f'Jogador jogou: {itens[jogador]}')
print('-=' * 11)

if computador == 0: #computador jogou PEDRA
   if jogador == 0:
       print('EMPATE')

   elif jogador ==1:
       print('JOGADOR VENCE')

   elif jogador ==2:
       print('COMPUTADOR VENCEU')

   else:
       print('JOGADA INVALIDA')

elif computador ==1: #computador jogou PAPEL
   if jogador == 0:
       print('JOGADOR VENCE')

   elif jogador == 1:
       print('EMPATE')

   elif jogador == 2:
       print('COMPUTADOR VENCEU')

   else:
       print('JOGADA INVALIDA')

elif computador ==1: #computador jogou TESOURA
   if jogador == 0:
       print('JOGADOR VENCE')

   elif jogador == 1:
       print('COMPUTADOR VENCEU')

   elif jogador == 2:
       print('EMPATE')

   else:
       print('JOGADA INVALIDA!')
