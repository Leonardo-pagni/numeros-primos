# numeros-primos-python
Elabore um programa em Python que recebe um número inteiro positivo qualquer de 0 a 100. O programa deverá verificar e exibir todos os números primos até o valor digitado.  A verificação se um número é primo deverá ser implementada por uma função que retorna um valor lógico ("True" ou "False") ao programa (ou script) principal.

def Primos(N):
    ax = False
    t = 0
    for i in range (1, N+1):
        if N % i ==0:
            t += 1
    if t == 2:
        ax = True
    return ax

entrada = int(input("escreva um numero inteiro de 0 até 100 = "))
while(entrada < 0 or entrada > 100):
    entrada = int(input("numero inválido, digite novamente: "))
print(f"Os números primos de 1 até {entrada} são:")
    
for c in range (1, entrada+1):
    if Primos(c) == True:
        print (c)
