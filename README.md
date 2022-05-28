# Estadistica Multivariada Avanzada

## Predicción de Demanda y Oferta de Energía

#### Profesores:

Tomas Olarte

Santiago Hernández

#### Estudiantes:

Sarah Henao

Julián Herrera

### Problema

Se tienen datos de la demanda y la oferta o generación de energía del sistema interconectado nacional colombiano (SIN). Por medio de estas variables, que son series de tiempo en esencia, se busca predecir cual será la demanda y predecir cual será la generación de energía de tipo renovable (hidráulica, eólica, solar) para así poder determinar cuanta energía no renovable será necesaria a futuro. El problema nace de la necesidad de determinar para un determinado momento cual será estos dos valores y poder anticiparse, ya que la producción de energía no renovable (termina y por generadores) tiene un tiempo de operación que debe considerarse.

Sin embargo, también se cuenta con información de la generación de energía no renovable, por tanto surge la pregunta de ¿por qué no predecir la generación no renovable?, y la respuesta es que la producción de esta depende de la demanda y de la generación de energía renovable, ya que en primera instancia se busca cubrir la demanda con la generación renovable, pero esta tiene limites (no controlables como las precipitaciones, los vientos, la nubosidad, etc), y lo faltante por tanto se cubre con energía no renovable. Ahora bien, ¿por qué no construir un modelo para la generación de energía no renovable utilizando las otras dos como entradas? esto es porque al momento en que se tiene el valor real de estas variables es muy tarde para poder hacer algo frente a la energía no renovable, por lo que es necesario anticiparse.

Así entonces, el trabajo consiste en predecir demanda y generación renovable, de tal manera que, si estos modelos son satisfactorios entonces mediante la resta de ambas (demanda - generación renovable) se obtendrá el valor futuro de energía no renovable que debe producirse. Entonces, la métrica de evaluación se aplicará a las predicciones de demanda y generación, las cuales serán Error Cuadrático Medio Promedio (MAPE) y Error Cuadrático Medio (MAE).

### Funcionamiento

En la carpeta src se encuentran los Notebooks de Jupyter con los modelos y datos requeridos.
