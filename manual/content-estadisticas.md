# Manual de interpretación de las vistas Live / Estadísticas

Guía para pilotos. Sin tecnicismos. La idea es simple: **qué te dice cada número y cómo usarlo para ir más rápido y más regular.**

En PitWall corres por **carriles** (C1, C2, C3…) y vas **rotando de carril manga a manga**. Por eso hay dos formas de mirar tu carrera: **lo que pasa AHORA en esta manga** y **cómo vas a quedar AL FINAL** cuando sumes todas tus mangas. Este manual te enseña a leer ambas.

---

## 1. La pantalla en directo

![img: 20-live-timing.png]

Es la pantalla de la manga en curso. Lo que ves en tiempo real, vuelta a vuelta.

**Relojes por circuito (C1, C2, C3…).** Si la carrera usa varios circuitos a la vez, arriba tienes un reloj por cada uno. Cada reloj marca el tiempo de esa manga en ese circuito. Cuando el reloj llega a cero, esa manga termina y todos rotáis de carril.

**Tarjetas de carril.** Una tarjeta por cada coche en pista. En cada tarjeta lees, de un vistazo:

- **TOTAL** — vueltas acumuladas hasta ahora en la manga.
- **ÚLTIMA** — tu última vuelta completa. Es tu referencia inmediata: ¿mejoras o te caes?
- **MEDIA** — tu ritmo medio en la manga (media simple de tus vueltas, sin contar la de calentamiento). Es lo que de verdad manda para ganar en resistencia: no la mejor vuelta suelta, sino el ritmo sostenido.
- **MEJOR** — tu mejor vuelta válida de la manga.

**Banner de vuelta rápida.** Cuando alguien marca la vuelta más rápida del momento, salta un aviso destacado. Si es tuya, bien. Si es de un rival, es la vara de medir a batir.

### Las tres vistas del directo (botón "Vista")

Con el botón **Vista** eliges cómo se muestran las tarjetas, según cuántos carriles haya. Hay tres modos:

**1 · Filas horizontales** — una fila por carril. Recomendada para **pocos carriles**: cada carril ocupa una fila ancha y se lee muy cómodo.

![img: 31-vista-1.png]

**2 · Cuadrícula compacta** — todas las pistas a la vez en rejilla. Ideal para **muchos carriles**: lo ves todo sin desplazarte.

![img: 31-vista-2.png]

**3 · Tarjetas con detalles** — como la compacta, pero con **VLT** (vueltas), **SAL** (salidas), **PIT** y **Δ** visibles en cada tarjeta. Más información por carril de un vistazo.

![img: 31-vista-3.png]

---

## 2. Live-stats: las 3 pestañas

Live-stats es la vista de estadísticas. Tiene tres pestañas y cada una responde a una pregunta distinta.

**Manga actual.**

![img: 21-livestats-manga.png]

La clasificación de **esta** manga, con el detalle de cada piloto: **V** (vueltas), **MEJOR**, **MEDIA**, **Δ** (delta, tu margen), **SALIDAS** y **PERDIDO** (tiempo perdido en salidas). Míralo para saber cómo vas AHORA, contra quién compartes carril y quién manda en tu manga.

**Clasificación proyectada.**

![img: 22-livestats-proyectada.png]

La posición estimada **al final de la carrera**, cuando todos hayáis completado todas vuestras mangas. Es la que de verdad importa para saber si vas ganando. Míralo para saber tu posición REAL en la general, no solo en la manga que estás corriendo.

**Comparativa por carril.**

![img: 23-livestats-carril.png]

Qué rinde cada carril. Unos carriles son más rápidos que otros. Aquí ves las diferencias entre C1, C2, C3… Míralo para saber si tu carril actual te ayuda o te penaliza, y qué carriles te quedan por rodar.

**Regla rápida:** *Manga actual* = la foto de ahora. *Proyectada* = cómo acabas. *Carril* = por qué tu ritmo cambia de manga a manga.

---

## 3. Tu panel (Mi panel)

![img: 21b-livestats-mipanel.png]

Elige tu piloto y tendrás tu propio panel con tarjetas. Una a una:

**POSICIÓN.** Ojo con esta: es tu posición **PROYECTADA de carrera**, no la de la manga. Te dice dónde vas a acabar si el ritmo se mantiene. Si en tu manga vas 4º pero tu panel dice P1, es que sumando todas las mangas vas primero. Fíate de esta.

**VUELTAS MANGA.** Cuántas vueltas llevas en la manga actual.

**MEJOR.** Tu mejor vuelta válida. "Válida" significa que **no cuenta**:
- la **vuelta de calentamiento** (la primera, con el lío del semáforo y el cruce inicial),
- ni un **cruce parcial** (una vuelta que en realidad es media vuelta mal contada),
- ni tiempos **por debajo del mínimo** de la carrera (cruces fantasma imposibles).

Así que tu MEJOR es una vuelta real de verdad, nunca un número regalado.

**MEDIA.** Tu ritmo medio. Media simple de tus vueltas de carrera (incluye salidas y pit-stops; solo excluye el calentamiento). Es el número que la proyección usa para estimar dónde acabas. **Baja tu media y subes en la general.**

**Δ (delta).** Es tu **media limpia menos tu mejor vuelta**. O sea: cuánto margen te queda. Un Δ pequeño = ruedas casi siempre a tope, muy poco que rascar. Un Δ grande = tienes ritmo pero lo pierdes en muchas vueltas: ahí está tu oro, en ser más constante. La "media limpia" aquí no cuenta salidas ni pits, solo tu rodar normal.

**SALIDAS / PIT-STOPS.** Cuántas veces te has salido y cuántas paradas has hecho. Cada salida te cuesta tiempo y posiciones.

**Tiempo perdido en salidas.** Lo que te han costado esas salidas, en segundos. Ponlo en contexto: a veces una sola salida vale más posiciones que décimas de ritmo durante toda la manga. Aquí lo ves claro.

---

## 4. PitWall Lap: tu carrera en el móvil

![img: 45-lap-access.png]

**PitWall Lap** es la web que abres en el **móvil desde tu box** para seguir tu carrera en directo, sin instalar nada. Es solo para **carreras de resistencia (por equipos)**. Es de solo lectura: consultas tu timing, no controlas la carrera.

**Cómo entras.** La organización te da la dirección (algo como `http://<IP-del-servidor>:3000/lap/<carrera>`) y un **PIN de 4 dígitos** de tu equipo. Abres la dirección, eliges tu **equipo** en la lista, metes el **PIN** y pulsas **Entrar**. Con **Cambiar equipo** puedes salir y entrar con otro.

![img: 48-lap-team-panel.png]

**Tu panel.** Arriba, tu **posición** en grande: es la **proyectada** (dónde vas a acabar sumando todas las mangas), la misma que ves en el directo y en la general — no la de la manga suelta. Debajo, tu distancia al líder (*"a N vueltas"*, *"a la par"* o *"🏁 Líder de la carrera"*). La línea de estado te dice en vivo **en qué manga y carril vas y cuánto queda** (o *"En descanso"* / *"Esperando próxima manga"* / *"Carrera finalizada"*). Y las tarjetas:

- **Última vuelta** — tu última vuelta (parpadea al actualizarse).
- **Mejor vuelta** — tu mejor vuelta válida.
- **Vueltas** — total acumulado de toda la carrera.
- **Media carrera** — tu ritmo medio acumulado (el que usa la proyección).
- **Pit stops** — paradas hechas.
- **Gap al líder** — a cuántas vueltas del primero.

Si hay proyección activa, aparece **Estimación al final** con tu **posición estimada** y tus **vueltas proyectadas**.

**La voz (canta-vueltas).** Con el botón **🔊 Voz** activas el locutor (arranca **apagado**: hay que tocar la pantalla una vez para que el móvil deje sonar el audio). Te canta el **tiempo de cada vuelta**, y avisa de **cambio de posición**, **media manga**, **último minuto**, **últimos 30 s** y **fin de manga**. En **⚙️ Ajustes de voz** activas/desactivas cada aviso y, en el bloque avanzado, que cante cada X minutos tu **media de carril**, los **gaps con rivales** o la **media para subir** una posición.

**Pantalla siempre activa.** Mientras el panel esté abierto, la pantalla **no se apaga**; a los **30 segundos sin tocarla se oscurece** (para no gastar batería ni molestar), pero **la voz sigue cantando**. Toca la pantalla para iluminarla otra vez.

> Consejo: entra con el PIN, activa la **Voz**, deja el móvil en el box y escucha. Es la forma de ir informado sin despegar la vista de la pista.

## 5. Consistencia

![img: 26-livestats-cons-con.png]

La tarjeta más importante para mejorar. **La consistencia mide tu regularidad vuelta a vuelta**: si haces siempre el mismo tiempo o si das saltos.

**Qué es el %.** Es 100 menos tu variación relativa (el CV, coeficiente de variación). 100% sería un robot perfecto, siempre idéntico. Cuanto más alto, más regular. En datos reales lo normal es **entre 90% y 99%**. Es la misma fórmula que usa TicTac, calculada sobre tus vueltas de ritmo (descartando incidentes puntuales).

**El ±DE en segundos (más útil que el %).** Junto al % verás algo como *±0,13 s*. Es tu desviación típica: **cuántos segundos, arriba o abajo, oscilas de una vuelta a otra.** Fíjate más en esto que en el %: un ±0,13 s te dice de forma directa lo apretado que ruedas, y discrimina mejor entre dos pilotos que a simple vista tienen un % parecido. **Objetivo: reducir tu ±DE.**

**Niveles de color.** El sistema te clasifica según tu variación:

- **Excelente** — variación por debajo del 1,5%. Rodar de reloj.
- **Buena** — entre 1,5% y 2,5%. Sólido.
- **Irregular** — entre 2,5% y 4%. Das saltos, hay tiempo que ganar siendo más fino.
- **Errática** — por encima del 4%. Mucha inestabilidad; céntrate en terminar vueltas limpias antes que en atacar.

**Toggle: Sin salidas / Con salidas.**

- **Sin salidas** — tu **ritmo puro**. Quita salidas, pits e incidentes. Responde: *cuando ruedo bien, ¿soy regular?* Úsalo para pulir tu conducción.
- **Con salidas** — la **regularidad real de tu stint**. Incluye TODO: salidas, pits, tráfico. Responde: *de verdad, tal cual, ¿qué ritmo entregué?* Úsalo para ver el impacto real de tus errores. Suele salir peor que "Sin salidas", y esa diferencia es exactamente lo que te cuestan los incidentes.

**Mínimo de vueltas.** Hacen falta al menos **3 vueltas válidas** (que, quitando calentamiento y primera cruzada, son unas 5 vueltas dadas) para que el número sea fiable. Con menos verás un guion (—) hasta que acumules recorrido.

---

## 6. Las gráficas

Cada gráfica tiene tres modos. Cambian según lo que quieras ver.

**Tiempo por vuelta.** El clásico: cada punto es una vuelta y su tiempo. Lees la forma de tu carrera. ¿Bajas al calentar? ¿Te caes al final por el coche o por ti? ¿Un pico aislado (una salida) o una tendencia? Sirve para ver dónde ganas y dónde pierdes a lo largo del stint.

**Sobre la media.**

![img: 24-livestats-chart-media.png]

Aquí cada vuelta se dibuja como diferencia respecto a tu media: por encima = vuelta más lenta, por debajo = más rápida. Es la mejor vista de la **consistencia**: cuanto más plana y pegada al cero esté tu línea, más regular eres. Los picos hacia arriba son tus vueltas malas. Objetivo visual: aplanar la línea.

**Gap de vueltas.**

![img: 25-livestats-chart-gaplaps.png]

Tu distancia al líder a lo largo del tiempo (eje X = minutos de la manga; eje Y = gap al líder que elijas). Sube = pierdes terreno; baja = recortas. Sirve para ver EN QUÉ MOMENTO de la manga ganaste o perdiste la carrera, y si el hueco es estable o se te escapa.

---

## 7. Proyección y gaps

![img: 22-livestats-proyectada.png]

**Posición proyectada vs posición de manga.** Son cosas distintas y las dos importan:

- **De manga** — dónde vas en la manga que corres ahora. Útil para tu duelo directo en pista.
- **Proyectada** — dónde vas a acabar la carrera sumando todas las mangas. Es tu posición REAL en la general. La proyección estima tus vueltas totales dividiendo el tiempo total de carrera entre tu media. **Bajar tu media = mejor proyección.**

Importante: la posición proyectada es **la misma en todas partes** (tarjeta del directo, Clasificación General y panel Lap). Si en un sitio ves P2, en todos ves P2. No hay dos verdades.

**Tipos de gap.**

- **Gap al líder** — a cuánto estás del primero.
- **Gap por vueltas** — la distancia expresada en vueltas (más intuitivo en resistencia: "voy a una vuelta").
- **Gap por minuto** — cómo evoluciona la distancia con el tiempo, para ver si recortas o te descuelgas.

Cuando dos pilotos tienen las mismas vueltas, desempata la **coma**: la fracción de vuelta que llevabas hecha justo al caer la bandera. Rodar apurado hasta el final puede darte esa fracción de más que te sube una posición.

---

## 8. La vista de Resultados (después de la carrera)

Cuando la carrera termina, **Resultados** es donde se analiza todo con calma. Tiene varias **pestañas**; cada una responde a una pregunta distinta. Arriba siempre ves la **vuelta rápida de la carrera** (quién y en qué carril).

### Comparativa (la parrilla por carril)

![img: st-comparativa.png]

Es la tabla principal. Una fila por participante y, para **cada carril** por el que pasó, cinco datos apilados:
- **Rápida** — tu mejor vuelta en ese carril. El punto azul + **MEJOR** marca la vuelta rápida *de ese carril* entre todos.
- **Media** — tu ritmo medio en ese carril.
- **Const. sin** — tu **consistencia** (sin salidas) en ese carril, en %.
- **Salidas** — cuántas te saliste ahí (y, debajo, el tiempo perdido).
- **Pit-stops** — paradas en ese carril (con el nº de vuelta, p.ej. *V355*).

Sirve para ver **en qué carriles rindes mejor o peor**, no solo tu número global. El rectángulo azul marca tu **carril de salida**.

**Carreras de pasadas / repetir-carril.** Si el mismo carril se corre varias veces, cada carril se **desdobla por ocurrencia** (`1/2`, `2/2`…), para comparar tu 1ª pasada con la 2ª por el mismo sitio.

![img: st-ocurrencia.png]

### Progresión (vuelta a vuelta)

![img: st-progresion.png]

Cada vuelta de la carrera, en orden. Puedes **elegir a quién comparar**, filtrar por **manga** o por **carril**, y mostrar/ocultar **salidas** (puntos rojos) y **pit-stops** (naranjas). Con el botón **Δ Delta vs media** cada vuelta se dibuja como diferencia respecto a tu media (mejor vista para juzgar tu regularidad: cuanto más plana, mejor). Responde: *¿bajé al calentar? ¿me caí al final? ¿fue un pico aislado o una tendencia?*

### Posiciones

![img: st-posiciones.png]

Una línea por participante; el eje vertical es la **posición** (P1 arriba). Si tu línea sube, pierdes posiciones; si baja, ganas. Sirve para ver **en qué momento** de la carrera se decidió tu resultado.

### Gap al líder

![img: st-gap.png]

Tu distancia al líder **a lo largo del tiempo** (puedes acotar el rango de mangas). La línea que baja = te acercas; que sube = te alejas. Responde: *¿en qué manga me descolgué o recuperé?*

### Gap (rejilla)

![img: st-gapgrid.png]

La misma idea pero en **tabla**: filas = equipos, columnas = mangas, y cada celda las **vueltas de desventaja** al cierre de esa manga (0 = líder). El **borde dorado** avisa de que hubo **pit-stop** en esa manga. Puedes elegir 2–4 equipos para ver el gap **entre ellos** (no solo contra el líder).

### Estadísticas avanzadas

![img: st-avanzadas.png]

El análisis profundo de un participante: **total de vueltas** (y limpias), **mejor**, **media** (con toggle *con/sin salidas*), **Δ consistencia**, **salidas · pit-stops** y **tiempo perdido**. Debajo, la **evolución por carril** (tu media pista a pista, para ver dónde fuiste más rápido) y una tarjeta por carril. Con **Comparar con** eliges un rival y se genera una tabla **cara a cara** con las diferencias coloreadas (verde = mejor, rojo = peor).

### Clasificación Le Mans (equipos)

![img: st-lemans.png]

En carreras por equipos existe además la **clasificación Le Mans**: la general en grande, con **vueltas proyectadas**, total, **gap** al líder, media, mejor y **P/Subir** (el ritmo que necesitarías para cazar al de delante). Ideal para carreras largas.

> **Iconos y colores que verás:** punto azul + **MEJOR** = vuelta rápida de ese carril · rectángulo azul = carril de salida · **borde dorado** = hubo pit-stop en esa manga · tendencia **▲/▼** = subiste/bajaste respecto a la manga anterior.

## 9. Glosario

- **Consistencia** — tu regularidad vuelta a vuelta. 100 menos tu variación relativa. Más alto = más constante.
- **±DE (desviación típica) / CV** — el ±DE son los segundos que oscilas de vuelta a vuelta (mira este número). El CV es esa oscilación en porcentaje relativo a tu ritmo; el % de consistencia es 100 − CV.
- **Media** — media simple de tus tiempos de vuelta, sin la de calentamiento. Incluye salidas y pits. Es la que usa la proyección.
- **Media limpia** — tu media contando solo vueltas normales (sin salidas). Se usa para el Δ y para detectar incidentes, no para proyectar.
- **Warmup (vuelta de calentamiento / cruce parcial)** — la primera vuelta real de la manga, con artefactos del semáforo y el cruce inicial. No cuenta para media, mejor ni consistencia.
- **Sub-mínimo** — un tiempo por debajo del mínimo de vuelta de la carrera. Cruce fantasma imposible; se descarta siempre.
- **Salida (exit)** — te has salido de pista. Cuenta para la media (es tiempo real perdido) pero no para tu mejor vuelta.
- **Pit-stop** — parada en boxes. Cuenta como tiempo, no como mejor vuelta.
- **Coma** — la fracción de vuelta que llevabas al caer la bandera. Desempata cuando dos tenéis las mismas vueltas.
- **Proyección** — estimación de tu resultado final sumando todas las mangas: tiempo total de carrera dividido entre tu media.
- **Gap** — tu distancia a otro coche (o al líder), en tiempo, en vueltas o por minuto.
- **PitWall Lap** — la web móvil de tu equipo (acceso por PIN): tu posición proyectada, tus tarjetas de ritmo y la voz que canta las vueltas. Solo en carreras por equipos.
- **Ocurrencia** — cada vez que corres el mismo carril en carreras de pasadas/repetir-carril (`1/2`, `2/2`…); permite comparar una pasada con otra.
- **P/Subir** — en la clasificación Le Mans, el ritmo (media por vuelta) que necesitarías para alcanzar al equipo de delante.
- **Carril de salida** — el carril desde el que arrancaste; en la parrilla de resultados se marca con un recuadro azul.

---

**En una frase:** mira tu **posición proyectada** para saber dónde acabas, baja tu **media** para subir, y aplana tu **consistencia** (reduce el ±DE) para dejar de regalar tiempo vuelta a vuelta.
