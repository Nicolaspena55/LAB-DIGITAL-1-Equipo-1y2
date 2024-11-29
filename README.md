# TTL-VS-CMOS-LAB-DIGITAL-1
El propósito de este laboratorio es analizar las características y ventajas de cada tecnología mediante experimentos prácticos. Esto permitirá observar su comportamiento en diferentes condiciones operativas y determinar cuál resulta más adecuado para ciertas aplicaciones. Durante este proceso, se evaluarán factores como:

-tiempo de subida y bajada
-tiempo de retardo
- disipacion de potencia
- fan-in y fan-out

encontramos el circuito equivalente de cada negador

## Circuito equivalente  74LS04
![ttl](https://github.com/user-attachments/assets/bd37e73f-eff7-4ed3-9421-eb3a12e64edc)

## Circuito equivalente  CD4069
![cmos](https://github.com/user-attachments/assets/d415f482-7571-4d85-9fc8-601dcad018b0)




para hacer esta practica se desarrollan las simulaciones de los parametros , como se muestra en las siguientes imagenes


# Practica 1: COMPARACIÓN DE TECNOLOGÍA CMOS y TTL

## Abstract
This project focuses on the comparative analysis of two fundamental technologies in the design and development of digital circuits: **TTL (Transistor-Transistor Logic)** and **CMOS (Complementary Metal-Oxide-Semiconductor)**. These architectures have been pivotal in the evolution of digital electronics and are widely used in various applications, ranging from computing systems to mobile devices and consumer electronics.

## Keywords
- TTL (Transistor-Transistor Logic)
- CMOS (Complementary Metal-Oxide-Semiconductor)
- Digital Circuits
- Semiconductor Technology
- Logic Gates
- Electronic Circuit Design

---

## Resumen
El presente proyecto se enfoca en el análisis comparativo entre dos tecnologías fundamentales en el diseño y desarrollo de circuitos digitales: **TTL (Transistor-Transistor Logic)** y **CMOS (Semiconductor Complementario de Óxido Metálico)**. Estas arquitecturas han sido pilares en la evolución de la electrónica digital y se utilizan ampliamente en diferentes aplicaciones, desde sistemas de computación hasta dispositivos móviles y electrónicos de consumo.

## Introducción
La electrónica digital es un área fundamental en el desarrollo de sistemas modernos, ya que permite el procesamiento de señales a través de circuitos que operan con valores discretos. Estos circuitos se implementan utilizando diversas tecnologías de fabricación, cada una con sus propias características y ventajas. Entre las tecnologías más comunes para la construcción de circuitos digitales se encuentran **TTL (Transistor-Transistor Logic)** y **CMOS (Complementary Metal-Oxide-Semiconductor)**. Ambas son ampliamente utilizadas en la creación de puertas lógicas y otros componentes esenciales en sistemas electrónicos.
    En este laboratorio, se realizará un análisis comparativo entre las tecnologías TTL y CMOS mediante la implementación de un negador (inversor) en ambos casos. El propósito es observar y analizar las diferencias entre los circuitos de **TTL 74LS04 y CMOS CD4069** en términos de diseño, tiempo de respuesta y consumo de energía. A través de esta comparación, se busca entender cómo las características propias de cada tecnología impactan en el rendimiento de un circuito básico y cómo se comportan bajo condiciones operativas similares. El análisis ayudará a identificar las ventajas y desventajas de cada tecnología, proporcionando una base sólida para seleccionar la más adecuada según las necesidades de un proyecto de diseño de circuitos digitales

---

## Objetivos
- Identificar las características de un dispositivo fabricado en diferentes tecnologías.
- Evaluar las ventajas y desventajas de las tecnologías **TTL** y **CMOS** en términos de diseño, tiempo de respuesta y consumo energético.

---

## Recursos Requeridos
- Negador **TTL 74LS04**
- Negador **CMOS CD4069**
- Simulador
- Datasheets
- Modelos Spice

---

## Circuitos Equivalentes

### TTL Circuit
![Circuito equivalente TTL](equivalentettl.png)

### CMOS Circuit
![Circuito equivalente CMOS](equivalentecmos.png)

---

## Especificaciones Técnicas

### Tiempos
El tiempo de subida, tiempo de bajada y tiempo de retardo son parámetros clave para evaluar el rendimiento dinámico de los circuitos digitales:

#### Tiempo de Subida
- **74LS04 (TTL)**: 104 nS  
  ![Tiempo de subida TTL](tsubida74ls.png)
- **CD4069 (CMOS)**: 118 nS  
  ![Tiempo de subida CMOS](tsubidacd.png)

#### Tiempo de Bajada
- **74LS04 (TTL)**: 338 nS  
  ![Tiempo de bajada TTL](tbajada74ls.png)
- **CD4069 (CMOS)**: 1.16 µS  
  ![Tiempo de bajada CMOS](tbajadacd.png)

#### Tiempo de Retardo
- **74LS04 (TTL)**: 84 nS  
  ![Tiempo de retardo TTL](tretardottl.png)
- **CD4069 (CMOS)**: 496 nS  
  ![Tiempo de retardo CMOS](tretardocmos.png)

---

## Condiciones del Datasheet

### TTL (74LS04)
- **Tiempo de Subida/Bajada/Retardo**: 10-15 nS  
- **Fan-In**: 1  
- **Fan-Out**: ~10 unidades de carga  
- **Disipación de Potencia**:  
  - \( V_{cc} = 2.22 \, \text{V} \), \( I_{cc} = 14.38 \, \text{mA} \)  
  - \( P = V_{cc} \cdot I_{cc} = 32 \, \text{mW} \)

### CMOS (CD4069)
- **Tiempo de Subida/Bajada/Retardo**: 30-50 nS  
- **Fan-In**: 1  
- **Fan-Out**: 5 unidades de carga  
- **Disipación de Potencia**:  
  - \( V_{cc} = 3.25 \, \text{V} \), \( I_{cc} = 13.23 \, \mu\text{A} \)  
  - \( P = V_{cc} \cdot I_{cc} = 42.99 \, \mu\text{W} \)

---

## Oscilador en Anillo Basado en la Compuerta NOT
El oscilador de anillo utiliza un número impar de inversores conectados en un bucle, aprovechando el tiempo de retardo inherente de las puertas digitales. Este retardo genera una oscilación con un periodo de \( 2N \cdot t_p \), donde \( N \) es el número de inversores.

Su diseño y funcionamiento son fundamentales en circuitos digitales para generar señales oscilatorias precisas y medir parámetros como el tiempo de propagación del inversor.

---

