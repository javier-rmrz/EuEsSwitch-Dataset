# EuEsSwitch-Dataset
**Corpus de voz con code-switching Español–Euskera**

## Descripción
EuEsSwitch-Dataset es un dataset de audio sintético diseñado para investigación en **reconocimiento automático del habla (ASR)** con **cambio de código (code-switching)** entre **español (castellano)** y **euskera**.

El dataset incluye tanto **segmentos monolingües** como **combinaciones bilingües**, lo que permite experimentar con:
- ASR con code-switching
- detección de idioma
- segmentación de audio
- modelos multilingües

---

## Estructura del dataset

El dataset se organiza en las siguientes carpetas:

### `plainEu`
- 50 segmentos de audio generados en **euskera**
- Duración: **4–7 segundos**

### `plainEs`
- 50 segmentos de audio generados en **castellano**
- Duración: **4–7 segundos**

### `2secCombos`
- 2500 audios
- Cada audio combina **2 segmentos**
- Los segmentos provienen de `plainEu` y `plainEs`
- Contienen combinaciones bilingües euskera–español

### `3secCombos`
- 1000 audios
- Cada audio combina **3 segmentos**
- Los segmentos provienen de `plainEu` y `plainEs`
- Se garantiza que:
  - no todos los segmentos son del mismo idioma
  - el patrón de idiomas varía entre audios

### `4secCombos`
- 500 audios
- Cada audio combina **4 segmentos**
- Los segmentos provienen de `plainEu` y `plainEs`
- Se garantiza que:
  - no todos los segmentos son del mismo idioma
  - el patrón de idiomas varía entre audios

---

## Propósito
Este dataset ha sido creado para facilitar experimentos en habla bilingüe y code-switching, especialmente en sistemas ASR español–euskera.

Puede utilizarse para:
- entrenamiento y evaluación de modelos ASR con mezcla de idiomas
- detección automática de idioma en audio
- análisis de transiciones entre euskera y castellano
- benchmarking de modelos multilingües como Whisper

---

## Estrategia de composición
El dataset sigue una estructura de complejidad progresiva:

- **Segmentos base monolingües**: `plainEu`, `plainEs`
- **Combinaciones de 2 segmentos**: escenarios simples
- **Combinaciones de 3 segmentos**: mayor variabilidad
- **Combinaciones de 4 segmentos**: secuencias más complejas

Esto permite analizar cómo se comportan los modelos ante distintos niveles de code-switching.

---

## Notas
- Este es un **dataset sintético**, generado a partir de segmentos de audio.
- Los audios combinados se construyen mediante concatenación de segmentos.
- Está orientado a investigación en procesamiento de habla multilingüe.

---

## Autor
**Javier Ramírez Zarzoso**  
GitHub: https://github.com/javier-rmrz

---

## Cita
Si utilizas este dataset, por favor cítalo como:

```bibtex
@dataset{ramirezzarzoso2026euesswitch,
  title     = {EuEsSwitch-Dataset: Corpus de voz con code-switching Español–Euskera},
  author    = {Javier Ramírez Zarzoso},
  year      = {2026}
}