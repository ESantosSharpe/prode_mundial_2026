# 🏆 PRODE Mundial 2026

Aplicación web para el prode de la fase de grupos del Mundial de Fútbol 2026. Cada jugador carga sus pronósticos, los bloquea antes del inicio del torneo, y la tabla de posiciones se actualiza automáticamente a medida que se cargan los resultados reales.

---

## Cómo jugar

### Registro
1. Entrá a la URL del prode
2. Hacé clic en **"+ Registrarme como nuevo jugador"**
3. Elegí un nombre o apodo y un PIN de al menos 4 caracteres
4. Guardá bien tu PIN — lo vas a necesitar para volver a entrar

### Cargar pronósticos
- Para cada partido elegís **1** (gana el local), **X** (empate) o **2** (gana el visitante)
- Podés guardar borradores las veces que quieras con **"Guardar borrador"**
- Cuando estés conforme con todos tus pronósticos, usá **"🔒 Enviar pronósticos"**
- **¡Atención!** Una vez enviados quedan bloqueados definitivamente. No se pueden modificar

---

## Sistema de puntos

| Resultado | Puntos |
|-----------|--------|
| Acierto (1, X o 2) | **1 punto** |
| Bonus grupo completo (los 6 partidos bien) | **+3 puntos** |

- **72 partidos** en la fase de grupos → máximo **72 puntos base**
- **12 grupos** × 3 puntos bonus → máximo **36 puntos extra**
- **Puntaje máximo posible: 108 puntos**

---

## Premios

| Puesto | Premio |
|--------|--------|
| 🥇 1° puesto | 70% del pozo |
| 🥈 2° puesto | 30% del pozo |

El pozo se calcula automáticamente según la cantidad de jugadores que hayan pagado la cuota.  
En caso de empate en algún puesto, el premio se divide en partes iguales entre los empatados.

---

## Los 12 grupos

| Grupo | Equipos |
|-------|---------|
| A | México · Corea del Sur · Sudáfrica · Rep. Checa |
| B | Canadá · Suiza · Qatar · Bosnia-Herz. |
| C | Brasil · Marruecos · Escocia · Haití |
| D | EE.UU. · Paraguay · Australia · Turquía |
| E | Alemania · Curazao · Costa de Marfil · Ecuador |
| F | Países Bajos · Japón · Túnez · Suecia |
| G | Bélgica · Egipto · Irán · Nueva Zelanda |
| H | España · Cabo Verde · Arabia Saudita · Uruguay |
| I | Francia · Senegal · Noruega · Irak |
| J | Argentina · Argelia · Austria · Jordania |
| K | Portugal · Colombia · Uzbekistán · RD Congo |
| L | Inglaterra · Croacia · Ghana · Panamá |

---

## Para el organizador (admin)

El panel de administración es accesible con el PIN **2026** desde la pantalla de login.

Desde el panel podés:
- **Marcar pagos**: indicar quién efectivamente pagó la cuota (el pozo se actualiza solo)
- **Cargar resultados**: ingresar el resultado real de cada partido (1 / X / 2) a medida que se juegan
- **Desbloquear jugadores**: si alguien necesita corregir sus pronósticos antes del inicio
- **Configurar la cuota**: el monto por jugador que define el pozo total
- **Eliminar jugadores**: en caso de que alguien se haya registrado por error

### Carga de resultados
Los resultados se cargan desde la pestaña **"Resultados ⚙"** (visible solo para el admin).  
Cada partido tiene los mismos botones **1 / X / 2**. Una vez cargado el resultado, la tabla y las estadísticas se actualizan automáticamente para todos.

---

## Tecnología

- Aplicación de página única en HTML/CSS/JavaScript puro — sin frameworks
- Base de datos: [JSONBin.io](https://jsonbin.io) (almacenamiento JSON gratuito vía API REST)
- Hosting: GitHub Pages
- Los PINs de los jugadores se almacenan hasheados, nunca en texto plano

---

## Actualizar la app

Si hay una nueva versión del archivo `index.html`:

1. Abrí el archivo localmente en tu navegador
2. Completá el setup con tu Master Key de JSONBin (el Bin ID existente se reutiliza)
3. Descargá el archivo configurado
4. En este repositorio, abrí `index.html` → lápiz ✏️ → reemplazá el contenido → "Commit changes"

La URL pública no cambia.

---

*Mundial 2026 — Estados Unidos, Canadá y México — 11 de junio al 19 de julio de 2026*
