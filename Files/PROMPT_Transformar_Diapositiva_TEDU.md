
# 🧠 PROMPT DE TRANSFORMACIÓN DE DIAPOSITIVAS AL ESTILO MEGAMODELO TEdU

## 🔧 TAREA
Transforma esta diapositiva HTML al estilo visual del MegaModelo TEdU.

## 🎯 OBJETIVO VISUAL
- La diapositiva debe tener un **lienzo centrado de 1280x720 px** con:
  - Bordes redondeados (`border-radius: 8px`)
  - Sombra elegante (`box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1)`)
  - Fondo claro exterior (`#f8fafc`)
- La **barra de colores** debe:
  - Estar al inicio del lienzo
  - Tener **bordes redondeados superiores** (`border-top-left-radius: 8px`, `border-top-right-radius: 8px`)
  - Usar los colores institucionales (`--unicomfa-blue`, `--unicomfa-orange`, `--unicomfa-green`) en gradiente
- El contenido debe:
  - Mantenerse intacto
  - Tener desplazamiento vertical interno si excede el alto disponible

## 🧠 DETALLES TÉCNICOS
- Asegúrate de que `.slide-container` centre verticalmente el lienzo:

```css
display: flex;
justify-content: center;
align-items: center;
min-height: 100vh;
background-color: #f8fafc;
```

- El contenedor `.slide` debe tener:

```css
width: 1280px;
height: 720px;
border-radius: 8px;
box-shadow: 0 10px 25px rgba(0,0,0,0.1);
overflow: hidden;
display: flex;
flex-direction: column;
```

- La barra `.header-bar` debe tener:

```css
height: 8px;
background: linear-gradient(to right, var(--unicomfa-blue) 33%, var(--unicomfa-orange) 33%, var(--unicomfa-orange) 66%, var(--unicomfa-green) 66%);
border-top-left-radius: 8px;
border-top-right-radius: 8px;
```

## 📎 INSTRUCCIONES DE USO
1. Copia y pega el contenido HTML original de cualquier diapositiva.
2. Ejecuta el prompt anterior en ChatGPT con GPT-4 o GPT-4o.
3. Solicita que se genere el archivo `.htm` resultante para descargarlo y reemplazar tu versión anterior.

> 🔁 Puedes usarlo en tantas diapositivas como necesites, una por una.
