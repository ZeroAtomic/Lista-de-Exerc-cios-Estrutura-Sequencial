# Lista-de-Exercecios-Estrutura-Sequencial
Lista de Exercícios feitas por mim.
 1. Faça um programa que mostre a mensagem: 'Alô mundo'.
   R:
     printe('Alõ mundo.')


3. Faça um programa que peça um número e então mostre a mensagem: O número informado foi
[número].

   nome = input("informe um numero: 3")
print(f'O Numero informado foi {nome}')

 5. Faça um programa que peça dois números e imprima a soma.
 
  n1 = int(input("informe um numero: "))
  n2 = int(input("informe outro numero: "))
  soma = n1 + n2
  print(f'A soma dos dois numeros foi: {soma}')

    
7. Faça um programa que peça as 4 notas bimestrais e mostre a média.

n1 = int(input("informe a nota : "))
n2 = int(input("informe a nota : "))
n3 = int(input("informe a nota : "))
n4 = int(input("informe a nota : "))
result = (n1 + n2 + n3 + n4) / 4
print(f'Nota final é: {result}')

  
9. Faça um programa que converta metros para centímetros.
n1 = int(input("informe quantos metros: "))
result = 100 * n1
print(f'metros em centimetros: {result}')


10. Faça um programa que peça o raio de um círculo, calcule e mostre sua área.

n1 = int(input("informe o Raio do circulo: "))
result = 3.14 * n1 ** 2
print(f'A aréa do circulo é: {result}')
  
12. Faça um programa que calcule a área de um quadrado e mostre o dobro desta área.
n1 = int(input("informe o lado do quadrado: "))
n2 = int(input("informe o lado do quadrado: "))
result = n1 * n1
result *= 2
print(f'a area dobrada do quadrado é: {result}')

 14. Faça um programa que pergunte quanto você ganha por hora e o número de horas trabalhadas no
mês. Calcule e mostre o salário total do mês.

n1 = float(input("quanto ganha por hora "))
n2 = int(input("quantas horas vc trabalha no mes "))
result = n1 * n2
print(f'a area do quadrado é: {result}')


 16. Faça um programa que peça a temperatura em Fahrenheit e converta para Celsius. Fórmula: C = 5
* ((F - 32) / 9).

f = float(input("Digite a temperatura em Fahrenheit: "))
c = 5 * ((f - 32) / 9)
print(f"A temperatura em Celsius é: {c:.2f}°C")


 11.  Faça um programa que peça a temperatura em Celsius e converta para Fahrenheit. Fórmula: F =
(C * 9/5) + 32.
c = float(input())
F = (c * 9/5) + 32.
print(f'temperatura: {F}')


 12. Peça dois números inteiros e um número real. Calcule: (a) o produto do dobro do primeiro com
 metade do segundo; (b) a soma do triplo do primeiro com o terceiro; (c) o terceiro elevado ao cubo.

a = int(input())
b = int(input())
c = float(input())
a1 = a

a *= 2
b /= 2
r = a * b

a1 *= 3
a1 += c

cubo = c ** 3

print(f'Qualculo (A) {r}')
print(f'Qualculo (b) {a1}')
print(f'Qualculo (c) {cubo}')




14. Converta um valor em Gigabytes para Megabytes. Fórmula: MB = GB * 1024.
GB = int(input())

MB = GB * 1024.

print(f'Qualculo {MB}')



15. Converta um valor em Gigabytes para Megabytes e Kilobytes.

GB = int(input())

MB = GB * 1024
KB = MB * 1024

print(f'Mega {MB}')
print(f'Kilo {KB}')


16. Um pescador paga multa de R$4,00 por quilo excedente caso ultrapasse 50 kg de peixes. Faça
um programa que calcule excesso e multa.

quilo = float(input("Informe o quilo: "))
qi = quilo
if quilo > 50:
    quilo -= 50
    quilo *= 4
    print(f'Kilos {qi}')
    print(f'multa de R${quilo:.2f} Reais')
else:
    print(f'quilo: {quilo}')
    print('Sem multa')
    
18. Faça um programa que calcule o salário com descontos: IR (11%), INSS (8%) e Sindicato (5%).
Mostrar salário bruto e líquido.
salar = float(input("Informe o salario: "))
ir = salar * 11 /100
inss = salar * 8 /100
sind = salar * 5 /100

salarL = salar - ir - inss - sind

print(f'seu salario Bruto: {salar:.2f}')
print(f'seu salario liquido: {salarL:.2f}')

20. Uma loja de tintas precisa calcular quantas latas comprar. 1 litro cobre 3 m2, lata tem 18 litros e
custa R$80.
lata = int(input("Informe quantas latas: "))

quantDetinta = lata * 18
precolata = lata * 80
print(f'latas: {lata}')
print(f'Litros: {quantDetinta}')
print(f'Preço: {precolata:.2f}')

22. Versão avançada da tinta: 1 litro cobre 6 m2. Lata 18L (R$80) e galão 3,6L (R$25). Calcular
melhor opção com 10% de folga.
area = float(input("Digite o tamanho da área (m2): "))

 2. Cálculos de base
litros = (area * 1.10) / 6  # Área com 10% de folga dividida pelo rendimento

Cálculo das opções 
latas_apenas = litros / 18
galoes_apenas = litros / 3.6

 Cálculo do Mix 
latas_mix = int(litros / 18)         
galoes_mix = (litros % 18) / 3.6      #

Preços
preco_latas = latas_apenas * 80
preco_galoes = galoes_apenas * 25
preco_mix = (latas_mix * 80) + (galoes_mix * 25)

 Resultados
print(f"Litros necessários: {litros:.2f}")
print(f"Apenas latas: {latas_apenas:.2f} unidades - R$ {preco_latas:.2f}")
print(f"Apenas galões: {galoes_apenas:.2f} unidades - R$ {preco_galoes:.2f}")
print(f"Mix: {latas_mix} latas e {galoes_mix:.2f} galões - R$ {preco_mix:.2f}")


24. Faça um programa que calcule o tempo aproximado de download de um arquivo dado seu
tamanho (MB) e velocidade da internet (Mbps).

MB = float(input("Informe tamanho do arquivo: "))
Mbps = float(input("Informe sua internet: "))
MB *= 8
tempDonw = MB / Mbps
minutos = tempDonw /60
print(f'tempo para down: {minutos:.2f}')


