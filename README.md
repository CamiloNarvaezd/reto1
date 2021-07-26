salario, numerohoras, bonificacion=input().split()
salario=float(salario)
numerohoras=int(numerohoras)
bonificacion=int(bonificacion)

##operaciones
hora_normal=salario/176
valor_hora_extra = hora_normal * 1.25
pago_extras = valor_hora_extra * numerohoras
##bonificacion

if bonificacion ==1:
    bonificacion = salario * 65/1000
else:bonificacion = 0    

salariobruto=salario+pago_extras+bonificacion

#deducciones

salud=salariobruto*25/1000
pension=salariobruto*25/1000
cajacompensacion=salariobruto*40/1000
 
total_deducciones = salud + pension + cajacompensacion

salarioneto = salariobruto - total_deducciones

print(round(salariobruto, 1), round(salarioneto, 1))
