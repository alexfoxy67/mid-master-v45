# MID MASTER V4.5 — primera versión funcional

## Incluye
- Aplicación web adaptable a móvil y escritorio.
- Cálculo reproducible de matriz de marcadores mediante Poisson independiente.
- Probabilidades 1X2, BTTS y over/under derivadas de la matriz.
- Historial local, exportación/importación JSON y auditoría postpartido.
- Modo instalable PWA cuando se sirve desde HTTPS y el navegador lo admite.

## Límites transparentes
- No hay proveedor de datos deportivos conectado.
- Los λ y valoraciones cualitativas son entradas manuales, no predicciones automáticas provenientes de fuentes.
- No scrapea Score365 ni afirma que un XI está confirmado sin que el usuario lo registre.
- La auditoría registra métricas; no ajusta parámetros automáticamente ni declara mejora a partir de una sola muestra.
- Para una app nativa iOS (.ipa) se necesita un proyecto iOS/Xcode, firma de Apple y distribución autorizada. Este paquete es una PWA inicial, no una .ipa.

## Ejecutar
Abre `index.html` en un navegador moderno. Para instalar como PWA, súbelo a un hosting HTTPS y abre la URL en Safari; usa Compartir > Añadir a pantalla de inicio. El modo offline requiere que el navegador registre el service worker desde HTTPS.

## Próximas etapas
1. Elegir proveedor de datos/licencia y API para fixtures, resultados, estadísticas y alineaciones.
2. Crear backend seguro para proteger API keys; no incrustar secretos en el cliente.
3. Implementar ingesta con fuente, hora, estado de verificación y manejo de datos faltantes.
4. Completar módulos MID cualitativos con reglas trazables y datos observables.
5. Ejecutar backtests temporales (Brier, Log Loss, calibración, MAE de goles) antes de cambiar el modelo.
6. Crear wrapper nativo iOS y firma/distribución cuando exista cuenta y entorno Apple adecuados.
