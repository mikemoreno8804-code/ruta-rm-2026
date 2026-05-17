# 📱 Ruta RM 2026 — Guía de instalación como PWA

## Archivos del proyecto
```
index.html      ← La app principal
manifest.json   ← Configuración PWA
sw.js           ← Service worker (modo offline)
icon-192.png    ← Ícono app
icon-512.png    ← Ícono app (alta resolución)
```

---

## Paso 1 — Crear repositorio en GitHub

1. Ve a https://github.com/new
2. Nombre del repo: `ruta-rm-2026` (o el que quieras)
3. Visibilidad: **Public** ← GitHub Pages gratis requiere público
   _(nadie lo va a encontrar si no compartes el link)_
4. Clic en **Create repository**

---

## Paso 2 — Subir los archivos

### Opción A — Desde la web (más fácil)
1. Entra al repositorio recién creado
2. Clic en **Add file → Upload files**
3. Arrastra los 5 archivos: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`
4. Clic en **Commit changes**

### Opción B — Desde terminal
```bash
git clone https://github.com/TU_USUARIO/ruta-rm-2026.git
cd ruta-rm-2026
# Copia los 5 archivos aquí
git add .
git commit -m "Initial PWA"
git push
```

---

## Paso 3 — Activar GitHub Pages

1. En tu repo, ve a **Settings → Pages**
2. En "Source" selecciona: **Deploy from a branch**
3. Branch: **main** / Folder: **/ (root)**
4. Clic en **Save**
5. Espera ~1 minuto

Tu app quedará en:
```
https://TU_USUARIO.github.io/ruta-rm-2026/
```

---

## Paso 4 — Instalar en tu celular

### En Android (Chrome)
1. Abre el link en Chrome
2. Aparece banner "Agregar a pantalla de inicio" → tócalo
3. O: menú ⋮ → "Instalar app"

### En iPhone (Safari)
1. Abre el link en Safari
2. Toca el botón compartir □↑
3. Selecciona "Agregar a pantalla de inicio"
4. Confirma

---

## ✅ Resultado

La app aparece en tu pantalla de inicio como cualquier app nativa.
Funciona sin internet (modo offline) gracias al service worker.
El progreso se guarda localmente en tu teléfono.

---

## 🔄 Actualizar la app en el futuro

Cada vez que modifiques y subas cambios a GitHub, la app se actualiza
automáticamente la próxima vez que la abras con internet.
