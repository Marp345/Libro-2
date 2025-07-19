## Libro de Estructura de Datos

---

📅 Fecha: *[18/6/2025]*  
📚 Docente: *[Fred torrez cruz]*  
🏫 Curso: *Estructura de Datos*
# Índice

- [Introducción](#introducción)
- [I. Operadores](#i-operadores)
- [II. Estructuras de Control](#ii-estructuras-de-control)
- [III. Funciones](#iii-funciones)
- [IV. Matrices](#iv-matrices)
- [V. Punteros y Referencias](#v-punteros-y-referencias)
- [VI. Operadores tipo & y *](#vi-operadores-tipo--y-)
- [VII. Entrada y Salida de Datos](#vii-entrada-y-salida-de-datos)
- [VIII. Tipos de Datos, Variables y Constantes](#viii-tipos-de-datos-variables-y-constantes)
- [IX. Comentarios y estructura de un programa](#ix-comentarios-y-estructura-de-un-programa)
- [X. Listas Enlazadas](#x-listas-enlazadas)
- [XI. Listas Doblemente Enlazadas](#xi-listas-doblemente-enlazadas)
- [XII. Listas Circulares](#xii-listas-circulares)
- [XIII. Colas](#xiii-colas)
- [XIV. Pilas](#xiv-pilas)
- [XV. Capitulos 1 al 5](#xv-cap-stl-1-5)
- [XVI. Recursión](#xvi-recursión)
- [XVII. Matrices (Avanzado)](#xvii-matrices-avanzado)
- [XVIII. Uso de Estructuras](#xviii-uso-de-estructuras)
- [XIX. Árboles Binarios](#xix-árboles-binarios)
- [XX. Árboles Binarios de Búsqueda (BST)](#xx-árboles-binarios-de-búsqueda-bst)
- [XXI. Árboles AVL](#xxi-árboles-avl)
- [XXII. Librerías y Cabeceras en C++](#xxii-librerías-y-cabeceras-en-c)
- [XXIII. Buenas Prácticas de Programación](#xxiii-buenas-prácticas-de-programación)
- [XXIV. Conclusión](#xxiv-conclusión)

# Índice con Definiciones y Ejemplos

## Introducción
La programación en C++ permite desarrollar aplicaciones de alto rendimiento. En este libro exploraremos las principales estructuras y fundamentos que todo programador debe conocer para dominar este lenguaje.

---

## I. Operadores

Los operadores son símbolos que le indican al compilador que realice operaciones matemáticas, lógicas o de asignación.

### Ejemplo:
```cpp
int a = 5, b = 3;
int suma = a + b;     // 8
int mult = a * b;     // 15
bool comp = a > b;    // true
```

---

## II. Estructuras de Control

Permiten alterar el flujo de ejecución de un programa: condicionales y bucles.

### Ejemplo:
```cpp
int edad;
cin >> edad;
if (edad >= 18) {
    cout << "Mayor de edad\n";
} else {
    cout << "Menor de edad\n";
}

for (int i = 0; i < 5; i++) {
    cout << i << " ";
}
```

---

## III. Funciones

Una función es un bloque de código reutilizable que realiza una tarea específica.

### Ejemplo:
```cpp
int suma(int a, int b) {
    return a + b;
}

int main() {
    cout << suma(3, 4); // 7
}
```

---

## IV. Matrices

Una matriz es una estructura bidimensional que permite almacenar datos en filas y columnas.

### Ejemplo:
```cpp
int mat[2][2] = {{1, 2}, {3, 4}};
cout << mat[0][1]; // 2
```

---

## V. Punteros y Referencias

Los punteros almacenan direcciones de memoria; las referencias actúan como alias de variables.

### Ejemplo:
```cpp
int a = 10;
int* p = &a; // puntero
int& ref = a; // referencia

cout << *p;  // 10
cout << ref; // 10
```

---

## VI. Operadores tipo & y *

`&` se usa para obtener direcciones de memoria y `*` para acceder a los valores apuntados.

### Ejemplo:
```cpp
int a = 5;
int* ptr = &a;

cout << &a << "\n"; // Dirección de a
cout << *ptr << "\n"; // Valor de a (5)
```

---

## VII. Entrada y Salida de Datos

Permiten interactuar con el usuario usando `cin`, `cout`, `scanf`, `printf`.

### Ejemplo:
```cpp
int x;
cin >> x;
cout << "Ingresaste: " << x << "\n";
```

---

## VIII. Tipos de Datos, Variables y Constantes

Los tipos definen el espacio de memoria; las constantes no cambian durante la ejecución.

### Ejemplo:
```cpp
int edad = 20;
float altura = 1.75;
const double PI = 3.1416;
```

---

## IX. Comentarios y estructura de un programa

Los comentarios ayudan a documentar el código. Todo programa tiene `main()` como punto de inicio.

### Ejemplo:
```cpp
#include <iostream> // Cabecera

using namespace std;

int main() {
    // Esto es un comentario
    cout << "Hola Mundo\n";
    return 0;
}
```

---

## X. Listas Enlazadas

Estructura donde cada nodo apunta al siguiente.

### Ejemplo:
```cpp
struct Nodo {
    int dato;
    Nodo* siguiente;
};

Nodo* cabeza = nullptr;
```

---

## XI. Listas Doblemente Enlazadas

Cada nodo tiene un puntero al siguiente y al anterior.

### Ejemplo:
```cpp
struct Nodo {
    int dato;
    Nodo* anterior;
    Nodo* siguiente;
};
```

---

## XII. Listas Circulares

La última posición apunta al inicio, formando un ciclo.

### Ejemplo:
```cpp
struct Nodo {
    int dato;
    Nodo* siguiente;
};

Nodo* cabeza = new Nodo{1, nullptr};
cabeza->siguiente = cabeza; // circular
```

---

## XIII. Colas

Estructura FIFO: primero en entrar, primero en salir.

### Ejemplo:
```cpp
#include <queue>
queue<int> q;
q.push(10);
q.push(20);
q.pop(); // Elimina el 10
```

---

## XIV. Pilas

Estructura LIFO: último en entrar, primero en salir.

### Ejemplo:
```cpp
#include <stack>
stack<int> s;
s.push(5);
s.push(8);
s.pop(); // Elimina el 8
```

---

<!-- Capítulo XV omitido para que el autor lo personalice -->

---

## XV Capitulos 1 al 5



## Ejercicio 1

### Código:
```cpp
#include <bits/stdc++.h>
using namespace std;

int main(){
    int a, b;
    int c, d;
    string m;
    string x;

    cin >> a >> b >> x;
    cout << a << " " << b << " " << x << endl;

    scanf("%d %d", &c, &d);
    printf("%d %d\n", c, d);

    getline(cin , m);
    cout << m;

    string p;
    while(cin >> p){
        cout << p << "\n";
    }
    return 0;
}
```
# ahora compilamos:
![alt text](<lo se-1.jpg>)
# la salida
![alt text](salida-1.jpeg)
## Ejercicio 2
```cpp
#include <bits/stdc++.h>
using namespace std;

int main(){
    int a = 123456;
    long long b = a * a;
    cout << b << "\n";

    //
    int m, n;
    cin >> n >> m;
    long long x = 1;
    for(int i = 1; i <= n; i++){
        x = (x * i) % m;
    }
    cout << x << "\n";

    //
    double o, l;
    cin >> o >> l;
    if(abs(o - l) < 1e-9){
        cout << "Iguales\n";
    } else {
        cout << "Diferentes\n";
    }

    return 0;
}
```
# Al compilar 
![alt text](image-4.png)
# Ejercicio 3
```cpp
#include <bits/stdc++.h>
using namespace std;

typedef long long ll;
typedef vector<int> vi;
typedef pair<int, int> pi;

#define F first
#define S second
#define PB push_back
#define MP make_pair
#define REP(i,a,b) for (int i = a; i <= b; i++)

int main() {
    ll a = 123456789, b = 987654321;
    cout << a * b << "\n";

    vi v;
    v.PB(1);
    v.PB(2);
    cout << v[0] << " " << v[1] << "\n";

    return 0;
}
```
# Al compilarlo
![alt text](image-5.png)

# Capitulo 2
 # Ejercicio 1
 ```cpp
#include <bits/stdc++.h>
using namespace std;

int n;
vector<int> subset;

void search(int k) {
    if (k == n + 1) {
        // Procesar el subconjunto
        cout << "{";
        for (size_t i = 0; i < subset.size(); i++) {
            cout << subset[i] << (i + 1 < subset.size() ? ", " : "");
        }
        cout << "}\n";
    } else {
        // Incluye k en el subconjunto
        subset.push_back(k);
        search(k + 1);

        // No incluye k en el subconjunto
        subset.pop_back();
        search(k + 1);
    }
}

int main() {
    cin >> n;
    search(1);
    return 0;
}
```
# Al compilarlo (si pones un numero alto, el resultado sera muy largo, asi que solo ponerlo de 1 a 3)
![alt text](image.png)

# Ejercicio 2
```cpp
#include <bits/stdc++.h>
using namespace std;

int n;
vector<int> permutation;
vector<bool> chosen;

void search() {
    if (permutation.size() == n) {
        for (int x : permutation) cout << x << " ";
        cout << "\n";
    } else {
        for (int i = 1; i <= n; i++) {
            if (chosen[i]) continue;
            chosen[i] = true;
            permutation.push_back(i);
            search();
            chosen[i] = false;
            permutation.pop_back();
        }
    }
}

int main() {
    cin >> n;
    chosen.assign(n + 1, false);
    search();
    return 0;
}
```
# Al compilarlo 
![alt text](image-1.png)

# Ejercicio 3
```cpp
#include <bits/stdc++.h>
using namespace std;

int n, count_solutions = 0;
vector<int> col, diag1, diag2;

void search(int y) {
    if (y == n) {
        count_solutions++;
        return;
    }
    for (int x = 0; x < n; x++) {
        if (col[x] || diag1[x + y] || diag2[x - y + n - 1]) continue;
        col[x] = diag1[x + y] = diag2[x - y + n - 1] = 1;
        search(y + 1);
        col[x] = diag1[x + y] = diag2[x - y + n - 1] = 0;
    }
}

int main() {
    cin >> n;
    col.assign(n, 0);
    diag1.assign(2 * n - 1, 0);
    diag2.assign(2 * n - 1, 0);
    search(0);
    cout << count_solutions << "\n";
    return 0;
}
```
# Al Compilar
![alt text](image-2.png)

# Capitulo 3

# Ejercicio 1
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int x = -43;
    unsigned int y = x;
    cout << x << "\n"; // -43
    cout << y << "\n"; // 4294967253 (en sistemas de 32 bits)
    return 0;
}
```
 # Al ejecutarlo
 ![alt text](image-3.png)
 # Ejercicio 1.2
 ```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int x = 2147483647;
    cout << x << "\n"; // 2147483647
    x++;
    cout << x << "\n"; // -2147483648 (overflow)
    return 0;
}
```
# Al ejecutarlo
![alt text](image-4.png)

# Ejercicio 2
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int x = 5328; // 00000000000000000001010011010000

    // Imprimir la representación binaria de x, 32 bits
    for (int k = 31; k >= 0; k--) {
        if (x & (1 << k)) cout << "1";
        else cout << "0";
    }
    cout << "\n";

    return 0;
}
```
 # al compilar el codigo 
 ![alt text](image-5.png)

 # Ejercicio 2.1 
 ```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int x = 5328; // binario: 00000000000000000001010011010000

    cout << __builtin_clz(x) << "\n";      // 19: ceros a la izquierda
    cout << __builtin_ctz(x) << "\n";      // 4: ceros a la derecha
    cout << __builtin_popcount(x) << "\n"; // 5: número de bits en 1
    cout << __builtin_parity(x) << "\n";   // 1: paridad (1 si número impar de bits en 1)

    return 0;
}
```
# Al ejecutarlo
![alt text](image-6.png)

# Ejercicio 3
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int x = 0;
    x |= (1 << 1); // Agrega el elemento 1
    x |= (1 << 3); // Agrega el elemento 3
    x |= (1 << 4); // Agrega el elemento 4
    x |= (1 << 8); // Agrega el elemento 8

    cout << __builtin_popcount(x) << "\n"; // Imprime el tamaño del conjunto (4)

    // Imprime los elementos que están en el conjunto
    for (int i = 0; i < 32; i++) {
        if (x & (1 << i))
            cout << i << " ";
    }
    cout << "\n"; // Salida: 1 3 4 8

    return 0;
}
```
# al ejecutar
![alt text](image-7.png)

# Ejercicio 3.1
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    // x = {1, 3, 4, 8}
    int x = (1 << 1) | (1 << 3) | (1 << 4) | (1 << 8);
    // y = {3, 6, 8, 9}
    int y = (1 << 3) | (1 << 6) | (1 << 8) | (1 << 9);

    // Unión: z = x ∪ y = {1, 3, 4, 6, 8, 9}
    int z = x | y;
    cout << __builtin_popcount(z) << "\n"; // 6

    // Intersección: x ∩ y
    int inter = x & y;
    cout << "Interseccion: ";
    for (int i = 0; i < 32; i++) {
        if (inter & (1 << i)) cout << i << " ";
    }
    cout << "\n";

    // Diferencia: x \ y
    int diff = x & (~y);
    cout << "Diferencia (x \\ y): ";
    for (int i = 0; i < 32; i++) {
        if (diff & (1 << i)) cout << i << " ";
    }
    cout << "\n";

    // Complemento de x (los elementos que NO están en x)
    int comp = ~x;
    cout << "Complemento de x (primeros 10 bits): ";
    for (int i = 0; i < 10; i++) {
        if (comp & (1 << i)) cout << i << " ";
    }
    cout << "\n";

    return 0;
}
```
# Al ejecutar
![alt text](image-8.png)

# Ejercicio 3.2
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    // x = {1, 3, 4, 8}
    int x = (1 << 1) | (1 << 3) | (1 << 4) | (1 << 8);
    int b = 0;
    do {
        cout << "Subconjunto: ";
        for (int i = 0; i < 32; i++) {
            if (b & (1 << i)) cout << i << " ";
        }
        cout << "\n";
    } while (b = (b - x) & x);
    return 0;
}
```
# AL EJECUTAR EL PROGRAMA
![alt text](image-9.png)

# Ejercicio 3.3
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    bitset<10> s;
    s[1] = 1;
    s[3] = 1;
    s[4] = 1;
    s[7] = 1;

    cout << s[4] << "\n"; // 1
    cout << s[5] << "\n"; // 0
    cout << s.count() << "\n"; // 4

    // Operaciones con bitsets
    bitset<10> a, b;
    a[1] = 1; a[2] = 1; a[5] = 1;
    b[2] = 1; b[3] = 1; b[5] = 1;

    bitset<10> c = a & b; // Intersección
    bitset<10> d = a | b; // Unión
    bitset<10> e = a ^ b; // Diferencia simétrica

    cout << "a: " << a << "\n";
    cout << "b: " << b << "\n";
    cout << "a & b: " << c << "\n";
    cout << "a | b: " << d << "\n";
    cout << "a ^ b: " << e << "\n";

    return 0;
}
```
# y ultimo al ejecutar este programa 
![alt text](image-10.png)

# VA DISCULPAR POR MANDAR MAL EL CAPITULO 2 EN SU HORA QUE DEJO :c

# Capitulo 4

## 📚 4.1.1 Ordenamiento Burbuja (Bubble Sort)

**Ordenamiento Burbuja** es un algoritmo de ordenamiento simple que funciona en tiempo \( O(n^2) \).  
El algoritmo consta de \( n \) rondas, y en cada ronda, itera a través de los elementos del arreglo.  
Siempre que se encuentran dos elementos consecutivos en el orden incorrecto, el algoritmo los intercambia.  
El algoritmo se puede implementar de la siguiente manera:

---

### 📈 Fig. 4.1 – Un arreglo antes y después del ordenamiento

| Arreglo original     | Arreglo ordenado     |
|----------------------|----------------------|
| `1 3 8 2 9 5 6`       | `1 2 3 5 6 8 9`       |

---

### 🔁 Fig. 4.2 – La primera ronda del ordenamiento burbuja

1. `1 3 8 2 9 5 6`
2. `1 3 2 8 9 5 6` ← Se intercambian 8 y 2  
3. `1 3 2 8 5 9 6` ← Se intercambian 9 y 5  
4. `1 3 2 8 5 6 9` ← Se intercambian 9 y 6  

---

### 💻 Código en C++ (Bubble Sort)

```cpp
#include <iostream>
#include <vector>
using namespace std;

void bubbleSort(vector<int>& array) {
    int n = array.size();
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n - 1; j++) {
            if (array[j] > array[j + 1]) {
                swap(array[j], array[j + 1]);
            }
        }
    }
}

int main() {
    vector<int> arr = {1, 3, 8, 2, 9, 5, 6};
    
    cout << "Arreglo original: ";
    for (int num : arr) cout << num << " ";
    cout << endl;
    
    bubbleSort(arr);
    
    cout << "Arreglo ordenado: ";
    for (int num : arr) cout << num << " ";
    cout << endl;
    
    return 0;
}
```
# al ejecutarlo
![alt text](image-6.png)

## 📚 4.1.2 Ordenamiento por Mezcla (Merge Sort)

Si queremos crear un algoritmo de ordenamiento eficiente, debemos ser capaces de reorganizar elementos que están en diferentes partes del arreglo.  
Hay varios algoritmos de ordenamiento que funcionan en \( O(n \log n) \) tiempo. Uno de ellos es **Merge Sort**, que se basa en la recursividad.  
Merge Sort ordena un subarreglo `array[a...b]` de la siguiente forma:

1. Si \( a = b \), no hacer nada, ya que un subarreglo con un solo elemento ya está ordenado.
2. Calcular la posición del elemento medio: `k = (a + b) / 2`.
3. Aplicar recursivamente el ordenamiento al subarreglo `array[a...k]`.
4. Aplicar recursivamente el ordenamiento al subarreglo `array[k + 1...b]`.
5. Mezclar los subarreglos ordenados `array[a...k]` y `array[k + 1...b]` en un subarreglo ordenado `array[a...b]`.

---

### 📊 Ejemplo

La **Figura 4.4** muestra cómo Merge Sort ordena un arreglo de ocho elementos:

| Arreglo original       | Arreglo ordenado       |
|------------------------|------------------------|
| `1 3 6 2 8 5 2 9`       | `1 2 2 3 5 6 8 9`       |

---


El algoritmo divide el arreglo en dos mitades de cuatro elementos, luego divide esas mitades en dos mitades de dos elementos, y así sucesivamente.  
Finalmente, fusiona los subarreglos ordenados en un arreglo completamente ordenado.

---

### 💻 Código en C++ 

```cpp
#include <iostream>
#include <vector>
using namespace std;

// Función para fusionar dos subarreglos ordenados
void merge(vector<int>& arr, int left, int mid, int right) {
    vector<int> leftSub(arr.begin() + left, arr.begin() + mid + 1);
    vector<int> rightSub(arr.begin() + mid + 1, arr.begin() + right + 1);

    int i = 0, j = 0, k = left;

    while (i < leftSub.size() && j < rightSub.size()) {
        if (leftSub[i] <= rightSub[j]) {
            arr[k++] = leftSub[i++];
        } else {
            arr[k++] = rightSub[j++];
        }
    }

    while (i < leftSub.size()) arr[k++] = leftSub[i++];
    while (j < rightSub.size()) arr[k++] = rightSub[j++];
}

// Función recursiva de merge sort
void mergeSort(vector<int>& arr, int left, int right) {
    if (left >= right) return;

    int mid = (left + right) / 2;
    mergeSort(arr, left, mid);
    mergeSort(arr, mid + 1, right);
    merge(arr, left, mid, right);
}

int main() {
    vector<int> arr = {1, 3, 6, 2, 8, 5, 2, 9};

    cout << "Arreglo original: ";
    for (int num : arr) cout << num << " ";
    cout << endl;

    mergeSort(arr, 0, arr.size() - 1);

    cout << "Arreglo ordenado: ";
    for (int num : arr) cout << num << " ";
    cout << endl;

    return 0;
}
```

# Al ejecutar
![alt text](image-7.png)

## 📉 4.1.3 Límite Inferior del Ordenamiento (Sorting Lower Bound)

¿Es posible ordenar un arreglo más rápido que en tiempo \( O(n \log n) \)?  
Resulta que esto **no es posible** si nos limitamos a algoritmos de ordenamiento basados en **comparación de elementos**.

El límite inferior para la complejidad temporal se puede demostrar considerando el proceso de ordenamiento como un árbol de decisiones, donde cada comparación entre dos elementos da más información sobre el contenido del arreglo. La **Figura 4.5** ilustra el árbol creado en este proceso.

> Aquí, `"x < y?"` significa que algunos elementos `x` y `y` son comparados.  
> - Si \( x < y \), el proceso continúa hacia la izquierda.  
> - Si no, hacia la derecha.  
>  
> Los resultados del proceso son las diferentes maneras posibles de ordenar el arreglo: **un total de \( n! \) formas**.  
> Por esta razón, la altura del árbol debe ser al menos:

\[
\log_2(n!) = \log_2(1) + \log_2(2) + \dots + \log_2(n)
\]

Podemos obtener una cota inferior para esta suma eligiendo los últimos \( n/2 \) elementos y reemplazando sus valores por \( \log_2(n/2) \), lo que da una estimación:

\[
\log_2(n!) \geq (n / 2) \cdot \log_2(n / 2)
\]

Así, la **altura del árbol** y el **peor caso** del número de pasos en cualquier algoritmo de ordenamiento basado en comparaciones es:

\[
\Omega(n \log n)
\]

---

### 4.1.4 Ordenamiento por Conteo (Counting Sort)

La cota inferior Ω(n log n) no se aplica a algoritmos que no comparan elementos del arreglo, sino que usan otro tipo de información. Un ejemplo de dicho algoritmo es el **ordenamiento por conteo** (counting sort), que ordena arreglos en tiempo O(n) asumiendo que cada elemento del arreglo es un número entero entre 0…c, y que c = O(n).

El algoritmo crea un arreglo auxiliar (bookkeeping array), cuyos índices son los elementos del arreglo original. El algoritmo recorre el arreglo original y calcula cuántas veces aparece cada elemento en el arreglo. Como ejemplo, la Figura 4.6 muestra un arreglo y el correspondiente arreglo auxiliar. Por ejemplo, el valor en la posición 3 es 2, porque el valor 3 aparece 2 veces en el arreglo original.

La construcción del arreglo auxiliar toma O(n) tiempo. Después de esto, el arreglo ordenado puede ser creado en tiempo O(n), ya que el número de ocurrencias de cada elemento puede ser recuperado desde el arreglo auxiliar. Por lo tanto, la complejidad temporal total del ordenamiento por conteo es **O(n)**.

El ordenamiento por conteo es un algoritmo muy eficiente, pero solo se puede usar cuando la constante **c** es lo suficientemente pequeña para que los elementos del arreglo puedan ser usados como índices en el arreglo auxiliar.
### 4.1.5 Ejemplo de ordenamientos en C++

```cpp
#include <iostream>
#include <vector>
#include <tuple>
#include <algorithm>
#include <string>

using namespace std;

// Comparador para strings: por longitud, luego alfabético
bool compString(string a, string b) {
    if (a.size() != b.size()) return a.size() < b.size();
    return a < b;
}

// Estructura con operador de comparación personalizado
struct Point {
    int x, y;
    bool operator<(const Point& p) const {
        if (y != p.y) return y < p.y;
        return x < p.x;
    }
}
```
# Un algoritmo de fuerza bruta revisa todos los pares de elementos en tiempo \( O(n^2) \):

```cpp
bool ok = true;
for (int i = 0; i < n; i++) {
    for (int j = i+1; j < n; j++) {
        if (array[i] == array[j]) ok = false;
    }
}
```
Sin embargo, podemos resolver el problema en tiempo 
𝑂
(
𝑛
log
⁡
𝑛
)
O(nlogn) si primero ordenamos el arreglo. Luego, si hay elementos iguales, estarán uno junto al otro en el arreglo ordenado, por lo que es fácil encontrarlos en tiempo 
𝑂
(
𝑛
)
O(n):

```cpp
bool ok = true;
sort(array, array+n);
for (int i = 0; i < n-1; i++) {
    if (array[i] == array[i+1]) ok = false;
}
```
## 4.2.1 Algoritmos de Línea de Barrido

Un algoritmo de *línea de barrido* modela un problema como un conjunto de eventos que se procesan en orden ordenado. Por ejemplo, supongamos que hay un restaurante y conocemos las horas de llegada y salida de todos los clientes que comen allí. Nuestra tarea es encontrar el número máximo de clientes que están en el restaurante al mismo tiempo.

Por ejemplo, la Figura 4.7 muestra un horario de intervalos para cuatro clientes: A, B, C y D. En este caso, el número máximo de clientes simultáneos es tres, cuando A, B y C están en el restaurante al mismo tiempo.

Para resolver el problema, almacenamos todos los eventos (la llegada y salida de cada cliente) en un arreglo y ordenamos esos eventos. Luego, recorremos los eventos y llevamos un contador de cuántos clientes hay en el restaurante. Si un evento es una llegada, incrementamos el contador; si es una salida, lo decrementamos. La respuesta al problema es el valor máximo que alcanza el contador durante el recorrido.

El algoritmo resultante funciona en tiempo \( O(n \log n) \), porque ordenar los eventos toma \( O(n \log n) \) y la parte de línea de barrido toma \( O(n) \).

Eventos ordenados:
Llegada(A), Llegada(B), Llegada(C), Salida(C), Salida(A), Llegada(D), Salida(B), Salida(D)

Contador a lo largo del recorrido:
# +1 (A) → 1
# +1 (B) → 2
# +1 (C) → 3 ← máximo
# -1 (C) → 2
# -1 (A) → 1
# +1 (D) → 2
# -1 (B) → 1
# -1 (D) → 0

## 4.2.2 Programación de Eventos (Scheduling Events)

Muchos problemas de programación pueden resolverse ordenando los datos de entrada y luego usando una estrategia voraz para construir una solución. Un algoritmo voraz siempre toma la decisión que parece la mejor en ese momento y nunca retrocede sobre sus elecciones.

Como ejemplo, consideremos el siguiente problema: Dados n eventos con sus tiempos de inicio y fin, encuentra un horario que incluya la mayor cantidad de eventos posible. Por ejemplo, la Fig. 4.9 muestra un ejemplo del problema donde una solución óptima es seleccionar dos eventos.

En este problema, hay varias formas en que podríamos ordenar los eventos de entrada. Una estrategia es ordenar los eventos según su duración y luego seleccionar los eventos más cortos primero. Sin embargo, esta estrategia no siempre funciona, como se muestra en la Fig. 4.10. Otra estrategia es ordenar los eventos por sus tiempos de inicio y siempre seleccionar el siguiente evento que comience más pronto. Esta también falla en algunos casos, como se muestra en la Fig. 4.11.

Una tercera idea es ordenar los eventos según su tiempo de finalización, y siempre seleccionar el primer evento que termine tan pronto como sea posible. Esta versión del algoritmo voraz siempre produce una solución óptima. Para justificar esto, consideremos lo que sucede si elegimos un evento que termina más tarde que otro evento disponible: en el mejor de los casos, tendremos la misma cantidad de opciones para seleccionar el próximo evento. Sin embargo, elegir un evento que termina más tarde nunca puede producir una mejor solución, y por tanto el algoritmo voraz es correcto.

## 4.2.3 Tareas y Fechas Límite (Tasks and Deadlines)

Finalmente, consideremos un problema donde se nos dan *n* tareas con duraciones y fechas límite, y nuestra tarea es elegir un orden para realizar las tareas. Por cada tarea, ganamos \( d - x \) puntos, donde \( d \) es la fecha límite de la tarea y \( x \) es el momento en el que la terminamos.

¿Cuál es el puntaje total más alto que se puede obtener?

Por ejemplo, supongamos que las tareas son las siguientes:

| Tarea | Duración | Fecha límite |
|-------|----------|---------------|
| A     | 4        | 2             |
| B     | 2        | 5             |
| C     | 3        | 7             |
| D     | 1        | 5             |

La **Figura 4.12** muestra una programación óptima de las tareas para este ejemplo. Usando ese orden (C, B, A, D):

- C rinde 6 puntos
- B rinde 5 puntos
- A rinde -7 puntos
- D rinde 2 puntos

En total se obtienen 6 puntos.

La solución correcta al problema no depende de las fechas límite en sí, sino que una buena estrategia voraz es simplemente ordenar las tareas por **duración creciente** y ejecutarlas en ese orden.

La razón de esto es que si realizamos una tarea más corta antes que otra más larga, el retraso de la tarea larga es menor. Si las tareas están fuera de orden, como se muestra en la **Figura 4.13**, donde hay dos tareas X e Y con duraciones \( a \) y \( b \), y \( a > b \), entonces el orden incorrecto puede generar más penalización. Al invertirlas, la penalización total disminuye en \( a - b \).

Por tanto, en una solución óptima, las tareas más cortas siempre deben preceder a las más largas. Es decir, ordenamos las tareas por duración.


**Solución en C++:**

```cpp
#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

typedef long long ll;

int main() {
    int n;
    cin >> n;
    vector<pair<ll, ll>> tasks(n);
    
    for (int i = 0; i < n; ++i) {
        cin >> tasks[i].first >> tasks[i].second; // duration, deadline
    }

    // Ordenamos por duración (greedy)
    sort(tasks.begin(), tasks.end());

    ll currentTime = 0;
    ll totalScore = 0;

    for (auto [duration, deadline] : tasks) {
        currentTime += duration;
        totalScore += (deadline - currentTime);
    }

    cout << totalScore << endl;

    return 0;
}
```
# al ejecutar
# 4
# 4 2
# 2 5
# 3 7
# 1 5

# 4.3.1 Implementando la búsqueda
Supongamos que se nos da una matriz ordenada de n elementos y queremos verificar si la matriz contiene un elemento con un valor objetivo. A continuación, discutimos dos formas de implementar un algoritmo de búsqueda binaria para este problema.

Primer método
La forma más común de implementar la búsqueda binaria se asemeja a buscar una palabra en un diccionario. La búsqueda mantiene un subarreglo activo en la matriz, que inicialmente contiene todos los elementos. Luego, cada paso reduce el tamaño del subarreglo activo a la mitad. En cada paso, se revisa el valor del elemento central del subarreglo. Si el valor coincide con el valor objetivo, se detiene la búsqueda. De lo contrario, la búsqueda continúa en la mitad izquierda o derecha del subarreglo, dependiendo del valor del elemento del medio. Por ejemplo, la Fig. 4.14 muestra una búsqueda de un valor 9 que se encuentra en la matriz.

La búsqueda puede implementarse de la siguiente manera:
 
```cpp
// Método 1: Búsqueda Binaria Tradicional
#include <iostream>
using namespace std;

int binarySearch(int array[], int n, int target) {
    int a = 0, b = n - 1;
    while (a <= b) {
        int k = (a + b) / 2;
        if (array[k] == target)
            return k; // encontrado
        else if (array[k] < target)
            a = k + 1; // buscar en la mitad derecha
        else
            b = k - 1; // buscar en la mitad izquierda
    }
    return -1; // no encontrado
}
```
# 4.3.2 Encontrando Soluciones Óptimas
Supongamos que estamos resolviendo un problema y tenemos una función valid(x) que devuelve true si x es una solución válida y false en caso contrario. Además, sabemos que:

valid(x) es falsa cuando x < k y verdadera cuando x ≥ k.

En esta situación, podemos usar búsqueda binaria para encontrar eficientemente el valor de x.

# La idea:
Buscar binariamente el mayor valor de x para el cual valid(x) es falsa. Entonces, el siguiente valor x + 1 será el menor valor posible para el cual valid(x) es verdadera.

# ejemplo
```cpp
#include <iostream>
#include <vector>
using namespace std;

// Función que determina si con 't' tiempo es posible procesar todos los trabajos
bool valid(long long t, const vector<int>& machines, int jobs) {
    long long total = 0;
    for (int time : machines) {
        total += t / time;
    }
    return total >= jobs;
}

long long minimumTimeToProcess(int jobs, const vector<int>& machines) {
    long long x = -1;
    long long b = 1;

    // Encontrar un límite superior inicial donde valid(x + b) sea verdadero
    while (!valid(x + b, machines, jobs)) {
        b *= 2;
    }

    // Búsqueda binaria para encontrar el mínimo t donde valid(t) sea verdadero
    for (; b >= 1; b /= 2) {
        while (!valid(x + b, machines, jobs)) {
            x += b;
        }
    }

    return x + 1;
}

int main() {
    int jobs = 7;
    vector<int> machines = {2, 3, 4}; // máquina 1: 2s, máquina 2: 3s, máquina 3: 4s

    long long minTime = minimumTimeToProcess(jobs, machines);
    cout << "El tiempo mínimo para procesar todos los trabajos es: " << minTime << endl;

    return 0;
}
```
# El ejecutar
![alt text](image-8.png)

# Capitulo 5

# 5.1.1 Vectores
Un vector es un arreglo dinámico que nos permite agregar y eliminar elementos de forma eficiente al final de la estructura. Podemos usar un vector para almacenar una lista de elementos. Por ejemplo, el siguiente código crea un vector vacío y agrega tres elementos:

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
    vector<int> v;
    v.push_back(3);      // agrega 3
    v.push_back(2);      // agrega 2
    v.push_back(5);      // agrega 5

    // Acceder a los elementos como si fuera un arreglo
    cout << v[0] << "\n"; // imprime 3
    cout << v[1] << "\n"; // imprime 2
    cout << v[2] << "\n"; // imprime 5

    return 0;
}
```
# Otra forma de crear un vector con una lista de elementos:
```cpp
vector<int> v = {2, 4, 2, 5, 1};
```
# Crear un vector con número de elementos e inicialización:
```cpp
vector<int> a(10);          // tamaño 10, todos con valor 0
vector<int> b(10, 42);      // tamaño 10, todos con valor 42
```
# Iterar sobre un vector usando índice:
```cpp
for (int i = 0; i < v.size(); i++) {
    cout << v[i] << " ";
}
```
# Forma más corta usando for-each (range-based for):
```cpp
for (auto x : v) {
    cout << x << " ";
}
```


### 5.1.2 Iterators and Ranges

Muchas funciones estándar de C++ usan iteradores (begin y end). Por ejemplo:

sort(v.begin(), v.end());
reverse(v.begin(), v.end());
random_shuffle(v.begin(), v.end());

Búsqueda binaria con iteradores:

auto it = lower_bound(v.begin(), v.end(), 5);

Eliminar duplicados:

sort(v.begin(), v.end());
v.erase(unique(v.begin(), v.end()), v.end());

### 5.1.3 Other Structures

**Deque:** permite inserciones y eliminaciones desde ambos extremos.

deque<int> d;
d.push_back(5);
d.push_front(3);
d.pop_back();

**Stack:** estructura LIFO (último en entrar, primero en salir).

stack<int> s;
s.push(2);
s.pop();
s.top(); // devuelve el último elemento

**Queue:** estructura FIFO (primero en entrar, primero en salir).

queue<int> q;
q.push(2);
q.pop();
q.front(); // primero
q.back();  // último

## 5.2 Set Structures

### 5.2.1 Sets and Multisets

Un `set` almacena elementos únicos ordenados.

set<int> s;
s.insert(3);
s.erase(3);
s.count(3); // 0 si no está, 1 si está

Un `multiset` permite elementos repetidos.

multiset<int> ms;
ms.insert(5);
ms.erase(ms.find(5)); // elimina uno solo
ms.count(5);

También están disponibles:

s.find(x);
s.lower_bound(x);
s.upper_bound(x);

### 5.2.2 Maps

Los mapas asocian claves con valores.

map<string,int> m;
m["cat"] = 5;
cout << m["cat"] << "\n"; // 5

`map` tiene complejidad O(log n), mientras que `unordered_map` tiene O(1) en promedio.

### 5.2.3 Priority Queues

Una cola de prioridad por defecto devuelve el mayor elemento primero.

priority_queue<int> q;
q.push(3);
q.push(5);
cout << q.top() << "\n"; // 5
q.pop();

Para obtener el menor primero:

priority_queue<int, vector<int>, greater<int>> q;

### 5.2.4 Policy-Based Sets

Estructura especial que permite operaciones adicionales:

#include <ext/pb_ds/assoc_container.hpp>
using namespace __gnu_pbds;

typedef tree<int, null_type, less<int>, rb_tree_tag,
    tree_order_statistics_node_update> indexed_set;

indexed_set s;
s.insert(2);
s.insert(3);
*s.find_by_order(1);    // segundo elemento más pequeño (3)
s.order_of_key(3);      // cuántos elementos menores que 3

## 5.3 Experiments

### 5.3.1 Set Versus Sorting

Para calcular cuántos elementos únicos hay:

- `set`: O(n log n)
- `unordered_set`: O(n)
- `sort + unique`: O(n log n), pero en la práctica el más rápido

| Tamaño | set (s) | unordered_set (s) | sort (s) |
|--------|---------|-------------------|----------|
| 1e6    | 0.65    | 0.34              | 0.11     |
| 2e6    | 1.50    | 0.76              | 0.18     |

### 5.3.2 Map Versus Array

Problema: encontrar el valor que más aparece en un array.

Soluciones:
- `map`: flexible, pero más lento
- `unordered_map`: más rápido
- `array` (si el rango es pequeño): mucho más rápido

| Tamaño | map (s) | unordered_map (s) | array (s) |
|--------|---------|-------------------|-----------|
| 1e6    | 0.55    | 0.23              | 0.01      |
| 2e6    | 1.14    | 0.39              | 0.02      |

### 5.3.3 Priority Queue Versus Multiset

Para acceder al elemento máximo o mínimo:

- `priority_queue`: muy eficiente (heap)
- `multiset`: más versátil pero más lento

# Ejercicios
# Capítulo 5: Data Structures - Ejercicios Prácticos

---

## 5.1.1 Vectors

**Ejercicio:** Lee `n` enteros, almacénalos en un `vector`, y muestra el mayor elemento.

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    int n, x;
    cin >> n;
    vector<int> v;
    for (int i = 0; i < n; i++) {
        cin >> x;
        v.push_back(x);
    }
    cout << *max_element(v.begin(), v.end()) << "\n";
}
```
# al ejecutar
![alt text](image-9.png)

# 5.1.2 Iterators and Ranges
Resumen: Los iteradores permiten usar funciones estándar como sort, reverse, unique.

Ejercicio: Leer n números, eliminar duplicados y mostrar los únicos ordenados.
```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    int n, x;
    cin >> n;
    vector<int> v;
    for (int i = 0; i < n; i++) {
        cin >> x;
        v.push_back(x);
    }

    sort(v.begin(), v.end());
    v.erase(unique(v.begin(), v.end()), v.end());

    for (int x : v) {
        cout << x << " ";
    }
}
```
# al ejecutar
![alt text](image-10.png)

# 5.1.3 Stack y Queue
Resumen: stack y queue permiten operaciones eficientes en los extremos de la estructura.

Ejercicio: Insertar números impares al frente y pares al final de una cola.
```cpp
#include <iostream>
#include <deque>
using namespace std;

int main() {
    int n, x;
    cin >> n;
    deque<int> dq;
    for (int i = 0; i < n; i++) {
        cin >> x;
        if (x % 2 == 0) dq.push_back(x);
        else dq.push_front(x);
    }

    while (!dq.empty()) {
        cout << dq.front() << " ";
        dq.pop_front();
    }
}
```
# al ejecutar 
![alt text](image-11.png)
# 5.2.1 Sets and Multisets
Resumen: set almacena elementos únicos ordenados, multiset permite duplicados.

Ejercicio: Leer n enteros y mostrar cuántos son únicos.
```cpp
#include <iostream>
#include <set>
using namespace std;

int main() {
    int n, x;
    cin >> n;
    set<int> s;
    for (int i = 0; i < n; i++) {
        cin >> x;
        s.insert(x);
    }
    cout << s.size() << "\n";
}
```

# 5.2.2 Maps
Resumen: map asocia claves con valores; útil para contar, indexar, etc.

Ejercicio: Contar cuántas veces aparece cada palabra.          

```cpp
#include <iostream>
#include <map>
using namespace std;

int main() {
    int n;
    string word;
    map<string, int> freq;

    cin >> n;
    for (int i = 0; i < n; i++) {
        cin >> word;
        freq[word]++;
    }

    for (auto p : freq) {
        cout << p.first << ": " << p.second << "\n";
    }
}
```
# 5.2.3 Priority Queues
Resumen: priority_queue permite obtener el mayor (o menor) elemento en O(log n).

Ejercicio: Mostrar los k mayores elementos de una lista.
```cpp
#include <iostream>
#include <queue>
using namespace std;

int main() {
    int n, k, x;
    cin >> n >> k;
    priority_queue<int> pq;

    for (int i = 0; i < n; i++) {
        cin >> x;
        pq.push(x);
    }

    for (int i = 0; i < k; i++) {
        cout << pq.top() << " ";
        pq.pop();
    }
}
```
# 5.3.1 Set Versus Sorting
Resumen: Diferentes formas de eliminar duplicados tienen rendimientos muy distintos.

Ejercicio: Comparar tiempos entre set y sort+unique.
 
```cpp 
#include <iostream>
#include <set>
#include <vector>
#include <algorithm>
#include <chrono>
using namespace std;
using namespace std::chrono;

int main() {
    int n = 1e6;
    vector<int> v(n);
    for (int i = 0; i < n; i++) v[i] = rand() % 1000000;

    auto start = high_resolution_clock::now();
    set<int> s(v.begin(), v.end());
    auto stop = high_resolution_clock::now();
    cout << "Set size: " << s.size() << "\n";
    cout << "Time (set): " << duration_cast<milliseconds>(stop - start).count() << "ms\n";

    start = high_resolution_clock::now();
    sort(v.begin(), v.end());
    v.erase(unique(v.begin(), v.end()), v.end());
    stop = high_resolution_clock::now();
    cout << "Unique sorted size: " << v.size() << "\n";
    cout << "Time (sort+unique): " << duration_cast<milliseconds>(stop - start).count() << "ms\n";
}

## XVI. Recursión

Una función se llama a sí misma.

### Ejemplo:
```cpp
int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);
}
```

---

## XVII. Matrices (Avanzado)

Manejo dinámico, multiplicación, transposición, etc.

### Ejemplo:
```cpp
vector<vector<int>> matriz(3, vector<int>(3, 0));
matriz[1][2] = 9;
```

---

## XVIII. Uso de Estructuras

Permiten agrupar datos bajo una sola entidad.

### Ejemplo:
```cpp
struct Estudiante {
    string nombre;
    int edad;
};

Estudiante e = {"Juan", 20};
```

---

## XIX. Árboles Binarios

Estructura jerárquica con un nodo raíz, y dos hijos como máximo.

### Ejemplo:
```cpp
struct Nodo {
    int valor;
    Nodo* izq;
    Nodo* der;
};
```

---

## XX. Árboles Binarios de Búsqueda (BST)

Árbol binario donde el hijo izquierdo < raíz < hijo derecho.

### Ejemplo:
```cpp
void insertar(Nodo*& raiz, int val) {
    if (!raiz) raiz = new Nodo{val, nullptr, nullptr};
    else if (val < raiz->valor) insertar(raiz->izq, val);
    else insertar(raiz->der, val);
}
```

---

## XXI. Árboles AVL

BST auto-balanceado para mantener eficiencia log(n).

### Ejemplo:
```cpp
// Se usan rotaciones: simple, doble izquierda/derecha (implementación avanzada)
```

---

## XXII. Librerías y Cabeceras en C++

Son archivos que contienen funciones ya implementadas.

### Ejemplo:
```cpp
#include <iostream>
#include <vector>
#include <cmath>
```

---

## XXIII. Buenas Prácticas de Programación

- Usa nombres descriptivos.
- Comenta tu código.
- Evita código duplicado.
- Sigue una indentación clara.

---

## XXIV. Conclusión

C++ es un lenguaje poderoso que combina eficiencia y control. Dominar sus estructuras fundamentales es esencial para resolver problemas complejos de manera eficiente.

![alt text](image-12.png)

```markdown
# CAPÍTULO x 
ÁRBOLES BALANCEADOS Y SUS VARIANTES

---

Este capítulo presenta diferentes estructuras de árboles balanceados fundamentales para mantener operaciones eficientes como búsqueda, inserción y eliminación. Se cubren los siguientes tipos:

- Árbol AVL  
- Árbol B / B+  
- Árbol Heap  
- Árbol Rojo-Negro  

---

## X.1 Árbol AVL

Los **árboles AVL** son árboles binarios de búsqueda auto-balanceados. Tras cada operación de inserción o eliminación, se verifica y ajusta el equilibrio del árbol mediante rotaciones. El nombre proviene de sus creadores: Adelson-Velsky y Landis.

### X.1.1 Propiedades del árbol AVL

- El **factor de equilibrio** (altura izquierda - altura derecha) de cualquier nodo es -1, 0 o 1.  
- Si un nodo se desequilibra, se aplica una **rotación** para restablecer el equilibrio.  

### X.1.2 Rotaciones

Existen cuatro tipos principales de rotaciones:

- **LL**: Rotación simple a la derecha.  
- **RR**: Rotación simple a la izquierda.  
- **LR**: Rotación doble izquierda-derecha.  
- **RL**: Rotación doble derecha-izquierda.

```pseudo
1) algoritmo RotarDerecha(y)
2)     x ← y.izquierda
3)     T2 ← x.derecha
4)     x.derecha ← y
5)     y.izquierda ← T2
6)     actualizarAltura(y)
7)     actualizarAltura(x)
8)     retornar x
9) fin RotarDerecha
```

### X.1.3 Inserción

```pseudo
1) algoritmo InsertarAVL(nodo, valor)
2)     si nodo = ∅
3)         retornar nuevoNodo(valor)
4)     si valor < nodo.valor
5)         nodo.izquierda ← InsertarAVL(nodo.izquierda, valor)
6)     sino si valor > nodo.valor
7)         nodo.derecha ← InsertarAVL(nodo.derecha, valor)
8)     sino
9)         retornar nodo // No se permiten duplicados
10)    actualizarAltura(nodo)
11)    balance ← obtenerBalance(nodo)
12)    si balance > 1 y valor < nodo.izquierda.valor
13)        retornar RotarDerecha(nodo) // LL
14)    si balance < -1 y valor > nodo.derecha.valor
15)        retornar RotarIzquierda(nodo) // RR
16)    si balance > 1 y valor > nodo.izquierda.valor
17)        nodo.izquierda ← RotarIzquierda(nodo.izquierda)
18)        retornar RotarDerecha(nodo) // LR
19)    si balance < -1 y valor < nodo.derecha.valor
20)        nodo.derecha ← RotarDerecha(nodo.derecha)
21)        retornar RotarIzquierda(nodo) // RL
22)    retornar nodo
23) fin InsertarAVL
```
## ✅ Ejemplo de Árbol AVL

Insertamos los valores: `10, 20, 30`

1. Insertamos 10 →  
```
10
```

2. Insertamos 20 →  
```
  10
    \
    20
```

3. Insertamos 30 → Se produce desbalance (caso RR), se realiza rotación izquierda:

```
   20
  /  \
10   30
```

El árbol queda balanceado después de la rotación.

---
---

## X.2 Árbol B

Los **árboles B** son árboles m-arios balanceados utilizados principalmente en sistemas de bases de datos y archivos. Son altamente eficientes para almacenamiento externo (disco).

### X.2.1 Propiedades

- Cada nodo contiene hasta *m - 1* claves y *m* hijos.  
- Todas las hojas están al mismo nivel.  
- Las claves dentro de cada nodo están ordenadas.  
- La inserción, búsqueda y eliminación son **O(log n)**.

### X.2.2 Inserción en Árbol B

```pseudo
1) algoritmo InsertarB(raíz, clave)
2)     si raíz está llena
3)         s ← nuevoNodo()
4)         s.hijos[0] ← raíz
5)         DividirHijo(s, 0)
6)         InsertarNoLleno(s, clave)
7)         retornar s
8)     sino
9)         InsertarNoLleno(raíz, clave)
10)    retornar raíz
11) fin InsertarB
```
## ✅ Ejemplo de Árbol B (orden 3)

Insertamos los valores: `10, 20, 5, 6, 12`

1. Insertamos 10, 20 →  
```
[10, 20]
```

2. Insertamos 5 →  
```
[5, 10, 20]
```

3. Insertamos 6 → nodo se divide:

```
        [10]
       /    \
 [5,6]      [20]
```

4. Insertamos 12 → se acomoda en el nodo derecho:

```
        [10]
       /    \
 [5,6]     [12,20]
```

---
---

## X.3 Árbol B+

El **árbol B+** es una mejora del árbol B, ideal para consultas de rango. Su estructura optimiza el recorrido de los datos.

### X.3.1 Diferencias clave con B

- Las **claves reales** solo están en las **hojas**.  
- Los **nodos internos** actúan como índices.  
- Las hojas están **enlazadas horizontalmente** para recorridos rápidos.

### X.3.2 Búsqueda

```pseudo
1) algoritmo BuscarBPlus(nodo, clave)
2)     si nodo es hoja
3)         retornar nodo si clave ∈ nodo.claves
4)     sino
5)         encontrar índice i tal que clave < claves[i]
6)         retornar BuscarBPlus(nodo.hijos[i], clave)
7) fin BuscarBPlus
```
## ✅ Ejemplo de Árbol B+ (orden 3)

Insertamos: `5, 10, 15, 20, 25`

Estructura final:

```
          [15]
         /    \
 [5,10]        [15,20,25]
```

- Las hojas contienen **todos los datos reales**.
- Las hojas están **enlazadas** para recorridos:

```
[5,10] —→ [15,20,25]
```

Este árbol es eficiente para búsquedas y consultas por rango.

---
---

## X.4 Árbol Heap (Montículo)

Un **heap** es una estructura basada en árboles binarios completos donde se conserva una propiedad de orden:

- **Min-Heap**: el valor del padre es menor o igual a sus hijos.  
- **Max-Heap**: el valor del padre es mayor o igual a sus hijos.  

Se implementa eficientemente mediante **arreglos lineales**.

### X.4.1 Fórmulas de índice en arreglo

- Padre(i) = (i - 1) / 2  
- HijoIzq(i) = 2i + 1  
- HijoDer(i) = 2i + 2

### X.4.2 Inserción en Min-Heap

```pseudo
1) algoritmo InsertarHeap(heap, valor)
2)     heap.agregar(valor)
3)     i ← índice de último
4)     mientras i > 0 y heap[i] < heap[Padre(i)]
5)         intercambiar(heap[i], heap[Padre(i)])
6)         i ← Padre(i)
7)     fin mientras
8) fin InsertarHeap
```

### X.4.3 Eliminación del mínimo

```pseudo
1) algoritmo ExtraerMin(heap)
2)     si heap está vacío retornar ∅
3)     min ← heap[0]
4)     heap[0] ← heap[último]
5)     eliminar último
6)     i ← 0
7)     mientras hijo válido y heap[i] > heap[hijo_menor(i)]
8)         intercambiar(heap[i], heap[hijo_menor(i)])
9)         i ← hijo_menor(i)
10)    fin mientras
11)    retornar min
12) fin ExtraerMin
```
## ✅ Ejemplo de Heap (Min-Heap)

Insertamos los valores: `40, 30, 50, 10, 20`

Construcción paso a paso:

1. Insertamos 40  
2. Insertamos 30 → sube  
3. Insertamos 50  
4. Insertamos 10 → sube hasta raíz  
5. Insertamos 20 → sube sobre 30

Resultado final (árbol):

```
        10
       /  \
     20    50
    /  \
  40   30
```

El elemento mínimo (10) siempre se encuentra en la raíz.

---
---

## X.5 Árbol Rojo-Negro

Los **árboles rojo-negro** son árboles binarios de búsqueda balanceados mediante propiedades de color. Su rendimiento es cercano al de AVL, pero con menor costo en rotaciones.

### X.5.1 Reglas

1. Cada nodo es rojo o negro.  
2. La raíz es negra.  
3. Un nodo rojo no puede tener hijos rojos.  
4. Cada camino desde un nodo a una hoja contiene el mismo número de nodos negros.

### X.5.2 Inserción

```pseudo
1) algoritmo InsertarRB(raíz, nodo)
2)     insertar como en BST
3)     nodo.color ← ROJO
4)     mientras nodo ≠ raíz y nodo.padre.color = ROJO
5)         si nodo.padre es hijo izquierdo
6)             tío ← nodo.padre.padre.derecho
7)             si tío.color = ROJO
8)                 recolorear padre, tío y abuelo
9)             sino
10)                si nodo = nodo.padre.derecha
11)                    nodo ← nodo.padre
12)                    rotarIzquierda(nodo)
13)                rotarDerecha(nodo.padre.padre)
14)                intercambiar colores
15)         sino
16)             // Casos simétricos
17)     raíz.color ← NEGRO
18) fin InsertarRB
```
## ✅ Ejemplo de Árbol Rojo-Negro

Insertamos los valores: `10, 20, 30`

1. Insertamos 10 → raíz, se pinta **negro**  
2. Insertamos 20 → hijo rojo  
3. Insertamos 30 → se produce violación de regla (dos rojos seguidos)

Se aplica **rotación izquierda** y **recoloración**

Resultado final:

```
     20 (negro)
    /     \
10 (rojo) 30 (rojo)
```

El árbol mantiene las propiedades rojo-negro:

- Raíz negra  
- No hay rojos consecutivos  
- Igual número de nodos negros en todos los caminos


```
---

## X.6 Resumen comparativo

| Tipo de Árbol    | Altura Balanceada | Inserción  | Eliminación | Búsqueda  | Uso común                             |
|------------------|-------------------|------------|-------------|-----------|----------------------------------------|
| AVL              | Muy estricta      | O(log n)   | O(log n)    | O(log n)  | Búsqueda en memoria, rendimiento alto |
| B                | Moderada          | O(log n)   | O(log n)    | O(log n)  | Bases de datos, discos                 |
| B+               | Moderada          | O(log n)   | O(log n)    | O(log n)  | Consultas por rango, índices           |
| Heap             | No ordenado       | O(log n)   | O(log n)    | O(n)      | Colas de prioridad, algoritmos greedy  |
| Rojo-Negro       | Equilibrio flexible| O(log n)  | O(log n)    | O(log n)  | Set/map en lenguajes como Java o C++  |

---

**Conclusión:**  
Cada tipo de árbol balanceado tiene ventajas específicas. El AVL ofrece máxima velocidad para búsquedas, el B/B+ optimiza el almacenamiento externo, el Heap es ideal para prioridades, y el Rojo-Negro ofrece balance eficiente con menos rotaciones. La elección correcta depende de la aplicación.
```

