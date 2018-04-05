# PR_LAB7_PROGRAMACION2_SETS
**Autor:** Luis Bravo  
**Curso:** 2017–2018  
**Asignatura:** Programación II — Laboratorio 7 (A.E.D.)

## Descripción
Este laboratorio implementa la clase `PositionListSet<E>` basada en listas posicionales (`PositionList<E>`), que cumple con la interfaz `Set<E>`.  
Se estudian las operaciones fundamentales de los conjuntos: inserción, eliminación, búsqueda, unión e intersección.

## Métodos principales
- `boolean add(E elem)`  
  Inserta un elemento si no existe en el conjunto.
- `boolean remove(E elem)`  
  Elimina un elemento si está presente.
- `boolean contains(Object o)`  
  Comprueba si el conjunto contiene un elemento.
- `Set<E> union(Set<E> s)`  
  Devuelve un nuevo conjunto con los elementos de ambos conjuntos.
- `Set<E> intersection(Set<E> s)`  
  Devuelve un nuevo conjunto con los elementos comunes.

## Condiciones
- No se permiten duplicados.
- Se admite el valor `null`.
- `union` e `intersection` no modifican los conjuntos originales.

## Ejemplo
```java
Set<Integer> a = new PositionListSet<>();
a.add(1); a.add(2);
Set<Integer> b = new PositionListSet<>();
b.add(2); b.add(3);

Set<Integer> u = a.union(b);        // u = {1, 2, 3}
Set<Integer> i = a.intersection(b); // i = {2}
```

## Archivos incluidos
- `Set.java` – Interfaz base.
- `PositionListSet.java` – Implementación con listas posicionales.
- `Tester.java` – Pruebas oficiales.
- `guia.pdf` – Guía del laboratorio.
- `Makefile`, `.project`, `.classpath`, `pom.xml`.

## Compilación y ejecución
```bash
mvn clean compile
mvn test
```

## Autor
— *Luis Bravo*
