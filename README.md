# DIGITOS_PARES_IMPARES_MULT_3X
este programa muestra la cantidad de digitos pares e impares que tiene un numero dado, asi como la cantidad de numeros multiplos de 3 introducidos por el usuario. El script termina cuando se introduce -1

dig_par=[]
dig_impar=[]
multiplos_tres=0
while True:
    numero=int(input("Inserte numero: "))
    if str(numero)=="-1":
        break
    for i in str(numero):
        if int(i)%2==0:
            dig_par.append(i)
        else:
            dig_impar.append(i)
    if numero%3==0:
        multiplos_tres+=1
    print("El numero {} tiene {} cifras pares y {} cifras impares".format(numero,len(dig_par),len(dig_impar)))
    dig_par=[]
    dig_impar=[]
print("Hay {} numeros multiplos de 3".format(multiplos_tres))
