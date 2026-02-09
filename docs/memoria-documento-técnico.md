# Memoria de Proyecto: World Happiness Report

Resultado del Análisis Exploratorio de Datos de los índices utilizados en la publicación del Work Happiness Report y sus resultados.

## Índice

-  [Preambulo: El contexto de los datos](#preambulo-el-contexto-de-los-datos)

- [1. Campos y categorías](#1-campos-y-categorías)

- [2. Patrones generales](#2-patrones)

- [3. Análisis Exploratorio de Datos (EDA)](#3-análisis-exploratorio-de-datos-eda)

- [4. Cambios ejecutados](#4-cambios-ejecutados)

- [5. Nuestras cuestiones sobre los datos](#5-nuestras-cuestiones-sobre-los-datos)

- [6. Visualización como respuesta](#6-visualización-como-respuesta)

- [7. Nuestra propuesta de valor](#7-propuesta-de-valor)

- [8. Next Steps: vistas a futuro](#8-next-steps-vistas-a-futuro)

---
---

## Preambulo: el contexto de los datos

### World Happiness Report: ¿Cuándo, cómo y dónde surge esta iniciativa?


El WHR usa una base de muestreo ya existente por iniciativa de Gallup INC.

El grupo Gallup es una empresa privada estadounidense que recibe encargos de cualquier tipo de naturaleza para conducir sus estudios sociales y de mercado.

En 2005, Gallup inicia su Encuesta Mundial (**World Poll**), a ciudadanos de 160 países: la intención es representar a más del 98 % de la población adulta mundial. La *World Poll* se usa de base para inferir el valor de ciertos campos en lo que luego será el *World Happiness Report*, que exisirá como iniciativa separada a partir de 2012.

La *World Poll* de Gallup incluye más de 100 preguntas globales, además de ítems específicos por región.

### 2012: el primer World Happiness Report

Se publica el 1 de abril de 2012, como documento base para la Reunión de Alto Nivel de la ONU sobre *Bienestar y Felicidad: Definiendo un Nuevo Paradigma Económico*.

Al día siguiente, el 2 de abril de 2012, tuvo lugar la reunión, presidida por el entonces secretario general de la ONU, Ban Ki-moon, y el primer ministro de Bután, Jigme Thinley, país que adoptó la felicidad nacional bruta (en lugar del PIB) como principal indicador de desarrollo.

[Aquí el enlace de lo publicado sobre la reunión de 2012 respecto al ejemplo de Bután.](617BhutanReport_WEB_F.pdf)


## 1. Campos y categorías

La  [fuente primaria de datos](/data/raw/World_Happiness_Report.csv) para este proyecto de análisis presenta los siguientes campos como índices:

- [Nombre del país](#country-name)

- [Indicador regional a nivel global](#regional-indicator)

- [Año](#year)

- [Satisfacción vital](#life-ladder)

- [PIB per cápita en logaritmo natural](#log-gdp-per-capita)

- [Soporte social](#social-support)

- [Expectativa de vida al nacer](healthy-life-expectancy-at-birth)

- [Libertad para tomar decisiones vitales](#freedom-to-make-life-choices)

- [Generosidad](#generosity)

- [Percepción de corrupción](#perceptions-of-corruption)

- [Afectos positivos](#positive-affect)

- [Afectos negativos](#negative-affect)

- [Confianza en el gobierno nacional](#confidence-in-national-government)


---

## 2. Patrones

|  Generales  |
| ----------- |
| Datos de naturaleza... ``<insertar descripción>``
| ``<insertar el homólogo en este batch de datos>`` a  ``Escalas de valoración (ambiente laboral, satisfacción con el trabajo) sin estandarizar (0-5, 0-50).``
|Columnas duplicadas (``<las que sean``>).
|Columnas que contienen ``<X cosa>``.
|``<más propiedades, como valores boleanos>``.|

---
---
ㅤ     

|  Valores nulos  |
| ----------------|
|``Descripción y distribución``|
---
---
ㅤ     


|  Valores Objeto |
| ----------------|
|``Descripción y distribución``|
---
---
ㅤ     

| Valores Numéricos |
| ------------------|
|``Descripción y distribución``|
---

---
---

ㅤ     

## 3. Análisis Exploratorio de Datos (EDA)


### Country Name

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Regional Indicator

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Year

*Año de la recolección de los datos*


**Propuesta de mejora:**

       > 
ㅤ
**Propuesta ejecutada:**

- 

---
---

### Life Ladder

*Escala de satisfacción vital.*

Las evaluaciones de vida de la encuesta Gallup *World Poll* son la base para el ranking anual de felicidad.

 La *escala de Cantril* pide a los encuestados que imaginen una escalera, donde el peldaño 10 representa la mejor vida posible para ellos y el 0, la peor. Luego, se les pide que califiquen su vida actual en una escala del 0 al 10.

**Propuesta de mejora:**

       > 

**Propuesta ejecutada:**

- 

---
---

### Log GDP Per Capita

*Logaritmo del PIB per cápita, que no es lo mismo que PIB per cápita*:

Esta métrica se refiere al logaritmo (generalmente en base 10 o natural) del Producto Interno Bruto (PIB) por persona, ajustado a paridad de poder adquisitivo (PPA) en muchos contextos.

Se utiliza para suavizar la distribución de los datos y **facilitar comparaciones entre países con diferencias económicas muy marcadas**, ya que el logaritmo reduce el impacto de valores extremos y permite analizar el crecimiento relativo en lugar del absoluto.

No trabajamos con el crecimiento absoluto. Podría ser interesante cruzar el dato.



**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Social Support

*Apoyo social percibido*

Usa la media nacional de las respuestas binarias (0=no, 1=sí) a la pregunta de la encuesta Gallup *World Poll* (GWP): 

>      “Si tuviera problemas, ¿tiene familiares o amigos en quienes pueda confiar para que le ayuden siempre que los necesite, o no?”.

ㅤ
**Propuesta de mejora:**

       > 

**Propuesta ejecutada:**

- 

---
---

### Healthy Life Expectancy At Birth

*Esperanza de vida al nacer.*

 La serie temporal se construye a partir de datos del repositorio de la Organización Mundial de la Salud (OMS). Para cubrir el período de este informe (2005-2022), se utilizan técnicas de interpolación y extrapolación.
ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Freedom To Make Life Choices

Se usa la media nacional de las respuestas binarias (0-1) a la pregunta de la GWP:

>      “¿Está satisfecho o insatisfecho con su libertad para elegir qué hacer con su vida?”


**Propuesta de mejora:**

       > 

**Propuestas ejecutadas:**

-

---
---

### Generosity

*Cantidad de donaciones en relación con el log. del PIB per cápita*

Se calcula como el residuo de la regresión de la media nacional de las respuestas de la GWP a la pregunta:

>      “¿Ha donado dinero a una organización benéfica en el último mes?” sobre el logaritmo del PIB per cápita.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Perceptions Of Corruption

Se usa la media de las respuestas binarias (0-1) a dos preguntas de la GWP: 

>      “¿La corrupción está muy extendida en el gobierno o no?”

>       “¿La corrupción está muy extendida en las empresas o no?”

Cuando faltan datos sobre corrupción gubernamental, se utiliza la percepción de corrupción en las empresas como medida general.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Positive Affect

*Sentimientos positivos experimentados recientemente*

Se define como la media de las medidas de efectos del día anterior para risa, disfrute e interés. La inclusión del interés (**incorporado por primera vez en el Informe Mundial de la Felicidad 2022**) aporta tres componentes tanto al afecto positivo como al negativo, mejorando ligeramente el ajuste del modelo en la columna 4. 

La forma general de las preguntas sobre afecto es: 

>      “¿Experimentó los siguientes sentimientos durante gran parte del día de ayer?”.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Negative Affect

*Sentimientos negativos experimentados recientemente*

Se define como la media de las medidas de efectos del día anterior para preocupación, tristeza y enojo.

ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

### Confidence In National Government

*Confianza en el Gobierno de la Nación*

Esta variable se calcula a partir de la siguiente pregunta de la encuesta Gallup *World Poll*:

>      “¿Tiene confianza en el gobierno nacional?”.

Las opciones de respuesta son:
- “Sí, siempre”

- “Sí, a veces”

- “No, rara vez”

- “No, nunca”

- “No sabe”

La variable se calcula como el porcentaje de encuestados que responden ``“Sí, siempre”`` o ``“Sí, a veces”`` a esta pregunta.


ㅤ
**Propuesta de mejora:**

       > 


**Propuestas ejecutadas:**

- 

---
---

## 4. Cambios ejecutados

Propuestas ejecutadas generales y particulares a columnas concretas:

| Transformaciones WHR [1](/notebooks/Transf/transformacion-original.ipynb), [2](/notebooks/Transf/transformacion-v1-imputar.ipynb), [3](/notebooks/Transf/transformacion-v2-sin-imputar.ipynb)

| Transformaciones en fuentes de datos secundarias [1](/notebooks/Transf/transformación-gallup-info-2005-2025.ipynb)

| [Resultados, datos limpios WHR](/data/processed/WHR_limpio_sin_imputar.csv)

| [Metodología y muestreo](/data/processed/gallup-interviews-info-2005-2025.csv), [Muestreo por país](/data/processed/summary_interviews_by_country.csv)

---

## 5. Nuestras cuestiones sobre los datos

Primeras preguntas para enfocar el análisis del proyecto:

``A integrar de los documentos anexos.``

---
---

## 6. Visualización como respuesta

---
---


## 7. Propuesta de valor

¿Qué concluimos que mide realmente este informe?

Responder a esto exige matices sobre el alcance de este modelo y sus limitaciones metodológicas, especialmente cuando se presentan resultados como reflejo de realidades nacionales o globales.

- El modelo mide satisfacción con el sistema, no felicidad en sentido amplio.

- El modelo no ajusta sus muestras por densidad poblacional.

- El modelo excluye deliberadamente zonas percibidas como 'peligrosas' para el entrevistador'; no se especifica criterio.

- El modelo presenta inconsistencia de métodos: la falta de uniformidad en la recolección complica la comparabilidad y el análisis estadístico.

Hemos comprobado que en sociedades con fuerte estado de bienestar, la gente puede percibir su vida como *buena* (en relación a su seguridad económica), pero eso no elimina problemas estructurales.

También hemos observado que favorece el sesgo de narrativa mediática:

- El uso de términos absolutos pueden inducir a confusión en la interpretación de qué quiere decir este dato. Por ejemplo, se presenta un índice de **Generosidad**, basado en datos fiscales de donaciones que se gravan en un país en relación a lo que se espera según su PIB, parejo al de **Satisfacción Vital** que, por otro lado, engloba las respuestas de los entrevistados sobre la percepción de sus aspiraciones.

Esto es importante sobre todo cuando el destino de estos reportes suelen ser los medios de comunicación.

Esto plantea 2 riesgos:

1. **Sobregeneralización**: Se confunde la opinión individual de una muestra aproximada de 1000 habitantes con datos estructurales.

2. **Sesgo cultural**: Lo que una sociedad entiende por *felicidad* o *apoyo social* varía enormemente (ej.: en Japón, la satisfacción vital puede estar ligada al grupo; en países nórdicos, al individualismo).

Por todo esto, concluimos que **la precisión técnica es un imperativo ético**.

### Nuestra propuesta de valor: ¿Qué podemos hacer y exigir como profesionales?

**Transparencia**    
Explicitar qué mide realmente un índice o un conjunto de muestras.

**Contextualización**       
Evitar fomentar rankings simplistas sin análisis de sesgos o contraste metodológico.

**Enfoque pragmático y**    
Preguntarnos ¿quién se beneficia con la perspectiva de estos resultados? y documentar quién y qué queda fuera del radar.

---
---

### 8. Next steps: vistas a futuro

**Normalización y Documentación**

- Glosario de Valores: sería necesario un glosario que defina explícitamente el significado de cada valor en las escalas utilizadas.

- Convención de Escala: Documentar formalmente el uso de los valores en las escalas, aunque no aparezcan en los registros actuales.