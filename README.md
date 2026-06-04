# Diseño de un Arreglo de Antenas Dipolo Plegado para la Banda WiFi de 5.6 GHz

> Universidad de Nariño — Ingeniería Electrónica  
> Autores: **Junior Lara**, **Jerson Lopez**  
> Pasto, Colombia

---

## Descripción

Diseño, simulación y fabricación de una antena de dipolo plegado y su arreglo de 4 elementos operando en la banda **U-NII de 5 GHz** (WiFi 802.11a/n/ac/ax).

| Etapa | Herramienta |
|-------|-------------|
| Simulación EM | FEKO (Altair) |
| Diseño PCB | EasyEDA |
| Fabricación | JLCPCB (China) |
| Sustrato | FR-4, εᵣ = 4.4, h = 1.575 mm |

---

## Resultados Principales

| Parámetro | Dipolo individual | Arreglo 4 elementos |
|-----------|:-----------------:|:-------------------:|
| Frecuencia de resonancia | 5.694 GHz | 5.701 GHz |
| S₁₁ mínimo | −21.9 dB | −19.79 dB |
| Ancho de banda | 4.0 – 6.2 GHz | 5.6 – 5.8 GHz |
| Ganancia máxima | ~0 dBi | ~5.6 dBi |
| Impedancia @ freq. diseño | 45.07 − j5.58 Ω | 58.55 + j0.27 Ω |

---

## Estructura del Repositorio

```
folded-dipole-array-5GHz/
│
├── simulation/           # Archivos de simulación FEKO
├── pcb/                  # Diseño PCB (EasyEDA)
├── measurements/         # Mediciones experimentales con VNA
├── paper/                # Informe en LaTeX
├── results/              # Figuras y datos exportados
├── README.md
└── LICENSE
```

---

## Diseño

- **Frecuencia central:** 5.6 GHz
- **Balun λ/4:** Zₜ = 122.47 Ω, longitud = 6.39 mm
- **Separación entre elementos:** λ (arreglo lineal)
- **Red de alimentación:** T-junction con transformadores λ/4
- **Impedancia de entrada total:** 50 Ω

---

## Requisitos para simulación

- **Altair FEKO** (versión utilizada: indicar la tuya)
- Los archivos `.cfx` / `.fek` se encuentran en `simulation/`

---

## Fabricación

El diseño PCB fue exportado desde EasyEDA y fabricado por **JLCPCB**. Los archivos Gerber listos para fabricación se encuentran en `pcb/gerber/`.

---

## Referencia

```bibtex
@inproceedings{lara2024dipolo,
  title     = {Diseño de un Arreglo de Antenas Dipolo Plegado para la Banda WiFi de 5.6 GHz},
  author    = {Lara, Junior and Lopez, Jerson},
  year      = {2024},
  institution = {Universidad de Nariño},
  address   = {Pasto, Colombia}
}
```

---

## Contacto

- Junior Lara — juniorlara24@udenar.edu.co
- Jerson Lopez — jersonalvarolopeztoro@gmail.com
