---
date: "2025-11-13"
description: Final statements
image: final.jpg
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




We documented:  

1. **Asthma** incidence at a **regional scale** focusing on the **border region**. 

2. The relationship between a **chronic-high cost disease**<span class="nowrap"><span class="emojify">🤧</span> and enviromental-human <span class="nowrap"><span class="emojify">🙈</span>caused exposition factors 🏭


## Analysis strengths:  


 * We use international comparable  indicators allowing **binational monitoring**.  
 
 * We employ data with a **local perspective** based on **electronic health records.**

* **Temporal** perspective allowing to define a **trend in time**📈. We actually find **asthma** to be a growing health concern for the region.

Which indicates a persistent issue demanding the attention of public health authorities.  Evidence indicates a cases concentration peak in **2016** relative to the national scenario (**LII=1.88**).   

* Higher than the national morbidity rates for the border and coal mining regions:   **15 vs. 9.2  per  100 000 pop**. 

* In additon **evidence** found suggest the existence of a **hot spot** 📍 of **asthma** in the **desert region** ️🏜️  as well as the **Laguna region**  The former assosated to desert dust (the highest concentration of **PM<sub>2.5</sub>** ) and the latter associated to the highest emissions of **Ammonia**.  **NH<sub>3</sub>** A quimical element found as a result of the economic activity of the region which includes **agro food and dairy industries 🐄**. (where NH<sub>3</sub> is a precursor of PM<sub>2.5</sub> 

## Final thoughts. 

Electricity generation using coal may be replaced with cleaner technologies. This energy transition is important to improve environmental quality and human health in this binational region at the Coahuila Texas border.   

Lessons learned from the **regional patterns** observed suggest that **economic activity**  and its environmental impacts provide valueble inputs for designing  **public health monitoring strategies.** 


## To do list for the research agenda.


* Incorporate a qualitative perspective to explore the life quality impacts for families and the challenges faced by children in particular border communities. 

***
###  Coloquio anual de políticas públicas 

#  Gracias por su atencion.  Noviembre 24, 2025.
jlmanzanaresrivera@colef.mx

![](./images/qr-code.png)



<!-- Return to Home Page -->
<div style="text-align: center; margin: 2rem 0;">
  <a href="/" style="background-color: #2E86AB; color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer; font-size: 14px; text-decoration: none; display: inline-block;">
    ← Return to Home
  </a>
</div>


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