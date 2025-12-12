# Configurar GitHub Pages para worldwide-app-qr

## Paso a paso para habilitar GitHub Pages

### 1. Ir a la configuración del repositorio
1. Ve a: https://github.com/wwdiegovarela/worldwide-app-qr
2. Haz clic en **Settings** (Configuración)
3. En el menú lateral izquierdo, busca y haz clic en **Pages**

### 2. Configurar GitHub Pages
1. En la sección **Source** (Fuente):
   - Selecciona **Deploy from a branch** (Desplegar desde una rama)
   - Branch (Rama): selecciona **main**
   - Folder (Carpeta): selecciona **/ (root)** (raíz)
2. Haz clic en **Save** (Guardar)

### 3. Esperar el despliegue
- GitHub Pages puede tardar unos minutos en desplegarse
- Aparecerá un mensaje verde indicando que el sitio está publicado
- La URL será: `https://wwdiegovarela.github.io/worldwide-app-qr/`

### 4. Verificar que funciona
- Visita la URL después de unos minutos
- Si sigue dando 404, espera 5-10 minutos más (puede tardar en propagarse)

## Verificación adicional

### Opción A: Verificar en el repositorio
1. Ve a **Settings** → **Pages**
2. Debe aparecer un mensaje: "Your site is live at https://wwdiegovarela.github.io/worldwide-app-qr/"

### Opción B: Usar una rama gh-pages (alternativa)
Si prefieres usar una rama dedicada, puedes:
1. Crear una rama `gh-pages`
2. Configurar GitHub Pages para usar esa rama

## Solución de problemas

### Si sigue dando 404 después de configurar:
1. **Verifica que el archivo `index.html` esté en la raíz del repositorio** ✅ (ya está)
2. **Verifica que la rama `main` tenga commits** ✅ (tiene commits)
3. **Espera 5-10 minutos** - GitHub Pages puede tardar en desplegarse
4. **Verifica en Settings → Pages** que aparezca la URL del sitio

### Si el sitio no se actualiza:
- Haz un commit nuevo (aunque sea vacío) para forzar un nuevo despliegue:
  ```bash
  git commit --allow-empty -m "Trigger GitHub Pages rebuild"
  git push
  ```

## URL del sitio

Una vez configurado, el sitio estará disponible en:
**https://wwdiegovarela.github.io/worldwide-app-qr/**

