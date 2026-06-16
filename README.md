# ⚽ Mundial FIFA 2026 - Widget Ryuk (Tiempo Real)

Widget Ryuk resultados en tiempo real para las **Plataformas de streaming** para el **Mundial FIFA 2026**. Muestra los partidos en vivo, los próximos partidos y los resultados anteriores de forma elegante y profesional.

---

## ✨ Características

- **Datos en tiempo real** desde la API oficial de ESPN
- **Prioridad inteligente**: Muestra primero los partidos **En Vivo**, luego los **próximos a jugar**
- **Efectos premium**:
  - Animación de gol (parpadeo + brillo verde)
  - Estado "EN VIVO" con pulso
  - Actualización suave del marcador
- **Diseño moderno** con fondo semi-transparente (estilo glassmorphism)
- **Muestra**:
  - Equipos con banderas
  - Marcador en tiempo real
  - Estadio / Ciudad
  - Grupo del partido
  - Tiempo de juego (minuto actual)
  - Hora programada de los partidos próximos
- **Totalmente responsive** y optimizado para OBS, Meld Studio y otras plataformas de streaming
- **Hecho por RyukPlay**

---

## 📦 Cómo usarlo en OBS, Meld Studio, entre otros.

### 1. Agregar como fuente de navegador

1. En OBS, haz clic derecho en **Fuentes** → **Agregar** → **Navegador**
2. Configura los siguientes parámetros:

| Parámetro                        | Valor recomendado          | Notas |
|----------------------------------|----------------------------|-------|
| **URL**                          | Ruta del archivo HTML      | Ver abajo |
| **Width**                        | `1100`                     | Ancho base |
| **Height**                       | `170`                      | Altura recomendada |
| **FPS**                          | `60`                       | O 30 si tu PC es limitada |
| **Shutdown source when not visible** | Activado              | Recomendado |
| **Refresh browser when scene becomes active** | Activado     | Recomendado |

### 2. URL visualizar widget
https://calypsobronte.github.io/widget_mundial_2026/widget_premium_ryukplay.html

---

## 🔄 Actualización de datos

El widget se actualiza automáticamente cada **30 segundos**.  
También puedes hacer clic en el botón **"Actualizar"** (si lo tienes visible) o recargar la fuente en OBS.

---

## 📌 Lógica del widget

El widget elige automáticamente qué partido mostrar según esta prioridad:

1. **Partido En Vivo** (si hay alguno)
2. **Próximo partido a jugar** (el más cercano)
3. **Último partido finalizado** (solo si no hay partidos activos)

---

## 📸 Vista previa

El widget muestra:
- Banderas de los equipos
- Marcador actualizado
- Estadio / Ciudad
- Estado del partido (EN VIVO / PRÓXIMO / FINALIZADO)
- Tiempo de juego o hora programada
- Efectos visuales al marcar gol

---

## 👤 Créditos

- **Desarrollado por:** [RyukPlay](https://calypsobronte.github.io/)
- **Datos proporcionados por:** [ESPN API](https://www.espn.com/)
- **Diseño & Código:** Premium Widget para FIFA World Cup 2026

---

## 📄 Licencia

- Este proyecto está bajo la licencia **MIT**.   
- Uso libre para streams y contenido personal.   
- Se agradece el crédito a **RyukPlay** si lo utilizas públicamente.

---

## 🤝 Contribuir

¿Quieres mejorar el widget? ¡Eres bienvenido!

1. Haz un **Fork** del repositorio
2. Crea una rama nueva (`git checkout -b feature/nueva_rama`)
3. Haz tus cambios
4. Abre un **Pull Request**
5. Describe claramente qué mejora o arreglo estás proponiendo

Revisaré los PRs y los aceptaré si son útiles y están bien hechos.

---

## 📬 Contact

- **Portfolio**: [calypsobronte.github.io](https://calypsobronte.github.io/)
- **LinkedIn**: [linkedin.com/in/calypsobronte](https://linkedin.com/in/calypsobronte)
- **GitHub**: [github.com/calypsobronte](https://github.com/calypsobronte)
- **YouTube**: [youtube.com/@ryukdeathnotetv](https://www.youtube.com/@ryukdeathnotetv)
- **Email**: codellinamaria@gmail.com

---

> Built with ❤️ and a lot of coffee.
