# atvidade-03

QUESTÃO 1
F = int(input('Digite uma temperatura em graus FARENHEIT: '))
C = 5/9 * (F - 32)

print('{0} graus FARENHEIT é equivalente a {1} graus CELSIUS'.format(F, C))

QUESTÃO 2 

time = input('Digite o nome da equipe de futebol: ')
derrotas = int(input('O {} perdeu quantas partidas? '.format(time)))
empates = int(input('Quantos empates? '))
vitórias = int(input('Agora insira o número de vitórias do {} até o momento: '.format(time)))

pontos_ganhos = vitórias * 3 + empates
pontos_perdidos = derrotas * 3 + empates * 2

partidas = derrotas + empates + vitórias

print()
print('O {0} disputou {1} jogos'.format(time, partidas))
print('{0} pontos ganhos e {1} pontos perdidos'.format(pontos_ganhos, pontos_perdidos))
print aproveitamento = (pontos_ganhos / (pontos_ganhos + pontos_perdidos)) * 100

QUESTÃO 3

aluno = input('Digite o nome do aluno: ')
nota1 = float(input('Agora informe a nota da primeira avaliação: '))
nota2 = float(input('Agora informe a nota da segunda avaliação: '))
media = (nota1 + nota2) / 2

print()
print('Media: ', media)

if media < 7:
    print('O Aluno foi reprovado!')
else:
    print('Parabéns {}, você foi aprovado(a)'.format(aluno))

QUESTÃO 4

num01 = int(input('Digite um valor:'))
num02 = int(input('Digite um valor:'))
if num01 == num02:
    print('Os valores digitados  são iguais')
elif num01 > num02:
    print('Maior número: {}'.format(num01))
elif num02 > num01:
    print('Maior número: {}'.format(num02))

QUESTÃO 5

inferior = superior = medio = 0

for i in range(10):
    altura = float(input('Digite sua altura: '))

    if altura < 1.6:
        inferior += 1
    elif altura > 1.8:
        superior += 1
    else:
        medio += 1
    
total = inferior + superior + medio

print('-*-' * 15)
print('Pessoas com altura menor que 1.60 ------> {}' .format(inferior))
print('Pessoas com altura maior que 1.80 ------> {}' .format(superior))
print('Pessoas com altura entre 1.60 e 1.80 ---> {}' .format(medio))
print('Total de pessoas cadastradas -----------> {}' .format(total))
print('-*-' * 15)
