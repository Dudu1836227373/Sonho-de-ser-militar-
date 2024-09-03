# Sonho-de-ser-militar-import random

def jogo_adivinhacao():
    numero_secreto = random.randint(1, 100)
    tentativas = 0
    acertou = False

    print("Bem-vindo ao jogo de adivinhação!")
    print("Tente adivinhar o número secreto entre 1 e 100.")

    while not acertou:
        palpite = int(input("Digite seu palpite: "))
        tentativas += 1

        if palpite < numero_secreto:
            print("Muito baixo! Tente novamente.")
        elif palpite > numero_secreto:
            print("Muito alto! Tente novamente.")
        else:
            acertou = True
            print(f"Parabéns! Você acertou o número secreto {numero_secreto} em {tentativas} tentativas.")

if __name__ == "__main__":
    jogo_adivinhacao()
