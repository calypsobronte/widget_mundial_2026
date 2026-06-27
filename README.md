# ⚽ Mundial FIFA 2026 - Widget Ryuk (Tiempo Real)
Widget Ryuk resultados en tiempo real para las **Plataformas de streaming** para el **Mundial FIFA 2026**. Muestra los partidos en vivo, los próximos partidos y los resultados anteriores de forma elegante y profesional.

---

## ✨ Características
- **Datos en tiempo real** desde la API oficial de ESPN
- **Prioridad inteligente**: Muestra primero los partidos **En Vivo**, luego los **próximos a jugar**
- **Filtro por equipo vía URL**: Elige exactamente qué partido mostrar cuando hay varios en simultáneo
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
  - Fecha del partido
- **Totalmente responsive** y optimizado para OBS, Meld Studio y otras plataformas de streaming
- **Hecho por RyukPlay**

---

## 📦 Cómo usarlo en OBS, Meld Studio, entre otros

### 1. Agregar como fuente de navegador
1. En OBS, haz clic derecho en **Fuentes** → **Agregar** → **Navegador**
2. Configura los siguientes parámetros:

| Parámetro | Valor recomendado | Notas |
|---|---|---|
| **URL** | Ruta del archivo HTML | Ver abajo |
| **Width** | `1100` | Ancho base |
| **Height** | `170` | Altura recomendada |
| **FPS** | `60` | O 30 si tu PC es limitada |
| **Shutdown source when not visible** | Activado | Recomendado |
| **Refresh browser when scene becomes active** | Activado | Recomendado |

### 2. URL del widget

```
https://calypsobronte.github.io/widget_mundial_2026/widget_premium_ryukplay.html
```

---

## 🎯 Filtrar partido por equipo (nuevo)

Cuando hay dos o más partidos en simultáneo puedes elegir cuál mostrar añadiendo parámetros a la URL:

| Parámetro | Ejemplo | Qué hace |
|---|---|---|
| `?home=XXX&away=YYY` | `?home=COL&away=ARG` | Muestra ese partido exacto |
| `?team=XXX` | `?team=COL` | Muestra cualquier partido donde juegue ese equipo |
| *(sin parámetros)* | URL normal | Auto: muestra el partido más relevante |

### Ejemplos de URL con filtro

```
...widget_premium_ryukplay.html?home=COL&away=ARG
...widget_premium_ryukplay.html?home=ESP&away=BRA
...widget_premium_ryukplay.html?home=NZL&away=BEL
...widget_premium_ryukplay.html?team=COL
...widget_premium_ryukplay.html?team=NZL
```

> **Consejo:** Usa `?team=XXX` si no sabes si tu equipo juega de local o visitante — el widget lo encuentra en ambos casos.  
> Si el partido no se encuentra, muestra el más relevante disponible con un aviso en el widget.

---

## 🌍 Abreviaturas de los 48 países — Mundial 2026

### CONMEBOL — Sudamérica
| País | Código |
|---|---|
| Argentina | `ARG` |
| Brasil | `BRA` |
| Colombia | `COL` |
| Ecuador | `ECU` |
| Paraguay | `PAR` |
| Uruguay | `URU` |

### UEFA — Europa
| País | Código |
|---|---|
| Alemania | `GER` |
| Austria | `AUT` |
| Bélgica | `BEL` |
| Bosnia y Herzegovina | `BIH` |
| Chequia | `CZE` |
| Croacia | `CRO` |
| Escocia | `SCO` |
| España | `ESP` |
| Francia | `FRA` |
| Inglaterra | `ENG` |
| Noruega | `NOR` |
| Países Bajos | `NED` |
| Portugal | `POR` |
| Suecia | `SWE` |
| Suiza | `SUI` |
| Turquía | `TUR` |

### CONCACAF — Norte y Centroamérica
| País | Código |
|---|---|
| Canadá | `CAN` |
| Curaçao | `CUW` |
| Haití | `HAI` |
| México | `MEX` |
| Panamá | `PAN` |
| USA | `USA` |

### CAF — África
| País | Código |
|---|---|
| Algeria | `ALG` |
| Camerún | `CMR` |
| Cabo Verde | `CPV` |
| Costa de Marfil | `CIV` |
| Egipto | `EGY` |
| Ghana | `GHA` |
| Marruecos | `MAR` |
| Nigeria | `NGA` |
| Rep. Democrática del Congo | `COD` |
| Senegal | `SEN` |
| Sudáfrica | `RSA` |
| Túnez | `TUN` |

### AFC — Asia
| País | Código |
|---|---|
| Arabia Saudita | `KSA` |
| Australia | `AUS` |
| Corea del Sur | `KOR` |
| Irak | `IRQ` |
| Irán | `IRN` |
| Japón | `JPN` |
| Jordania | `JOR` |
| Qatar | `QAT` |
| Uzbekistán | `UZB` |

### OFC — Oceanía
| País | Código |
|---|---|
| Nueva Zelanda | `NZL` |

### Lista rápida — todos los códigos
```
ALG · ARG · AUS · AUT · BEL · BIH · BRA · CAN · CIV · CMR
COD · COL · CPV · CRO · CUW · CZE · ECU · EGY · ENG · ESP
FRA · GER · GHA · HAI · IRN · IRQ · JOR · JPN · KOR · KSA
MAR · MEX · NED · NOR · NZL · PAN · PAR · POR · QAT · RSA
SCO · SEN · SUI · SWE · TUN · TUR · URU · USA · UZB
```

---

## 🔄 Actualización de datos
El widget se actualiza automáticamente cada **30 segundos**.  
También puedes recargar la fuente manualmente en OBS si lo necesitas.

---

## 📌 Lógica del widget

El widget elige automáticamente qué partido mostrar según esta prioridad:

1. **Partido En Vivo** que coincida con el filtro (si se especificó)
2. **Próximo partido a jugar** que coincida con el filtro
3. **Último partido finalizado** que coincida con el filtro
4. Si no hay coincidencia → muestra el partido más relevante disponible con aviso

Sin filtros activos sigue la misma prioridad pero sobre todos los partidos disponibles.

---

## 📸 Vista previa

El widget muestra:
- Banderas de los equipos
- Marcador actualizado
- Estadio / Ciudad
- Grupo del partido
- Estado del partido (EN VIVO / PRÓXIMO / FINALIZADO)
- Tiempo de juego o hora programada
- Fecha del partido
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

## 📬 Contacto
- **Portfolio**: [calypsobronte.github.io](https://calypsobronte.github.io/)
- **LinkedIn**: [linkedin.com/in/calypsobronte](https://linkedin.com/in/calypsobronte)
- **GitHub**: [github.com/calypsobronte](https://github.com/calypsobronte)
- **YouTube**: [youtube.com/@ryukdeathnotetv](https://www.youtube.com/@ryukdeathnotetv)
- **Email**: codellinamaria@gmail.com

---

> Built with ❤️ and a lot of coffee.
