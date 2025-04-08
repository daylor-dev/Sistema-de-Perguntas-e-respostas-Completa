# Sistema-de-Perguntas-e-respostas-Completa
Código de um sistema de perguntas e respostas. Linguagem Python
#Exercício - sistema de perguntas e resposta

perguntas = [
    {'pergunta' : 'Qual foi o primeiro computador inventado?', 
     'alternativas' : ['PP3', '4004', 'Eniac', 'GG2'],
     'resposta correta' : 'Eniac'},

    {'pergunta' : 'Quanto é 23 em bits?',
     'alternativas' : [1000, 1101, 10111,1111],
     'resposta' : 10111},

     {'pergunta': 'Quanto é 2 + 2?',
      'alternativas' : [1, 2, 3, 4],
      'resposta correta' : 4}
]

p1 = perguntas[0].get('pergunta')
alternativas_1 = perguntas[0].get('alternativas')
acertos = 0
erros = 0 

print(f'\n {p1}')
for i, alternativa in enumerate(alternativas_1):
    print(f'{i})', alternativa)

escolha = input('Digite a opção correta:  ') 
    
if escolha == '2':
    print('Você acertou ✅')
    acertos+= 1

else:
    print('Você errou! ❌')
    erros += 1


p2 = perguntas[1].get('pergunta')
alternativas_2 = perguntas[1].get('alternativas')


print(f'\n {p2}')
for k, alternativa2 in enumerate(alternativas_2):
    print(f'{k})', alternativa2)

escolha1 = input('Digite a opção correta ') 
    
if escolha1 == '2':
    print('Você acertou ✅')
    acertos+= 1

else:
    print('Você errou! ❌')
    erros += 1


p3 = perguntas[2].get('pergunta')
alternativas_3 = perguntas[2].get('alternativas')
print(f' \n {p3}')
for l, alternativa3 in enumerate(alternativas_3):
    print(f'{l})', alternativa3)

escolha2 = input('Digite a opção correta ') 
    
if escolha2 == '2':
    print('Você acertou ✅')
    acertos+= 1

else:
    print('Você errou! ❌')
    erros += 1

print(f'Você acertou {acertos} e errou { erros}')


