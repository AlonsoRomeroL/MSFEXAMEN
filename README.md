[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=AlonsoRomeroL/MSFEXAMEN)

# Práctica de Exámen: Sistema circulatorio
## Información del estudiante

Romero Landa Alonso Alejandro \[21212749]; l21212749@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1. Dibujar el diagrama eléctrico del sistema circulatorio, identificando cada uno de sus elementos: componentes, voltajes, corrientes y nodos de entrada y salida.
2. Determinar el modelo de ecuaciones integro-diferenciales del sistema.
3. Calcular la función de transferencia del sistema.
4. Utilizar Simulink para construir el sistema cardiovascular descrito.
5. Obtener las respuestas del Caso y el sistema de control en lazo cerrado.
6. Realizar la simulación del sistema con un tiempo de 10 s.

## Descripción detallada del sistema

El sistema circulatorio, en particular el comportamiento del corazón, puede ser representado de forma simplificada mediante un modelo que simule la dinámica de la presión y flujo sanguíneo a través de los compartimentos cardiacos. Para describir este comportamiento, se utiliza un circuito eléctrico de segundo orden tipo RLC.

La resistencia vascular se modela mediante un resistor `R`. La elasticidad de las arterias, que permite el almacenamiento temporal de energía, se representa mediante un capacitor `C`. La inercia de la masa de la sangre, que refleja la oposición al cambio de flujo, se modela mediante un inductor `L`.

El circuito comienza con una fuente de voltaje de entrada `Ve(t)`, la cual proporciona la señal de excitación y ocasiona una alteración en el flujo sanguíneo primario del compartimento. El resistor `R1` se conecta en serie con la fuente de voltaje y representa la resistencia al flujo sanguíneo en la rama principal `Fp(t)`.

El inductor `L` se conecta en serie con el resistor `R1`, representando la inercia de la masa sanguínea en todo el compartimento. En la primera rama secundaria se coloca un segundo resistor `R2`, cuyo valor permite identificar la capacidad de respuesta del sistema. Si el valor de `R2` es mucho mayor que `R1`, entonces el error en la respuesta será menor.

En la segunda rama secundaria se conecta un capacitor `C` en paralelo con `R2`, representando la elasticidad de las arterias. Entre más grande sea el valor del capacitor, la respuesta del sistema será más lenta. Este capacitor almacena y libera energía en el compartimento con un flujo sanguíneo secundario `Fs(t)`.

La energía almacenada y liberada se identifica como la salida del sistema `Vs(t)`, localizada en el nodo principal que conecta la rama principal con las ramas secundarias.

La señal de entrada `Ve(t)` está dada por una señal de impulso unitario, que representa una excitación abrupta similar a cómo el corazón responde a una estimulación inicial, por ejemplo, la señal generada por el nodo sinoauricular. El nodo sinoauricular se ubica en la parte superior de la aurícula derecha y se conoce como el marcapasos natural del corazón, ya que genera los impulsos eléctricos que regulan el latido cardiaco.

## Palabras clave
Sistema circulatorio; Circuito RLC; Controlador PID; Modelo biomecánico; Simulaciones numéricas, EID, Función de transferencia.

## Lista de archivos incluidos en el repositorio

1. Modelo de Simulink `[.slx]`.
2. Imágenes correspondientes al Scope con las señales de cada subsistema.
3. Capturas de pantalla de cada subsistema.
4. Imagen con los parámetros del controlador.
5. Evidencia del diagrama eléctrico del sistema cardiovascular.
6. Evidencia del modelo de ecuaciones integro-diferenciales.
7. Evidencia de la función de transferencia.
8. Archivo README.
9. Archivo CITATION.

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

\[3] N. S. Nise, Control Systems Engineering, 8th ed. Hoboken, New Jersey, USA: John Wiley \& Sons, 2020.

\[4] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 2, Page 26.

