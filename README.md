# Mis Propiedades

App web para llevar el control de casas, departamentos, cocheras y locales:

- alta, edición y baja de propiedades;
- ocupación: uso propio, vacía, alquilada directo o alquilada por inmobiliaria;
- datos del inquilino o de la inmobiliaria (con comisión);
- contrato: fechas, monto, moneda, índice y frecuencia de ajuste, depósito;
- impuestos, servicios y expensas de cada propiedad con su **link de pago**;
- **avisos** de contratos por vencer, ajustes de alquiler y pagos vencidos o próximos;
- calendario de los próximos 12 meses, rentabilidad bruta anual y costo mensual de lo vacío;
- respaldo: exportar e importar todos los datos en un archivo `.json`.

Es un solo archivo (`index.html`), sin instalación ni servidor.

## Cómo correrla en tu computadora

1. Descargá `index.html`.
2. Abrilo con doble clic. Se abre en tu navegador (Chrome, Firefox, Edge o Safari).

Listo. Los datos se guardan **en ese navegador, en esa computadora**. Si borrás los datos de navegación o abrís la app en otro navegador o equipo, no los vas a ver. Para no perder nada, usá **Exportar respaldo** de vez en cuando y guardá el archivo en un lugar seguro. Con **Importar** los recuperás o los pasás a otro equipo.

### Opcional: con un servidor local

Si preferís abrirla en una dirección `http://localhost`:

```bash
# con Python
python3 -m http.server 8000
# o con Node
npx serve .
```

Después entrá a <http://localhost:8000>.

## Publicarla gratis con GitHub Pages

1. En el repositorio de GitHub, andá a **Settings → Pages**.
2. En **Build and deployment**, elegí **Deploy from a branch**, rama `main`, carpeta `/ (root)` y tocá **Save**.
3. En uno o dos minutos queda online en `https://TU-USUARIO.github.io/mis-propiedades/`.

Aunque esté publicada, cada persona que la abre ve **solo los datos de su propio navegador**. Nadie más ve tus propiedades.

> Si dejás el repositorio público, el **código** queda visible para cualquiera. Tus datos no se suben a GitHub, salvo que subas un archivo de respaldo `.json` (no lo hagas).

## Versión dentro de Claude

La versión publicada en Claude usa una base de datos en la nube y además tiene:

- permisos: solo el dueño edita y los demás ven en modo lectura;
- un asistente con IA;
- avisos diarios al celular.

Esta versión independiente es más simple: guarda todo localmente y no incluye el asistente.
