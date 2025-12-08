# 📝 Guía de Actualización del Portafolio

## 🚀 Cómo Actualizar Tu Información

### 1. Información Personal (Sección "Sobre Mí")

Ubicación: `index.html` - Sección `#about`

```html
<h1 class="mb-0">
    Luciana
    <span class="text-primary">Sarate</span>
</h1>
```

**Qué actualizar:**
- Nombre y apellido
- Email y teléfono
- Ubicación
- Descripción profesional
- Enlaces a redes sociales

---

### 2. Experiencia Laboral

Ubicación: `index.html` - Sección `#experience`

**Formato para agregar nueva experiencia:**

```html
<div class="d-flex flex-column flex-md-row justify-content-between mb-5">
    <div class="flex-grow-1">
        <h3 class="mb-0">Título del Puesto</h3>
        <div class="subheading mb-3">Nombre del Proyecto o Empresa</div>
        <p>Descripción del proyecto y tus responsabilidades...</p>
        
        <div class="achievement-list">
            <p class="mb-2"><strong>Características principales:</strong></p>
            <ul>
                <li>Logro o característica 1</li>
                <li>Logro o característica 2</li>
            </ul>
        </div>
        
        <div class="tech-stack mb-3">
            <span class="badge bg-primary me-2">Tecnología 1</span>
            <span class="badge bg-primary me-2">Tecnología 2</span>
        </div>
    </div>
    <div class="flex-shrink-0">
        <span class="text-primary">Fecha Inicio - Fecha Fin</span>
    </div>
</div>
```

---

### 3. Formación Académica

Ubicación: `index.html` - Sección `#education`

**Para agregar nueva formación:**

```html
<div class="d-flex flex-column flex-md-row justify-content-between mb-5">
    <div class="flex-grow-1">
        <h3 class="mb-0">Título o Certificación</h3>
        <div class="subheading mb-3">Institución Educativa</div>
        <p>Descripción breve de lo aprendido...</p>
    </div>
    <div class="flex-shrink-0">
        <span class="text-primary">Fecha Inicio - Fecha Fin</span>
    </div>
</div>
```

---

### 4. Habilidades Técnicas

Ubicación: `index.html` - Sección `#skills`

**Iconos de tecnologías (dev-icons):**

```html
<li class="list-inline-item" title="Nombre Tecnología">
    <i class="fab fa-nombre-icono"></i>
</li>
```

**Buscar iconos en:** [Font Awesome](https://fontawesome.com/icons)

**Agregar nueva tecnología al stack:**

```html
<span class="badge bg-primary me-2">Nueva Tecnología</span>
```

---

### 5. Cambiar Colores del Sitio

Ubicación: `css/styles.css` - Variables CSS

```css
:root {
  --primary-color: #2c3e50;     /* Color principal (navbar, títulos) */
  --secondary-color: #3498db;   /* Color de acento (enlaces, badges) */
  --accent-color: #e74c3c;      /* Color de énfasis */
  --text-primary: #2c3e50;      /* Color de texto principal */
  --text-secondary: #7f8c8d;    /* Color de texto secundario */
}
```

**Paletas de colores sugeridas:**

#### Opción 1: Azul Profesional (Actual)
```css
--primary-color: #2c3e50;
--secondary-color: #3498db;
--accent-color: #e74c3c;
```

#### Opción 2: Verde Tecnológico
```css
--primary-color: #1e3a3a;
--secondary-color: #10b981;
--accent-color: #f59e0b;
```

#### Opción 3: Morado Creativo
```css
--primary-color: #4a1d6d;
--secondary-color: #8b5cf6;
--accent-color: #ec4899;
```

---

### 6. Actualizar Foto de Perfil

1. Coloca tu nueva imagen en la carpeta `img/`
2. Actualiza la referencia en `index.html`:

```html
<img class="img-profile rounded-circle mx-auto mb-2" 
     src="img/TU_NUEVA_IMAGEN.jpg" 
     alt="Luciana Sarate">
```

**Recomendaciones:**
- Formato: JPG o PNG
- Tamaño recomendado: 500x500px
- Peso máximo: 200KB

---

### 7. Agregar Nuevas Redes Sociales

Ubicación: `index.html` - Sección de iconos sociales

```html
<a class="social-icon" href="URL_DE_TU_RED_SOCIAL" target="_blank" aria-label="Nombre Red">
    <i class="fab fa-icono-red-social"></i>
</a>
```

**Iconos disponibles:**
- LinkedIn: `fa-linkedin-in`
- GitHub: `fa-github`
- Twitter/X: `fa-twitter` o `fa-x-twitter`
- Instagram: `fa-instagram`
- YouTube: `fa-youtube`
- TikTok: `fa-tiktok`

---

## 📤 Cómo Publicar los Cambios

### Método 1: GitHub Desktop
1. Abre GitHub Desktop
2. Revisa los cambios en "Changes"
3. Escribe un mensaje descriptivo
4. Click en "Commit to main"
5. Click en "Push origin"

### Método 2: Línea de Comandos
```bash
git add .
git commit -m "Actualización de portafolio: [descripción breve]"
git push origin main
```

### Método 3: GitHub Web
1. Ve a tu repositorio en GitHub
2. Click en "Upload files"
3. Arrastra los archivos modificados
4. Escribe un mensaje de commit
5. Click en "Commit changes"

---

## ✅ Checklist de Actualización

- [ ] Información de contacto actualizada
- [ ] Enlaces de redes sociales funcionando
- [ ] Nueva experiencia laboral agregada
- [ ] Habilidades técnicas actualizadas
- [ ] Foto de perfil actualizada (si aplica)
- [ ] Enlaces externos probados
- [ ] Revisión ortográfica completa
- [ ] Prueba en móvil y desktop
- [ ] Cambios publicados en GitHub

---

## 🐛 Solución de Problemas Comunes

### El sitio no se actualiza
- Espera 2-5 minutos después del push
- Limpia la caché del navegador (Ctrl + F5)
- Verifica que los cambios estén en la rama `main`

### Los estilos no se aplican
- Verifica que `styles.css` esté en la carpeta `css/`
- Revisa que no haya errores de sintaxis en el CSS
- Limpia la caché del navegador

### Las imágenes no se muestran
- Verifica que las rutas sean correctas (`img/nombre.jpg`)
- Asegúrate de que las imágenes estén en la carpeta `img/`
- Confirma que subiste las imágenes al repositorio

---

## 📞 Contacto

Si tienes dudas sobre cómo actualizar algo específico, puedes:
- Revisar la documentación de Bootstrap: https://getbootstrap.com
- Consultar Font Awesome para iconos: https://fontawesome.com
- Ver ejemplos en el código existente

---

**¡Éxito con tu portafolio! 🚀**
