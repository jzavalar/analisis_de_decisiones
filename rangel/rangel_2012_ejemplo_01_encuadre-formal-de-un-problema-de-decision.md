### Ejemplo 1: Encuadre Formal y Estructuración de un Problema de Decisión

#### 1. Contextualización del problema
Un propietario de una tienda de artículos deportivos enfrenta una situación administrativa característica de la gestión de inventarios estacionales. Cada mes de enero debe formalizar un pedido único de playeras de verano a su proveedor. Debido a los plazos de entrega, no existe la posibilidad de realizar ajustes o reposiciones posteriores. El reto analítico radica en determinar el volumen óptimo de pedido, equilibrando variables económicas conocidas (costos escalonados, precio de venta, valor de remate) con una incertidumbre inherente respecto a la demanda futura, bajo el objetivo de maximizar el beneficio neto.

#### 2. Identificación formal de los elementos del acto decisorio
Para transformar el escenario en un modelo cuantificable, se delimitan explícitamente los componentes estructurales conforme a los fundamentos de la teoría de decisiones:
* **Decisor:** El propietario de la tienda (sujeto con objetivos de rentabilidad y capacidad de elección).
* **Conjunto de acciones ($A = \{a_j\}$):** Cursos de acción bajo control directo del decisor. Dado que los pedidos se procesan en lotes de 100 prendas, el conjunto debe ser *exhaustivo* (agotar las opciones relevantes) y *exclusivo* (la selección de una excluye a las demás):
  * $a_1$: Ordenar 100 playeras.
  * $a_2$: Ordenar 200 playeras.
  * $a_3$: Ordenar 300 playeras.
* **Conjunto de estados de la naturaleza ($\Theta = \{\theta_i\}$):** Eventos futuros inciertos, ajenos al control del decisor, derivados de estimaciones de mercado:
  * $\theta_1$: Demanda de 100 playeras.
  * $\theta_2$: Demanda de 150 playeras.
  * $\theta_3$: Demanda de 200 playeras.
* **Función de consecuencias ($C_{ij}$):** Medida del beneficio neto (en unidades monetarias) asociada a cada par ordenado $(\theta_i, a_j)$.

#### 3. Modelado económico y condiciones lógicas
Se establecen los parámetros operativos que rigen la estructura de costos e ingresos:
* Precio de venta unitario ($P_v$): \$120.
* Costo unitario por escala de volumen ($C_u$): \$100 (para $a_1$), \$90 (para $a_2$), \$85 (para $a_3$).
* Precio de liquidación o remate ($P_r$): \$60.
* Pérdida por demanda insatisfecha ($L_g$): \$5 por unidad no entregada (costo de oportunidad por deterioro del buen nombre).

La función de consecuencias se formaliza mediante tres condiciones lógicas mutuamente excluyentes:
1. **Si la demanda iguala al pedido ($D = Q$):**  
   $C = D \times (P_v - C_u)$
2. **Si la demanda es menor al pedido ($D < Q$):**  
   $C = [D \times (P_v - C_u)] + [(Q - D) \times (P_r - C_u)]$
3. **Si la demanda supera al pedido ($D > Q$):**  
   $C = [Q \times (P_v - C_u)] - [L_g \times (D - Q)]$

#### 4. Demostración aritmética progresiva
A continuación, se calcula sistemáticamente cada celda de la matriz, aplicando la condición lógica correspondiente a cada intersección entre estado de la naturaleza y acción.

**Para la acción $a_1 ( C_u = 100 pesos)$:**  
- $\theta_1$ $(Demanda 100):$ $100$ $\times$ $(120 - 100) = 100$ $\times$ $20 =$ $\mathbf{2,000} pesos$  
- $\theta_2$ (Demanda 150): $[100 \times 20] - [5 \times (150 - 100)] = 2,000 - 250 = \mathbf{1,750} pesos$  
- $\theta_3$ (Demanda 200): $[100 \times 20] - [5 \times (200 - 100)] = 2,000 - 500 = \mathbf{1,500} pesos$  

**Para la acción $a_2 (C_u = 90 pesos)$:**  
- $\theta_1$ (Demanda 100): $[100 \times (120 - 90)] + [(200 - 100) \times (60 - 90)] = 3,000 + (100 \times -30) = \mathbf{0} pesos$  
- $\theta_2$ (Demanda 150): $[150 \times (120 - 90)] + [(200 - 150) \times (60 - 90)] = 4,500 + (50 \times -30) = \mathbf{3,000} pesos$  
- $\theta_3$ (Demanda 200): $200 \times (120 - 90) = 200 \times 30 = \mathbf{6,000} pesos$  

**Para la acción $a_3 (C_u = 85 pesos)$:**  
- $\theta_1$ (Demanda 100): $[100 \times (120 - 85)] + [(300 - 100) \times (60 - 85)] = 3,500 + (200 \times -25) = \mathbf{-1,500} pesos$  
- $\theta_2$ (Demanda 150): $[150 \times (120 - 85)] + [(300 - 150) \times (60 - 85)] = 5,250 + (150 \times -25) = \mathbf{1,500} pesos$  
- $\theta_3$ (Demanda 200): $[200 \times (120 - 85)] + [(300 - 200) \times (60 - 85)] = 7,000 + (100 \times -25) = \mathbf{4,500} pesos$  

#### 5. Matriz de pagos inicial
Respetando la convención notacional de la autora, donde las **filas representan los estados de la naturaleza ($\theta_i$)** y las **columnas representan las acciones ($a_j$)**, se integra la matriz de consecuencias (Ganancia en pesos):

| Estado de la naturaleza ($\theta_i$)\ Acción ($a_j$) | $a_1$ (100 pzas.) | $a_2$ (200 pzas.) | $a_3$ (300 pzas.) |
|:---|:---:|:---:|:---:|
| $\theta_1$: Demanda 100 | \$2,000 | \$0 | -\$1,500 |
| $\theta_2$: Demanda 150 | \$1,750 | \$3,000 | \$1,500 |
| $\theta_3$: Demanda 200 | \$1,500 | \$6,000 | \$4,500 |

#### 6. Principio de dominación
Conforme a lo establecido en la sección 1.6 del material base (Rangel, 2012), una acción se considera **inadmisible (dominada)** cuando los resultados de su implementación son sistemáticamente inferiores o iguales a los de otra alternativa en todos los estados de la naturaleza, siendo estrictamente inferiores en al menos uno. Para garantizar la eficiencia analítica, es imperativo depurar el espacio de soluciones antes de aplicar criterios de elección.

**Algoritmo sistemático de identificación de dominación (para problemas de maximización):**
1. **Selección de pares:** Comparar sistemáticamente cada par de acciones $(a_j, a_k)$ con $j \neq k$.
2. **Evaluación fila por fila:** Para cada estado de la naturaleza $\theta_i$, verificar si se cumple $C(\theta_i, a_j) \geq C(\theta_i, a_k)$.
3. **Conteo de superioridad:** 
   * Registrar si la igualdad o superioridad se mantiene en *todos* los renglones.
   * Registrar si existe al menos un renglón donde $C(\theta_i, a_j) > C(\theta_i, a_k)$.
4. **Determinación:** Si ambas condiciones se verifican, $a_j$ domina estrictamente a $a_k$ ($a_j \succ a_k$). La acción dominada $a_k$ se elimina de la matriz sin afectar la optimalidad del proceso.

#### 7. Aplicación del algoritmo y depuración matricial
Se aplica el protocolo al par $(a_2, a_3)$:

| Estado $\theta_i$ | $C($ $\theta_i$ $,$ $a_2$ $)$ | $C(\theta_i, a_3)$ | Evaluación ($a_2 \geq a_3$) | Evaluación ($a_2 > a_3$) |
|:---|:---:|:---:|:---:|:---:|
| $\theta_1$: Demanda 100 pzas | \$0 | -\$1,500 | ✓ | ✓ |
| $\theta_2$: Demanda 150 pzas | \$3,000 | \$1,500 | ✓ | ✓ |
| $\theta_3$: Demanda 200 pzas | \$6,000 | \$4,500 | ✓ | ✓ |

* **Resultado algorítmico:** La acción $a_2$ cumple con superioridad o igualdad en los tres estados, y estricta superioridad en los tres. Por lo tanto, $a_2$ $\succ$ $a_3$.
* **Conclusión:** La estrategia $a_3$ es inadmisible y se elimina del análisis.

#### 8. Matriz depurada para la toma de decisión
El espacio de soluciones queda reducido a las estrategias admisibles, listo para la aplicación de los criterios de decisión bajo incertidumbre o riesgo que se desarrollan en unidades subsiguientes:

| Estado de la naturaleza ($\theta_i$) \ Acción ($a_j$) | $a_1$ (100 pzas.) | $a_2$ (200 pzas.) |
|:---|:---:|:---:|
| $\theta_1$: Demanda 100 pzas | \$2,000 | \$0 |
| $\theta_2$: Demanda 150 pzas | \$1,750 | \$3,000 |
| $\theta_3$: Demanda 200 pzas | \$1,500 | \$6,000 |

Esta estructuración formal no solo garantiza la trazabilidad de cada consecuencia económica, sino que establece las bases epistemológicas necesarias para comprender por qué la teoría de decisiones exige la eliminación previa de alternativas ineficientes. La claridad en la delimitación de acciones, estados y funciones de consecuencias constituye el requisito indispensable para validar los resultados obtenidos mediante los distintos criterios de decisión.

#### 8. Referencias

Rangel Nafaile, L. M. (2012). *Guía de estudio de la asignatura Análisis de Decisiones* (1.ª ed.). México: Universidad Nacional Autónoma de México, Facultad de Estudios Superiores Acatlán.
