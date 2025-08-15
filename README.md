# agenda.py

def agregar_contacto(nombre, celular):
    with open("contactos.txt", "a") as archivo:
        archivo.write(f"{nombre},{celular}\n")
    print("Contacto agregado correctamente.")

# Ejemplo de uso
nombre = input("Ingrese el nombre: ")
celular = input("Ingrese el número de celular: ")
agregar_contacto(nombre, celular)
