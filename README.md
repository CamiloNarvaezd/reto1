salario, numerohoras, bonificacion= input().split()
salario = float(salario)
numerohoras = int(numerohoras)
bonificacion = int(bonificacion)

##operaciones
hora_normal = salario / 176
valor_hora_extra = hora_normal * 0.25

##bonificacion

if bonificacion ==1:
    bonificacion = salario * 0.065
else:bonificacion = 0    

salariobruto = salario + valor_hora_extra + bonificacion

#deducciones

salud = salariobruto * 0.25
pension = salariobruto * 0.25
cajacompensacion = salariobruto * 0.4

salarioneto = salariobruto-(salud+pension+cajacompensacion)


print(salariobruto)

print(salarioneto)
