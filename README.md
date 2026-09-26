# Tenshigana

**Aprender japonés debería sentirse como un juego, no como una tarea.** Tenshigana es una aplicación de escritorio para practicar Hiragana, Katakana, Kanji, Números y Vocabulario basada en inferencias forzadas y memoria: ves el carácter, escribís su lectura en romaji… contra reloj. Sin ayuda visual, sin excusas.

LINK DE DESCARGA: https://www.mediafire.com/file/ev5f4ktgk6omehp/Tenshigana_by_Ronzano.rar/file



## ¿Qué te vas a encontrar?

### Cinco modos de estudio, con contenido real incluido

| Modo | Contenido | Tiempo por pregunta |
|---|---|---|
| **Hiragana** | 46 caracteres básicos | 3 segundos |
| **Katakana** | 46 caracteres básicos | 3 segundos |
| **Kanji** | 20 kanji esenciales (ichi ni san … hito nichi tsuki yama kawa) | 6–10 s según longitud de la lectura |
| **Vocabulario** | 160 palabras reales (80 en hiragana + 80 en katakana) | 8–15 s según largo de la palabra |
| **Números** | 60 números en japonés | Sin límite de tiempo |

En **Vocabulario** además podés filtrar qué tipo de palabras practicar: solo hiragana, solo katakana o todas juntas (ya meteré más cositas).

### Cuentas regresivas dinámicas (los "cooldown" por palabra)

El cronómetro no es fijo: se adapta a cada pregunta. En Vocabulario, una palabra de 1-2 kana tiene 8 segundos, y cada kana extra suma 1 segundo más (hasta 15 s). En Kanji, las lecturas largas también reciben tiempo adicional (6 s base + 0,5 s por kana extra). Así, una palabra difícil nunca te roba tiempo que necesitabas, ni una fácil te lo regala de más. Si se agota el tiempo, la respuesta cuenta como incorrecta y pasás a la siguiente.

### Respuestas flexibles, corrección estricta

El evaluador normaliza lo que escribís y acepta variantes comunes de romanización (por ejemplo `shi` / `si`, `tsu` / `tu`, `fu` / `hu`), así que no perdés puntos por escribir "ko" en vez de "kō". Cada pregunta se resuelve al instante: aciertos y errores se marcan con parpadeos verdes/rojos (éxito, error y tiempo agotado tienen su propio efecto).

### Sistema de rachas con multiplicador

El motor de rachas (`StreakManager`) está listo para premiar tu constancia: x2 a las 5 correctas seguidas, x3 a las 10, x4 a las 15, x5 a las 20, x7 a las 30 y x10 a las 50. Romper la racha vuelve a empezar desde cero (el mejor récord se conserva) — mantenerla es parte del desafío.

### Sesiones a tu medida

Elegí entre 10, 20, 30 preguntas o el mazo completo ("Todo", que la verdad no te lo recomiendo, es re denso y no le puse botón de cancelar prueba), siempre en orden aleatorio. Al terminar, la pantalla de resultados te muestra todo: total de preguntas, aciertos, errores, porcentaje, tiempo total y tiempo promedio por pregunta.

### Estadísticas que motivan

La sección **Ver Estadísticas** guarda todo tu progreso en una mini base de datos en tu PC y lo convierte en información útil:

- **Resumen global**: sesiones jugadas, precisión media y totales.
- **Rendimiento por modo**: cómo andás en cada uno de los cinco modos.
- **Tus errores más frecuentes (Top 5)**: los caracteres que más fallás, con su romanización para que dejes de tropezar con la misma piedra.
- **Curva de desempeño**: tu evolución de precisión a lo largo de los últimos 30 días.
- **Mapa de calor**: tu actividad diaria (estilo GitHub) de hasta un año — ideal para no romper la constancia, más decoración que otra cosa.
- **Comparativa de modos**: un gráfico de radar para ver de un vistazo dónde sos fuerte y dónde flojeás.
- **Logros y rangos**: 6 familias de logros (sesiones, respuestas correctas, mejor racha, días activos, precisión y maestría de modos) y un sistema de XP con 8 rangos: de *Principiante* a *Gran Maestro*.



## Requisitos

- Python 3.8+
- customtkinter
- Pillow
- matplotlib y numpy (para las gráficas de estadísticas)
- pygame (opcional, para los sonidos)

(Nada de esto debería hacerte falta, si me salió bien lo estás usando sin complicaciones)

## Instalación

Opción A: Usás el ejecutable que te di yo (ese ZIP que te pasé). Más fácil y como debería ser hecho.

Opción B: No, no te voy a dejar clonar el repositorio original. Pa qué?

```

## Donaciones

Si esta app te está ayudando en tu camino por el japonés y querés apoyar su desarrollo, podés dejar tu cafecito en: [cafecito.app/liminarg](https://cafecito.app/liminarg) ☕

## Tecnologías Utilizadas

- **CustomTkinter**: interfaz gráfica moderna y oscura
- **SQLite**: persistencia de progreso, logros y rangos
- **matplotlib + numpy**: gráficas de rendimiento
- **Pillow**: imágenes de fondo y efectos
- **pygame**: sonidos (opcional)

## Licencia

Este proyecto es de código abierto. Siéntete libre de usarlo, modificarlo y distribuirlo. PERO REDIRIGÍS A MIS PERFILES

## Autor

Desarrollado por Liminarg (SanRIchi_Ronz)

---

Nos vimo' en Tokio~
