# FamiliTV - Redireccionador GitHub Pages

URL pública fija: `https://skerrigan05.github.io/familitv`

Esta página redirige al túnel actual de Cloudflare donde corre FamiliTV.

## ¿Por qué existe esto?

Los quick tunnels de Cloudflare (`cloudflared tunnel --url`) generan una URL aleatoria cada vez que se reinicia. Esta página permite tener una URL fija en GitHub Pages que apunta siempre al túnel activo.

## Cómo actualizar cuando cambie el túnel

### Opción 1: Editar directamente en GitHub (más fácil)

1. Ve a `https://github.com/skerrigan05/familitv`
2. Abre el archivo `index.html`
3. Haz clic en el lápiz ✏️ ("Edit this file")
4. Reemplaza **todas** las URLs antiguas por la nueva URL del túnel
5. Haz scroll abajo y presiona "Commit changes..."
6. Espera 1-2 minutos y la URL fija redirigirá al nuevo túnel

### Opción 2: Actualizar desde tu PC con git

```bash
cd familitv-github
# editar index.html con la nueva URL
git add index.html
git commit -m "Actualizar URL del tunel"
git push origin main
```

## Canales disponibles

- TVN
- Mega
- Canal 13
- Chilevisión (CHV)
- La Red
