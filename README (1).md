# Mi web, editable desde el navegador

Toda la página es un solo archivo: `index.html`. El editor viene incluido y los visitantes no lo ven.

## 1. Publicarla en GitHub Pages (una sola vez)

1. En GitHub, creá un repositorio **público**.
   - Si lo llamás `TU-USUARIO.github.io`, la web queda en `https://TU-USUARIO.github.io/`.
   - Con cualquier otro nombre (por ejemplo `web`), queda en `https://TU-USUARIO.github.io/web/`.
2. Subí `index.html` (y este README si querés): **Add file → Upload files → Commit changes**.
3. Andá a **Settings → Pages**. En *Build and deployment*, elegí **Deploy from a branch**, rama **main**, carpeta **/ (root)** y tocá **Save**.
4. En 1 o 2 minutos la página está en línea.

## 2. Editar

1. Abrí tu página con `?editar` al final, por ejemplo `https://TU-USUARIO.github.io/web/?editar`
   (también podés usar Ctrl/Cmd + Shift + E).
2. Hacé clic en cualquier texto para cambiarlo. Pasá el mouse sobre tarjetas y secciones para moverlas,
   duplicarlas, ocultarlas o borrarlas. El botón **Diseño** cambia colores, tipografía y bordes.
3. Los cambios se guardan solos en tu navegador mientras trabajás.

## 3. Publicar los cambios

La primera vez que tocás **Publicar**, te pide conectar GitHub:

1. Usuario, repositorio y rama se completan solos.
2. Creá un token en <https://github.com/settings/personal-access-tokens/new>:
   - **Repository access:** *Only select repositories* → el repositorio de tu web.
   - **Permissions → Repository permissions → Contents:** *Read and write*.
   - **Generate token**, copialo y pegalo en el editor.
3. Listo. Desde ahí, **Publicar** guarda directo en GitHub y la web se actualiza en 1 o 2 minutos.

El token queda guardado solo en ese navegador; nunca se publica dentro de la página.
En otro dispositivo (por ejemplo, el celular) hay que pegarlo una vez más.
Si lo perdés o vence, borralo en GitHub y creá otro.

## 4. Notas privadas

Las notas con candado son **privadas**: no se publican en la página. Se guardan en un archivo `notas.json`
dentro de un segundo repositorio **privado** (por ejemplo `miweb-notas`), y solo las ves vos, con GitHub conectado.

Para que funcione (una sola vez):
1. En GitHub, creá un repositorio nuevo **privado** llamado `miweb-notas` (podés marcar *Add a README*).
2. Editá tu token en <https://github.com/settings/personal-access-tokens> y en *Repository access* sumá `miweb-notas`
   (así el token tiene acceso a los dos repositorios, con *Contents: Read and write*).
3. En el editor, menú **⋯ → Conexión con GitHub**: revisá que diga `miweb-notas` y tocá **Probar y guardar**.
4. Tocá **Publicar**. Las notas privadas pasan a `miweb-notas` y salen de la página pública.

Cada nota se cambia desde su manija **⋮⋮ → Hacer pública / Hacer privada**. Las notas nuevas empiezan como privadas.
Si el repositorio privado no está disponible, el editor no publica nada, para que no se pierdan notas.

## Bueno saber

- **Siempre editás la última versión.** Al entrar al editor, se trae la versión publicada más reciente directo de GitHub,
  aunque GitHub Pages todavía muestre una anterior por caché.
- **Cambios sin publicar:** si cerrás sin publicar, al volver los encontrás donde los dejaste (en ese mismo navegador).
- **Historial:** cada vez que publicás queda un commit en GitHub, así que siempre podés volver a una versión anterior desde ahí.
- **Copia de respaldo:** en el menú **⋯** del editor está **Descargar HTML** (sin las notas privadas).
- Si publicaste desde otro dispositivo mientras tenías el editor abierto, te avisa antes de reemplazar esa versión.
