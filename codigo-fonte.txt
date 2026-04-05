import random

print("Uma pesca Minimalista")
pontos = 0

while True:
    acao = input("\nDigite 'pescar' ou 'sair': ")

    if acao == "sair":
        break

    if acao == "pescar":
        numero = random.randint(1, 5)

        if numero == 3:
            print("Você pegou um peixe!")
            pontos += 1
        else:
            print("Nada... Tente novamente.")
    else:
        print("Comando inválido. Digite 'pescar' ou 'sair'.")

print("\nJogo encerrado")
print("Pontos:", pontos)
