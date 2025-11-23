---
date: "2024-12-02"
image: equation.jpg
math: true
tags:
title: Resultados
---

## Estados Unidos. Líder productor mundial de LNG.


**Figura 1.** Producción gas natural. Principales países 1980-2024.

![](./images/s4.jpg)
<span style="font-size: 10px;">Fuente: Elaboración propia con datos de (Enerdata, 2025).</span> 


Estados Unidos se ha convertido en el **líder productor mundial** y es proveedor de importantes socios  comerciales en Asia. 

### Japón, Corea del sur, Taiwán capturan **un tercio** de las importaciones mundiales. Potentes demandantes por su magnitud son China e India. 

**Figura 2**.  Gas natural en Estados Unidos. Balance entre producción, consumo interno y exportaciones 1950-2023.


![](./images/s2.jpg )
<span style="font-size: 10px;">Fuente Elaboración propia con datos de (Energy Information Agency, 2025).</span> 

#### El **superávit** generado ha creado el incentivo económico de la **industria energética** estadounidense por desarrollar infraestructura con el propósito de transportar los excedentes desde los sitios de producción hasta los mercados destino, incluida la demanda de consumidores en Asía, lo que **implica contar con rutas eficientes en el océano Pacífico**.

La **desequilibrio geográfica** entre las zonas de **disponibilidad-extracción-exportación** y aquellas que impulsan los procesos de **demanda-importación-consumo**, ha resultado en el desarrollo de estrategias de abastecimiento que se materializan en <span style="color:  red;">proyectos de infraestructura trans regionales.</span> 



---

<!-- Return to Home Page -->
<div style="text-align: center; margin: 2rem 0;">
  <a href="/" style="background-color: #2E86AB; color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer; font-size: 14px; text-decoration: none; display: inline-block;">
    ← Return to Home
  </a>
</div>

<style>
.expandable-image {
    cursor: zoom-in;
    transition: transform 0.3s ease;
    border: 2px solid transparent;
}
.expandable-image:hover {
    transform: scale(1.02);
    border-color: #2E86AB;
}
.image-modal {
    display: none;
    position: fixed;
    z-index: 10000;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.95);
    animation: fadeIn 0.3s;
}
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}
.modal-content {
    margin: auto;
    display: block;
    width: auto;
    max-width: 95%;
    max-height: 90vh;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    animation: zoomIn 0.3s;
}
@keyframes zoomIn {
    from { transform: translate(-50%, -50%) scale(0.8); }
    to { transform: translate(-50%, -50%) scale(1); }
}
.close-modal {
    position: absolute;
    top: 20px;
    right: 35px;
    color: #fff;
    font-size: 40px;
    font-weight: bold;
    cursor: pointer;
    z-index: 10001;
    background: rgba(0,0,0,0.5);
    border-radius: 50%;
    width: 50px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.close-modal:hover {
    color: #ccc;
    background: rgba(0,0,0,0.7);
}
.image-caption {
    color: #fff;
    text-align: center;
    padding: 15px;
    font-size: 14px;
    position: absolute;
    bottom: 0;
    width: 100%;
    background: rgba(0,0,0,0.7);
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
    // Crear el modal
    const modal = document.createElement('div');
    modal.className = 'image-modal';
    modal.innerHTML = `
        <span class="close-modal">&times;</span>
        <img class="modal-content" id="expanded-image">
        <div class="image-caption" id="modal-caption"></div>
    `;
    document.body.appendChild(modal);

    // Hacer las imágenes expandibles
    const images = document.querySelectorAll('img');
    images.forEach(img => {
        // No aplicar a botones o logos pequeños
        if (img.width > 100 && img.height > 100 && !img.closest('a')) {
            img.classList.add('expandable-image');
            
            img.addEventListener('click', function() {
                const modal = document.querySelector('.image-modal');
                const modalImg = document.getElementById('expanded-image');
                const caption = document.getElementById('modal-caption');
                
                modal.style.display = 'block';
                modalImg.src = this.src;
                modalImg.alt = this.alt;
                
                // Buscar el texto de fuente
                let sourceText = this.alt || '';
                let nextElement = this.nextElementSibling;
                
                // Buscar en los siguientes 2 elementos
                for (let i = 0; i < 2; i++) {
                    if (nextElement && nextElement.tagName === 'SPAN') {
                        if (nextElement.textContent.includes('Fuente:') || 
                            nextElement.textContent.includes('Source:')) {
                            sourceText = nextElement.textContent;
                            break;
                        }
                    }
                    if (nextElement) {
                        nextElement = nextElement.nextElementSibling;
                    }
                }
                
                caption.textContent = sourceText;
            });
        }
    });

    // Cerrar modal
    const closeBtn = document.querySelector('.close-modal');
    const modalElement = document.querySelector('.image-modal');
    
    closeBtn.addEventListener('click', function() {
        modalElement.style.display = 'none';
    });
    
    modalElement.addEventListener('click', function(e) {
        if (e.target === modalElement) {
            modalElement.style.display = 'none';
        }
    });
    
    // Cerrar con tecla ESC
    document.addEventListener('keydown', function(e) {
        if (e.key === 'Escape') {
            modalElement.style.display = 'none';
        }
    });
});
</script>