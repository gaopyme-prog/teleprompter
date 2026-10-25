# Teleprompter de ponencia

Teleprompter web para ponencias virtuales: muestra las diapositivas junto al guion, que se desplaza solo. No necesita instalación ni servidor, solo un navegador.

## Qué hace

- Carga diapositivas desde un PDF o desde imágenes.
- Reparte el guion por diapositiva (separado con `---` o con líneas "Diapositiva 3").
- Texto con desplazamiento automático, velocidad y tamaño de letra ajustables, guía de lectura y modo espejo.
- Cronómetro con tiempo asignado y estimación de duración según palabras por minuto.
- Vista "Solo diapositiva" para compartir una pestaña en Meet, Zoom o Teams, mientras el guion se lee en otra pestaña. Ambas cambian de diapositiva a la vez.

## Uso

1. Abre la página y sube el PDF de la presentación.
2. Pega el guion y pulsa "Repartir en diapositivas".
3. Pulsa "Presentar".

Atajos: `Espacio` inicia o pausa, `←` `→` cambian de diapositiva, `↑` `↓` mueven el texto, `+` `-` cambian la velocidad, `M` espejo, `F` pantalla completa, `Esc` salir.

Todo se guarda en el navegador (no se sube a ningún servidor). Usa el mismo navegador para preparar y para presentar.

## Publicar en GitHub Pages

1. Sube estos archivos a un repositorio de GitHub.
2. En el repositorio: Settings → Pages → Source: "Deploy from a branch" → Branch: `main` y carpeta `/ (root)` → Save.
3. Espera uno o dos minutos. La página queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/`.

## Probar en el computador

Abre `index.html` con doble clic. Si el navegador no guarda las diapositivas al abrirlo así, usa un servidor local:

```
python3 -m http.server 8000
```

y entra a `http://localhost:8000`.

## Notas

- Necesita internet para cargar el lector de PDF (pdf.js) y las tipografías desde sus CDN.
- Funciona mejor en Chrome, Edge o Firefox actualizados.
