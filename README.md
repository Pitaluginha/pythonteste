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
    
    Faça um Programa que peça um número inteiro e determine se ele é par ou impar. Dica: utilize o operador módulo (resto da divisão).
