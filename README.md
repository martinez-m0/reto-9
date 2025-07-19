# reto-9
# promedio de un arreglo
    def promedio_arreglo(arr):
        if len(arr) == 0:
            return 0  # Evitar división por cero
        return sum(arr) / len(arr)

    # Ejemplo
    numeros = [4.5, 3.2, 6.7, 2.1]
    print("Promedio:", promedio_arreglo(numeros))

#  Producto punto de dos arreglos del mismo tamaño
    def producto_punto(arr1, arr2):
        if len(arr1) != len(arr2):
            raise ValueError("Los arreglos deben tener el mismo tamaño.")
        return sum(a * b for a, b in zip(arr1, arr2))

    # Ejemplo
    a = [1, 2, 3]
    b = [4, 5, 6]
    print("Producto punto:", producto_punto(a, b))  # 1×4 + 2×5 + 3×6 = 32

# mover ceros
    def mover_ceros_al_final(arr):
        no_ceros = [x for x in arr if x != 0]
        ceros = [0] * (len(arr) - len(no_ceros))
        return no_ceros + ceros

    # Ejemplo
    arreg lo = [0, 1, 0, 3, 12, 0, 5]
    print("Arreglo modificado:", mover_ceros_al_final(arreglo))

# bubble-sort
    def bubble_sort(lista):
        n = len(lista)  # Obtener la longitud de la lista
        for i in range(n):  # Repetir el proceso n veces
            for j in range(0, n - i - 1):  # Recorrer desde el inicio hasta el final "útil"
                if lista[j] > lista[j + 1]:  # Comparar elemento actual con el siguiente
                    # Si están en orden incorrecto, intercambiarlos
                    lista[j], lista[j + 1] = lista[j + 1], lista[j]
        return lista  # Devolver la lista ya ordenada

    # Lista de ejemplo
    numeros = [5, 3, 8, 4, 2]
    print("lisa original:", numeros)
  
    # Aplicar bubble_sort
    ordenada = bubble_sort(numeros)
  
    # Mostrar el resultado
    print("Lista ordenada:", ordenada)

# sorting
    # Ordenar lista en el lugar (modifica la original)
    lista = [5, 2, 9, 1]
    lista.sort()
  
    # Ordenar sin modificar la original (devuelve una nueva lista)
    nueva_lista = sorted([5, 2, 9, 1])

