# pythonteste

##Identificar o triangulo:
 
cat1 = float(input('digite um cateto: '))
cat2 = float(input('digite outro cateto: '))
hipo = float(input('digite a hipotenusa: '))
if cat1 == cat2 and cat1 == hipo and cat2 ==hipo:
    print('E um triangulo equilatero')
elif cat1== cat2 and cat1 != hipo:
    print('E um triangulo isosceles')
elif cat1 != cat2 and cat2 != hipo:
    print('E um triangulo escaleno')

##Achar se o ano é bissesto ou não:
 
 ano = int(input('Digite o ano: '))
if (ano%4==0 and ano%100!=0) or (ano%400==0):
    print('Bissexto')
else:
    print('Não é bissexto')
    
##Faça um Programa que peça uma data no formato dd/mm/aaaa e determine se a mesma é uma data válida.

data = (input("Data:"))

if int(data[0:2]) != 0  and int(data[0:2]) <= 31 :
    if int(data[3:5]) != 0  and int(data[3:5]) <= 12 :
        if int(data[6:11]) != 0 :
            print("")
            print("Data Válida")
        else :
            print("")
            print("Data Inválida")
    else :
        print("")
        print("Data Inválida")
else:
    print("")
    print("Data Inválida")
    
 ##Faça um Programa para leitura de três notas parciais de um aluno.
    
    nota1 = float(input('digite a primeira nota: '))
nota2 = float(input('digite a segunda nota: '))
nota3 = float(input('digite a terceira nota: '))
media = (nota1 + nota2 + nota3)/3

if media >=7 :
    print(f'aprovado com media {media :.1F}')
    
elif media <=7 :
    print(f'reprovado com media {media :.1F}')
    
elif media ==10 :
    print(f'aprovado com distinçao com media {media :.1F}')
    
    ## jogo de advinhação
    
    print("*********************************")
print("Bem vindo ao jogo de Adivinhação!")
print("*********************************")

numero_secreto = 42
total_de_tentativas = 3

for rodada in range(1, total_de_tentativas + 1):
    print("Tentativa {} de {}".format(rodada, total_de_tentativas))
    chute_str = input("Digite um número entre 1 e 100: ")
    print("Você digitou " , chute_str)
    chute = int(chute_str)

    if(chute < 1 or chute > 100):
        print("Você deve digitar um número entre 1 e 100!")
        continue

    acertou = chute == numero_secreto
    maior   = chute > numero_secreto
    menor   = chute < numero_secreto

    if(acertou):
        print("Você acertou!")
        break
    else:
        if(maior):
            print("Você errou! O seu chute foi maior do que o número secreto.")
        elif(menor):
            print("Você errou! O seu chute foi menor do que o número secreto.")

print("Fim do jogo")
