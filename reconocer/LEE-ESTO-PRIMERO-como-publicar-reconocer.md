# 🔴 LEE ESTO PRIMERO · Cómo hacer que el código QR de «Reconocer» funcione

## Por qué el QR no te abre nada

El código está bien hecho y apunta a la dirección correcta. Lo que pasa es que
**esa dirección todavía no existe en internet**: el aplicativo está en un archivo de tu
computador, no en una página web publicada.

Piénsalo así: el QR es la dirección de una casa. La dirección está bien escrita, pero la casa
todavía no está construida. Eso es lo que vas a hacer ahora y toma unos diez minutos.

**Importante:** yo no puedo publicar la página por ti. No tengo forma de crear cuentas ni de
subir archivos a internet. La publicación la tiene que hacer una persona de la Secretaría. Lo
que sí hice fue dejar todo listo y los códigos ya calculados para la dirección de la Opción A.

---

## La dirección que quedó grabada en el QR

Los códigos y el afiche que te entregué apuntan a:

**`https://saludvaupes.github.io/reconocer/`**

Si sigues la **Opción A** tal cual, no tienes que regenerar nada: el QR impreso funcionará
apenas subas el archivo. Si prefieres otra dirección, usa la **Opción B** y vuelve a generar
los códigos con la herramienta incluida.

---

## Opción A · GitHub Pages · **RECOMENDADA**

Es gratis, no caduca y **el QR que ya tienes queda funcionando sin cambiar nada**.

### Paso 1 · La cuenta

Si la Secretaría ya tiene la cuenta `saludvaupes` de la campaña de prevención del suicidio,
**salta al Paso 3**: vas a agregar esta página al mismo sitio.

Si no la tienen todavía:

1. Entra a **github.com** y pulsa *Sign up*.
2. En «Username» escribe exactamente: **`saludvaupes`**

   ⚠️ Tiene que ser idéntico, en minúsculas y sin espacios. El nombre de usuario es parte de la
   dirección web: si escribes otro, los QR impresos dejan de servir.
3. Completa el correo institucional y la contraseña. Confirma el correo que te llega.

### Paso 2 · El repositorio

1. Arriba a la derecha, pulsa el **+** → *New repository*.
2. En «Repository name» escribe exactamente: **`saludvaupes.github.io`**

   ⚠️ También idéntico. Ese nombre especial hace que el sitio quede en la raíz, que es donde
   apuntan los códigos.
3. Marca **Public** y pulsa *Create repository*.

### Paso 3 · Subir la página

1. En tu computador, crea una carpeta nueva en el escritorio y llámala exactamente
   **`reconocer`** (minúsculas, sin tildes, sin espacios).
2. Mete dentro el archivo **`index.html`** que te entregué. La carpeta debe quedar así:

   ```
   reconocer/
     index.html
   ```

   ⚠️ No le cambies el nombre al archivo. Si se llama distinto, la dirección deja de funcionar.
3. En GitHub, entra al repositorio `saludvaupes.github.io` y pulsa
   **Add file** → *Upload files*.
4. **Arrastra la carpeta `reconocer` completa** al recuadro. GitHub conserva la carpeta y verás
   aparecer la ruta `reconocer/index.html`.
5. Abajo pulsa el botón verde *Commit changes*.

### Paso 4 · Activar la publicación

Si ya lo hiciste antes para la otra campaña, esto ya está activo y puedes saltar al Paso 5.

1. Arriba, entra a **Settings** → en el menú de la izquierda, **Pages**.
2. En «Source» elige *Deploy from a branch*.
3. En «Branch» elige **`main`** y la carpeta **`/ (root)`**. Pulsa *Save*.
4. Espera entre uno y tres minutos.

### Paso 5 · Comprobar

Abre en el celular: **https://saludvaupes.github.io/reconocer/**

Si ves la portada morada con la frase «Ponerle nombre es empezar a salir», ya está publicado.
Ahora escanea el QR del afiche con **dos celulares distintos**: debe abrir esa misma página.

> **¿Sigue saliendo «404 · There isn't a GitHub Pages site here»?**
> Casi siempre es una de tres cosas: no pasaron los tres minutos, el archivo no se llama
> `index.html`, o quedó suelto en la raíz en vez de dentro de la carpeta `reconocer`.
> Entra al repositorio y confirma que ves la ruta `reconocer/index.html`.

---

## Opción B · Si prefieren el dominio de la Gobernación

Es la vía más institucional y la mejor a largo plazo, porque la dirección es suya para siempre.

1. Pide al área de TIC o de comunicaciones que suba `index.html` al portal, por ejemplo en
   `https://vaupes.gov.co/reconocer/`. Diles que es una página autónoma de un solo archivo, sin
   base de datos ni dependencias, y que no recoge datos de los usuarios.
2. Cuando te confirmen la dirección, abre con doble clic el archivo
   **`generador-qr-afiche.html`**. Se abre en el navegador y funciona sin internet.
3. Borra la dirección de ejemplo y escribe la definitiva. El QR y el afiche se actualizan solos
   mientras escribes.
4. Descarga lo que necesites: **QR en PNG** para documentos, **QR en SVG** para la imprenta,
   **Afiche en PDF** para imprimir, **Afiche en PNG** para redes.

⚠️ **Muy importante:** las piezas impresas con el QR anterior quedan desactualizadas. Si ya
mandaste a imprenta con la dirección de la Opción A y luego cambias a la Opción B, hay que
reimprimir. Por eso conviene decidir la dirección **antes** de imprimir.

💡 **El truco para no reimprimir nunca:** pide a TIC que `https://vaupes.gov.co/reconocer/`
redirija a donde esté alojada la página. Ese día puedes mover el aplicativo de servidor las
veces que quieras y los afiches siguen sirviendo.

---

## Opción C · Si necesitan algo funcionando hoy mismo

1. Crea una carpeta llamada `reconocer` con el archivo `index.html` adentro.
2. Entra a **app.netlify.com/drop** y arrastra la carpeta.
3. En segundos te da una dirección activa, algo como `https://alegre-tucan-4821.netlify.app`.
4. Crea la cuenta gratuita cuando lo pida: si no lo haces, el sitio se borra a las 24 horas.

Sirve para mostrar el aplicativo en una reunión o probarlo con el equipo, pero la dirección es
aleatoria. **Antes de imprimir** hay que fijar la dirección definitiva y regenerar los códigos
como se explica en la Opción B.

---

## Qué archivo es cada uno

| Archivo | Para qué sirve | ¿Va a internet? |
| --- | --- | --- |
| `index.html` | El aplicativo completo. Es el único que se sube | **Sí** |
| `generador-qr-afiche.html` | Crea el QR y el afiche para cualquier dirección | No, doble clic |
| `afiche-reconocer-vaupes.pdf` | Afiche A4 listo para imprenta (dirección de la Opción A) | No |
| `qr-reconocer-vaupes.png` y `.svg` | El QR suelto, para otras piezas gráficas | No |

El aplicativo lleva adentro los logos, las tipografías, los textos y la programación. No
necesita base de datos, ni servidor especial, ni instalación. Cualquier servicio que muestre
páginas web sirve.

---

## Antes de mandar a imprenta

- [ ] La página abre desde un celular con **datos móviles**, no solo con el wifi de la oficina
- [ ] Abre bien en Android y en iPhone
- [ ] El QR escanea con **dos celulares distintos** y lleva al aplicativo
- [ ] El botón rojo **Salir rápido** cierra la página
- [ ] Los botones de llamada de la sección de líneas marcan el número correcto
- [ ] Las nueve fichas de tipos de violencia abren y cierran
- [ ] El ejercicio de situaciones avanza y corrige
- [ ] El autodiagnóstico llega a un resultado con plan de pasos
- [ ] Las tres puertas de la ruta abren su línea de tiempo
- [ ] Los siete números de las líneas están verificados y vigentes
- [ ] Imprimiste una prueba en papel y la escaneaste desde 40 cm

Por si el QR falla, **el afiche lleva la dirección escrita en letra debajo del código**, para
que cualquier persona pueda escribirla en el navegador.

---

## Dos cosas para cuidar en el tiempo

**Para actualizar el aplicativo** (cambiar un número, un texto, una entidad): sube el archivo
corregido con el mismo nombre y en la misma ruta. La dirección no cambia, así que el QR impreso
sigue sirviendo y no hay que reimprimir nada.

**Sobre la privacidad:** el aplicativo no guarda ni envía nada, y eso está escrito en la
pantalla. Si alguien le agrega analítica, formularios, pixeles de seguimiento o un chat externo,
esa promesa deja de ser cierta y pone en riesgo a quien lo usa. Si necesitan medir, cuenten
visitas en el servidor o descargas del afiche, nunca lo que la persona escribe.

---

## Dónde pegar el afiche

Una recomendación de contenido, no de técnica: pégalo donde la gente pueda mirarlo **sin ser
observada**. Una sala de espera, un pasillo, la puerta interior de un baño o el consultorio
funcionan mejor que una cartelera central a la vista de todos. Quien está viviendo violencia
necesita poder escanear sin que nadie la vea hacerlo.
