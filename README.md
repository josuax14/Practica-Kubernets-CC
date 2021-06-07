# Practica-Kubernets-CC

#Los pasos realizados para esta práctica son:

#1 crear regla de abrir tcp

![Captura1cc](https://user-images.githubusercontent.com/34063107/121074956-da09c680-c7d4-11eb-86c9-5ca138232602.PNG)

#2 Conectarse al clúster

![Captura2cc](https://user-images.githubusercontent.com/34063107/121075076-07ef0b00-c7d5-11eb-85db-243461418495.PNG)¡

#3 Clon del git

![Captura3cc](https://user-images.githubusercontent.com/34063107/121075110-13dacd00-c7d5-11eb-9e3b-c7f40abbef97.PNG)

#4 Modificar el tipo

![Captura7cc](https://user-images.githubusercontent.com/34063107/121075218-35d44f80-c7d5-11eb-8a92-1c4dc12eeaf0.PNG)

![Captura6cc](https://user-images.githubusercontent.com/34063107/121075233-3b319a00-c7d5-11eb-9a87-7b85044f6b4d.PNG)

#5 Ejecutar el deploy

![Captura4cc](https://user-images.githubusercontent.com/34063107/121075276-4684c580-c7d5-11eb-8612-b32e2cfc5d20.PNG)

#6 Ver las ip externas para ver las páginas

![Captura9cc](https://user-images.githubusercontent.com/34063107/121075329-57cdd200-c7d5-11eb-9c53-ced65e1cdd95.PNG)

#7 Podemos ver la páginas por esas ip externas

![Captura8cc](https://user-images.githubusercontent.com/34063107/121075368-64eac100-c7d5-11eb-8051-c02a640aed9c.PNG)

![Captura10cc](https://user-images.githubusercontent.com/34063107/121075382-6ae0a200-c7d5-11eb-94c8-cb214ba1e0ab.PNG)

#8 Para cambiar el manualmente el número de nodos podemso lanzar esto:

gcloud container clusters resize cluster-1 --region us-central1-c --num-nodes=2

#9 Para poder permitir el escalar podemos lanzar
 
kubectl scale deployments/vote --replicas=4
 
#10 Para actualizar imágen
 
kubectl set image deployments/postgres postgres=postgres:postgres:10.4
