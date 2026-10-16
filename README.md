# Modo Anti-Celular · demo en navegador

Experimento de visión por computadora que detecta la categoría `cell phone` de COCO-SSD en la cámara y muestra una advertencia mientras el teléfono aparece en el encuadre. La inferencia se ejecuta en el navegador con TensorFlow.js; no hay backend en este repositorio.

## Probar

Ejecutar `python -m http.server 5500` en este directorio y abrir `http://127.0.0.1:5500`. Permitir la cámara y pulsar iniciar. El navegador descarga TensorFlow.js y COCO-SSD desde CDN, por lo que se requiere Internet.

## Límites

- Solo detecta teléfonos visibles en cámara y puede fallar con oclusiones, distancia o iluminación difícil.
- No impide el uso del teléfono; únicamente muestra una advertencia en la interfaz.
- Los fotogramas se procesan localmente en el navegador según el código actual. Antes de usarlo con otras personas, obtener consentimiento para activar la cámara.
- Es una demo, no una herramienta de disciplina, vigilancia o evaluación de personas.

El código se extrajo del ZIP original para que sea navegable desde GitHub.
