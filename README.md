# ClickSon · Demo Menú Digital Food Park

Demo funcional para pitch. Flujo completo: QR → bienvenida → restaurante → menú → carrito → mesa → pago → comanda a cocina (WhatsApp simulado). Cobro y WhatsApp están simulados para presentación.

## Correr en local
```bash
npm install
npm run dev
```
Abre el link que aparezca (normalmente http://localhost:5173).

## Publicar (link para compartir con clientes / Raúl)

### Opción A — Vercel (recomendado, gratis)
1. Sube esta carpeta a un repo de GitHub, o instala Vercel CLI.
2. Con CLI:
   ```bash
   npm i -g vercel
   vercel
   ```
3. Vercel detecta Vite solo. Da un link tipo `clickson-foodpark.vercel.app`.
4. Sin logo de terceros. Se abre en el navegador de cualquier celular.

### Opción B — Netlify
1. `npm run build`
2. Arrastra la carpeta `dist/` a https://app.netlify.com/drop
3. Te da un link al instante.

## Notas para el pitch
- La vista "Cocina" guarda pedidos en el mismo dispositivo (no se sincroniza entre celulares). Para la demo, haz el pedido en el mismo teléfono donde muestres la cocina.
- Para producción real (Stripe, WhatsApp Cloud API, panel del food park, menús cargables por restaurante) se conecta al backend de ClickSon.

## Personalizar
- Restaurantes, platillos y precios: edita el array `RESTAURANTS` al inicio de `src/App.jsx`.
- Nombre del food park: objeto `PARK`.
- Colores de marca: objeto `BRAND`.
