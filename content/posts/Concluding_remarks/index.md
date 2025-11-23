---
date: "2025-11-13"
description: Final statements
image: micare.jpg
math: true
enableEmoji: true
tags:
title: La narrativa de la transición energética
---


###### El impulso para la comercialización global del gas natural se ha hecho bajo el amparo de la narrativa de la transición energética.

### Definición:
> **La transición energética global**, entendida como el proceso en el que las sociedades a escala mundial llevan a cabo estrategias para reducir<mark>  el uso de combustibles de alto impacto ambiental (Naciones Unidas, 2023.).

### Contraste de emisiones Carbón vs. Gas Natural. 


![](./images/s8.jpg)


## México:  Un país dependiente de la energía proveniente de Estados Unidos.
Indicadores Críticos

+	<span style="color:  red;">Declive del 42.6% en producción doméstica 2012-2022<span style="color:  red;">

+	Incremento del 24.1% en consumo 2012-2022

+	Dependencia de importaciones de EE.UU. superará 50% para 2030

+ 	48% de generación eléctrica usa gas natural

+	Solo 46.8% de gasoductos son propiedad del Estado

####  Expansión de Infraestructura 2018-2024

+	3,050 km de nuevos gasoductos

+	48.9% en región noroeste

+	Proyectos emblemáticos en Sonora


***
###  Coloquio anual de políticas públicas 

#  Gracias por su atencion.  Noviembre 24, 2025.
jlmanzanaresrivera@colef.mx

![](./images/qr-code.png)

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

<!-- Return to Home Page -->
<div style="text-align: center; margin: 2rem 0;">
  <a href="/" style="background-color: #2E86AB; color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer; font-size: 14px; text-decoration: none; display: inline-block;">
    ← Return to Home
  </a>
</div>
