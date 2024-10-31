# Codigo #1 Del Examen Del Segundo Parcial

print(" ")#Espacio entre lineas 
print("Nombre Del Alumno: Ramirez Torres Angel Manuel")#Nombre del alumno
print("Grado y Grupo: 3°W")#Grado y grupo del alumno
print("NO. De Control: 1206")#Muestra el numero de control
print(" ")#Espacio entre lineas
#Nos muestra a continuacion las instrucciones del programa a realizar 
print("-INSTRUCCIONES-")
print("Escribir un programa que almacene las asignaturas de un curso")
print("por ejemplo Matemáticas, Física, Química, Historia y Lengua")
print("en una lista, pregunte al usuario la nota que ha sacado en cada asignatura")
print("y elimine de la lista las asignaturas aprobadas. Al final el programa debe mostrar")
print("por pantalla las asignaturas que el usuario tiene que repetir.")
#Fin de las instrucciones
print(" ")#Espacio entre lineas 

print("Codigo #1")

print(" ")#Espacio entre lineas 

#Se crea la ista de materias
materias = ["Matemáticas", "Física", "Química", "Historia", "Lengua"]

#Esta lista almacena las materias a repetir
materias_a_repetir = []

# Preguntar al usuario la nota en cada asignatura
for asignatura in materias:
    #Pide la calificacion
    nota = float(input(f"¿Qué calificacion has sacado en {asignatura}? "))
    
    #Se agrega una condicion, si la nota es <6 debe de repetir la materia 
    if nota < 6:
        materias_a_repetir.append(asignatura)

# Muestra las materias a repetir 
print("Tienes que repetir las siguientes materias:")
print(materias_a_repetir) if materias_a_repetir else print("¡Felicidades! Has aprobado todas las materias.")

![image](https://github.com/user-attachments/assets/4c00dee4-e6d8-48b8-ae08-cdf325a739c6)
![image](https://github.com/user-attachments/assets/0e5d3c94-b6b5-4251-b0ba-6a43e9b29130)


# Codigo #2 Del Examen Del Segundo Parcial

print(" ")#Espacio entre lineas 
print("Nombre Del Alumno: Ramirez Torres Angel Manuel")#Nombre del alumno
print("Grado y Grupo: 3°W")#Grado y grupo del alumno
print("NO. De Control: 1206")#Muestra el numero de control
print(" ")#Espacio entre lineas
#Nos muestra a continuacion las instrucciones del programa a realizar 
print("-INSTRUCCIONES-")
print("Escribir un programa que almacene el diccionario")
print("con los créditos de las asignaturas de un curso {'Matemáticas': 6, 'Física': 4, 'Química': 5} y")
print("después muestre por pantalla los créditos de cada asignatura en el formato <asignatura>")
print("tiene <créditos> créditos, donde <asignatura> es")
print("cada una de las asignaturas del curso, y <créditos> son sus créditos. Al final debe")
print("mostrar también el número total de créditos del curso.")
#Fin de las instrucciones
print(" ")#Espacio entre lineas 


materias_con_creditos = { #Se crea el diccionario con sus materias y sus creditos 
    'Matemáticas': 6,
    'Física': 4,
    'Química': 5
}

total_de_creditos = 0 #Se inicia el total de créditos 

#Nos mostrar los créditos de cada materia y nos calcula el total
for materia, creditos in materias_con_creditos.items():
    print(f"{materia} tiene {creditos} créditos.")
    total_de_creditos += creditos

#Nos muestra el total de credito 
print(f"El número total de créditos del curso es: {total_de_creditos}")


![image](https://github.com/user-attachments/assets/d1d113c1-41e7-4080-b22b-82cfb2a2252b)
![image](https://github.com/user-attachments/assets/f8cceb61-e0e7-4e02-9a94-832375b24f13)


# Codigo #3 Del Examen Del Segundo Parcial

print(" ")#Espacio entre lineas 
print("Nombre Del Alumno: Ramirez Torres Angel Manuel")#Nombre del alumno
print("Grado y Grupo: 3°W")#Grado y grupo del alumno
print("NO. De Control: 1206")#Muestra el numero de control
print(" ")#Espacio entre lineas
#Nos muestra a continuacion las instrucciones del programa a realizar 
print("-INSTRUCCIONES-")
print("Escribir un programa que almacene las")
print("asignaturas de un curso (por ejemplo Matemáticas, Física, Química, Historia y Lengua) ")
print("en una lista, pregunte al usuario la nota que ha sacado en cada")
print("asignatura, y después las muestre por pantalla con el mensaje En <asignatura> has sacado <nota> donde <asignatura> es")
print("cada una des las asignaturas de la lista y <nota> cada una de las correspondientes")
#Fin de las instrucciones
print(" ")#Espacio entre lineas }

# Lista de materias
materias = ["Matemáticas", "Física", "Química", "Historia", "Lengua"]

#Se crea un diccionario
calificaciones = {}#Almacena las calificaiones 

#Pregunta que calificacion es la que saco
i = 0
while i < len(materias):
    materia = materias[i]
    calificacion = float(input(f"Introduce la calificación que has sacado en {materia}: "))
    calificaciones[materia] = calificacion
    i += 1

#Nos mostra las calificaciones
for materia, calificacion in calificaciones.items():
    print(f"En {materia} has sacado {calificacion}")

![image](https://github.com/user-attachments/assets/7bb24a3b-36c9-48a5-ae34-a8b8659eb931)
![image](https://github.com/user-attachments/assets/5e3b176f-237e-4f8f-b8a6-80fcbbebcb2e)



# Codigo #4 Del Examen Del Segundo Parcial

print(" ")#Espacio entre lineas 
print("Nombre Del Alumno: Ramirez Torres Angel Manuel")#Nombre del alumno
print("Grado y Grupo: 3°W")#Grado y grupo del alumno
print("NO. De Control: 1206")#Muestra el numero de control
print(" ")#Espacio entre lineas
#Nos muestra a continuacion las instrucciones del programa a realizar 
print("-INSTRUCCIONES-")
print("Escribir un programa que pregunte al usuario su nombre, edad, dirección y")
print("teléfono y lo guarde en un diccionario. Después debe mostrar por pantalla el")
print("mensaje <nombre> tiene")
print("<edad> años, vive en <dirección> y su número de teléfono es")
print("<teléfono>.")
#Fin de las instrucciones
print(" ")#Espacio entre lineas 

# Crear un diccionario vacío 
persona = {}
# Solicitar y añadir el nombre
nombre = input("Introduce el nombre: ")  #introduzca su nombre
persona['nombre'] = nombre  #nombre al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido
print(" ")#crear un espacio entre lineas 

# Solicitar y añadir la edad
edad = input("Introduce la edad: ")  # Pide que introduzca su edad
persona['edad'] = edad  # Añade la edad al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido
print(" ")#crear un espacio entre lineas 

print(" ")#crear un espacio entre lineas 
# Solicitar y añadir la direccion
direccion = input("Introduce tu direccion: ")  # Pide que introduzca su direccion
persona['direccion'] = direccion  # Añade la direccion al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido
print(" ")#crear un espacio entre lineas 

print(" ")#crear un espacio entre lineas 
# Solicitar y añadir el teléfono
telefono = input("Introduce el teléfono: ")  # Pide que introduzca su teléfono
persona['telefono'] = telefono  # Añade el teléfono al diccionario
print("Contenido del diccionario:", persona)  # Muestra el contenido
print(" ")#crear un espacio entre lineas 

![image](https://github.com/user-attachments/assets/1f3a9412-e906-4a01-a6e7-7eeb1ce63827)
![image](https://github.com/user-attachments/assets/c62baa35-0c90-4139-b85c-c83a06006d0b)
![image](https://github.com/user-attachments/assets/c0d15d76-c247-4504-8bc4-ad00bf12b142)
