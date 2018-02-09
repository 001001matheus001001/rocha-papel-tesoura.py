# rocha-papel-tesoura.py
# Scprit feito por Matheus Silva
# 08/02/2018 Hs 21:30
# Simples Rocha,papel,tesoura Posivel emplementação de largato,spock


import random

escolha = ["rocha","papel","tesoura"]

print("Rocha esmaga Tesoura,Tesoura corta Papel, Papel cobre Rocha")

jogador = input("Escolha sua jogada , ROCHA , TESOURA ou press [ENTER]:")
while jogador != "":
    jogador = jogador.lower()
    computador = random.choice(escolha)
    print("Voce jogou: " +jogador+ ". O computador jogou: " +computador+ ".")

    if jogador == computador:
        print("Oou ouve empate.")

 # JOGADA 1 rocha contra tesoura tesoura contra rocha
    elif jogador == "rocha":
        if computador == "tesoura":
            print("Voce ganhou:")
        else:
            print("computador ganhou de voce seu noob !!! ")
 # JOGADA 2 papel contra rocha rocha contra papel
    elif jogador == "papel":
        if computador == "rocha":
            print("Voce ganhou:")
        else:
            print("computador ganhou de voce seu noob !!! ")
 # JOGADA 3 tesoura contra papel papel contra tesoura
    elif jogador == "tesoura":
        if computador == "papel":
            print("Voce ganhou:")
        else:
            print("computador ganhou de voce seu noob !!! ")
 # JOGADA 4

 # JOGADA 5
    else:
        print("Ajuste o codigo:")
    print()
    jogador = input("Escolha sua jogada ROCHA < PAPEL > TESOURA:")
