# GymLog — Setup en GitHub Pages

## Archivos
```
gymlog/
├── index.html     ← app completa
├── manifest.json  ← PWA config
└── icon.svg       ← ícono
```

## Pasos (10 minutos)

### 1. Crear repo en GitHub
- Entrás a github.com → New repository
- Nombre: `gymlog`
- Público (GitHub Pages gratis requiere repo público)
- Crear

### 2. Subir los archivos
Opción A — desde el navegador (más fácil):
- En el repo → Add file → Upload files
- Subís los 3 archivos juntos
- Commit changes

Opción B — si tenés Git instalado:
```bash
git clone https://github.com/TU_USUARIO/gymlog
cd gymlog
# copiás los 3 archivos acá
git add .
git commit -m "GymLog PWA"
git push
```

### 3. Activar GitHub Pages
- En el repo → Settings → Pages
- Source: Deploy from a branch
- Branch: main / (root)
- Save

### 4. URL de tu app
Después de ~2 minutos:
`https://TU_USUARIO.github.io/gymlog`

---

## Instalar en el teléfono (Android)

1. Abrís la URL en Chrome
2. Chrome muestra "Agregar a pantalla de inicio" (banner automático)
   — O menú ⋮ → "Instalar app" / "Añadir a pantalla de inicio"
3. Queda como app nativa, sin barra del browser

## Instalar en iPhone

1. Abrís la URL en Safari (no Chrome)
2. Compartir (ícono cuadrado con flecha) → "Agregar a pantalla de inicio"
3. Queda como app nativa

---

## Migración de teléfono

1. En la app → Evolución → Backup JSON → "Copiar JSON de backup"
2. Te mandás el JSON a Gmail o Drive
3. En el teléfono nuevo: abrís la app → Evolución → Backup JSON → pegás el JSON → Restaurar backup

## Actualizar la app (cuando cambies rutina o quieras nueva versión)

Solo reemplazás `index.html` en el repo y GitHub Pages actualiza automáticamente.
