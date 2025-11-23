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
> **<mark> La transición energética global**, entendida como el proceso en el que las sociedades a escala mundial llevan a cabo estrategias para reducir el uso de combustibles de alto impacto ambiental (Naciones Unidas, 2023.).

### Contraste de emisiones Carbón vs. Gas Natural. 


![](./images/s8.jpg)

### México:  Un país dependiente de la energía proveniente de Estados Unidos.


**Figura 3**. Exportaciones mensuales de gas natural por gasoducto desde EE. UU. a Canadá y México (1973-2023)

![](./xports.jpeg)

<span style="font-size: 10px;">Fuente Elaboración propia con datos de (Energy Information Agency, 2025).</span> 


**Figura 4.** Precio de exportación Gas Natural Licuado (US dólar por miles de pies cúbicos) y precio de petróleo crudo, mezcla West Texas Intermediate (wti) 2001-2024



![](./p.jpg)

### <span style="color:  #F18F01;">Indicadores Críticos</span>

+	<span style="color:  red;">Declive del 42.6% en producción doméstica 2012-2022</span>

+	Incremento del 24.1% en consumo 2012-2022

+	Dependencia de importaciones de EE.UU. superará 50% para 2030

+ 	48% de generación eléctrica usa gas natural

+	Solo 46.8% de gasoductos son propiedad del Estado

###  <span style="color:  #F18F01;">Expansión de Infraestructura 2018-2024</span> 

+	3,050 km de nuevos gasoductos

+	48.9% en región noroeste

+	<span style="color:  red;"> Proyectos emblemáticos en Sonora</span>

###  Gracias por su atencion.  

![](./images/qr-code.png)


## <span style="color:  #e77162;">Coloquio Anual de Políticas Públicas</span>
#####  Universidad Autónoma Metropolitana  Casa Abierta al tiempo
Noviembre 24, 2025.

jlmanzanaresrivera@colef.mx


<style>
/* Black background for this specific post */
main, .content, article, .post {
    background-color: #000000 !important;
    color: #ffffff !important;
    padding: 2rem !important;
    min-height: 100vh !important;
}

/* Add all the other styles from above */
</style>
  


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