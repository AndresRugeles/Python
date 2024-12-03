# PANDAS

## Método shape
* Retorna una tupla y no lleva parénteses porque no es una función, sino una propiedad.
* Es solo de inspección, no altera el contenido del DataFrame ni de la Serie

## Método describe()
Para columnas numéricas

* Count: Número de valores no nulos.
* Mean: Media aritmética.
* Std: Desviación estándar.
* Min: Valor mínimo.
* 25% / 50% / 75%: Percentiles (cuartiles).
* Max: Valor máximo.

Para columnas categóricas: Si se utiliza con columnas de texto u objetos (o si se especifica include=['object']), genera:

* Count: Número de valores no nulos.
* Unique: Número de valores únicos.
* Top: Valor más frecuente.
* Freq: Frecuencia del valor más frecuente.

Configuraciones adicionales:
* include: Para especificar qué tipos de datos incluir ('all', ['number'], ['object'], etc.).
* exclude: Para excluir tipos de datos específicos. 

Ejemplo: `print(f'Resumen estadístico de las columnas numéricas o categóricas: \n {df.describe(include="all")}')`