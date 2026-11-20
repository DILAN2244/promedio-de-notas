# Promedio de Notas

Calculadora académica gratuita y aplicación web progresiva (PWA).

## Funciones
- Promedio simple con evaluaciones completadas y pendientes.
- Promedio ponderado por porcentajes.
- Estimación de la nota promedio necesaria para alcanzar una meta configurable (3.0 por defecto).
- Guardado local en el navegador.
- Exportación de notas a CSV.
- Guía educativa con ejemplos y preguntas frecuentes.
- Diseño adaptable a celular y computador.
- Caché para uso sin conexión después de la primera visita.

## Publicación con GitHub Pages
1. Abre **Settings → Pages**.
2. En **Build and deployment**, selecciona **Deploy from a branch**.
3. Elige la rama **main** y la carpeta **/(root)** y guarda.
4. Espera a que finalice la publicación.

URL esperada: https://dilan2244.github.io/promedio-de-notas/

## Privacidad
Las notas se guardan en LocalStorage del navegador. No hay cuentas, backend ni sincronización en esta versión. Consulta [Política de privacidad](./privacidad.html) y [Términos de uso](./terminos.html).

## Tecnologías
HTML, CSS, JavaScript, LocalStorage, Web App Manifest y Service Worker.

## Monetización
Esta versión todavía no contiene anuncios, pagos ni funciones premium. Antes de incorporar publicidad, revisa las políticas del proveedor, privacidad, consentimiento aplicable y requisitos de edad de la cuenta publicitaria. No se deben presentar funciones como premium hasta que estén implementadas y probadas.

## Comprobaciones manuales recomendadas

- Meta configurable: cambiarla a 4.0 debe actualizar el texto y el cálculo de nota necesaria; al recargar, la meta debe conservarse.
- Promedio simple: 4.0, 3.0 y 5.0 deben dar 4.00.
- Promedio ponderado: 4.0 al 40% y 3.0 al 60% deben dar 3.40.
- Nota pendiente: 4.0 al 40% y 60% restante deben requerir 2.33 para llegar a 3.0.
- Validación: comprobar que se rechacen notas fuera de 0 a 5 y porcentajes totales superiores al 100%.
- Exportación: probar nombres que comiencen con `=`, `+`, `-` o `@` y verificar que se exporten como texto.
- Modo sin conexión: abrir la aplicación y la guía una vez, desconectarse y comprobar que ambas páginas carguen.
