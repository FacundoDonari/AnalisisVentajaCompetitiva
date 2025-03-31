Análisis de Ventaja Competitiva mediante Ratios Financieros

Metodología de Evalucion:

El análisis utiliza un conjunto de 21 ratios financieros clave para evaluar la presencia de ventajas competitivas
sostenibles en empresas cotizadas. La metodología combina métricas cuantitativas con criterios estructurados en forma de preguntas
binarias ("Tabla Conclucsiones en el archivo Excel") (Sí/No), permitiendo una evaluación objetiva de los fundamentales del negocio.


¿Cómo Funciona el Excel?
 
Este sistema automatizado evalúa si una empresa tiene una ventaja competitiva sostenible utilizando datos financieros históricos 
y una serie de ratios clave. El proceso se divide en 3 pasos principales:

1. Obtención de Datos (Automático con Python)
✅ Qué hace:

Usa un código en Python que, al ingresar el ticker de la empresa (ej: AAPL para Apple), descarga automáticamente:

▪ Balance General (activos, pasivos, patrimonio).

▪ Estado de Resultados (ventas, gastos, utilidades).

Los datos vienen en inglés y cubren los últimos 9 años.

Al final se genera un archivo Excel que luego se carga en la hoja "database" del informe.

🔹 Nota: Solo se ejecuta el código una vez por empresa.


2. Análisis Automático en Excel
✅ Qué hace:

Usa fórmula financieras y otras avanzadas como BUSCARV (VLOOKUP) para extraer datos especificos y asi calcular:

Crecimiento de ventas (¿suben consistentemente?).

Márgenes (bruto, operativo y neto).

Deuda vs. Patrimonio (¿la empresa está muy endeudada?).

Flujo de Caja Libre (¿genera dinero después de gastos?).

Rotaciones (inventario, activos, capital de trabajo).

Rentabilidad (ROIC, EVA, EPS).

📌 Cada ratio tiene un "target" (meta) que debe cumplir.
🔸 Ejemplo: Si el margen neto promedio de los últimos 9 años es menor al 20%, se marca como "No".



3. Evaluación Final: ¿Tiene Ventaja Competitiva?   (Conclsuiones en el Archivo)
✅ Qué hace:

Responde 21 preguntas clave (Sí/No) basadas en los ratios calculados.

Ejemplos de preguntas:

¿Las ventas crecieron al menos 9 años seguidos?

¿El margen neto supera el 20%?

¿La deuda equivale a un 50% que el patrimonio?

¿Genera flujo de caja libre consistentemente?



Composicion del Archivo:

El archivo cuenta con 3 Hojas. 

Primer hoja: En la hoja 'database' se encuentra cargados todos los balances y estados de resultados de la empresas que se pretenden analisar. Podrian ser empresas del mismo sector para hacer 
un analsiis especifico de una deeterminada indutria. En este caso a modo de ejemplo se cargaron empresas conocidas y de gran capitalizacion como son Apple, CocaCola, Microsoft
Amazon, Nvdia, Google, Meta y Tesla. Se extrajeorn los balances y estados de resultado de los utilmos 9 años de las empresas mencioanadas y se cargaron en esta hoja. 


Segunda Hoja: La hoja 'salida' es la que se usa para extraer los datos de la empresa especifica a analisar a traves de la formula 'BUSCARV', para que solo quede cargado en esta hoja los 
balances y estados de resultado de lo ultimos 9 años de una sola empresa, ademas se ajusto el fomrato para que se cargen de una forma especifica, por ejemplo que siempre el TotalRevenue
se carge en la fila 3 y el NetIncome en la fila 16, esto es muy importante, ya que permite aplicar las formulas financieras de forma consistente y sin importar que
empresa se escoja de la base de datos, siempre se aplicara las formulas sobre las mismas filas y en el caso mencioando se podria calcular el Margen Neto para cualquier empresa.

![Image](https://github.com/user-attachments/assets/76467e3f-f786-46ee-9470-8dc5e08503ac)



Tercer Hoja: La hoja 'ANALISIS DE VENTAJA COMPETITIVA', es donde se vuelcan los resultados. 
Lo primero que se ve es una lista validada en donde se ecuntran los ticker de las empresa que conforman la base de datos y se puede seleccionar la que se desea analisar. 

![Image](https://github.com/user-attachments/assets/e1f2ffa4-b15d-47fa-af2e-6665cd406725)




Tambien estan los ratios calculados del Balance General, de Estado de Resultado y Caluclos de Rentabilidad. AL final del cada ratio hay un resumen con los reusltados obtenidos
y un target (meta) a alcanzar con el que se compara. 

![Image](https://github.com/user-attachments/assets/3d3dc82c-0c6f-409c-9962-ec9c5f55ecb5)
