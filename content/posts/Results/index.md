---
date: "2024-12-02"
image: equation.jpg
math: true
tags:
title: Resultados
---

## Estados Unidos. Líder productor mundial de LNG.

![](./images/s4.jpg)
<span style="font-size: 10px;">Fuente: Elaboración propia con datos para los años 2004 a 2022 (SINAIS, 2022).</span> 


Although the proposed indicator is a relative measure of concentration and **controls for the population size** of the states compared to the national level, the age-specific structure in these geographic areas could introduce biases in the estimation of the Relative Concentration Index (ILI).

Therefore, the age distribution by hospital discharge for the case of Coahuila is explored below, based on the construction of **Kernel density curves** according to Chen (2017).



**Figure  3** Average age of hospital discharges by State 2022. (T-test with 95% confidence intervals).

![](./images/asma_test.jpg)
<span style="font-size: 10px;">Fuente: Elaboración propia con datos de (SINAIS, 2022)</span> 


**Figure 4**. Age distribution for hospital discharges. asthma patientes in Coahuila, CDMX, and Jalisco 2022.


![](./images/edad_asma_comparison.jpg)
<span style="font-size: 10px;">Fuente: Elaboración propia con datos de (SINAIS, 2022)</span

The distribution of hospital discharges by age indicates that the most affected population is **young**, as **75%** of hospital discharges for asthma at the national level are between the ages of **1 and 21**.


**Figure 5**. Age-structure-adjusted asthma morbidity rates
by Region.  Coahuila, 2022

![](./images/Regiones_v3.jpeg)
<span style="font-size: 10px;">Fuente:Fuente: Datos de (Consejo Nacional de Población, 2017; SINAIS, 2022).</span


* **Key findings:**  The influence area defined in this study, encompassing emissions from the coal-fired power plants of the Federal Electricity Commission, which includes both the **coal mining region** and the **border region**, shows an incidence rate of **15.2** cases per 100,000 inhabitants. This rate is higher than the **national average of 9.6** cases per 100,000 inhabitants. 


To further inquiry  into this pattern we documented emission concentrations of criteria pollutants by region for key air quality related elements.

**Table 1** Inventory of Criteria Pollutant Emissions (Mg/year). <cite>[^2]</cite>

[^2]:  <span style="font-size: 11px;">Air pollutants for which acceptable levels of exposure have been determined and air quality standards have been set.The abbreviation Mg stands for megagrams, which is equivalent to metric tons (1 Mg = 1,000 kilograms or approximately 2,204.62 pounds). In environmental contexts, such as the reporting of criteria pollutant emissions, quantities are often expressed in megagrams per year (Mg/year) to denote the mass of pollutants emitted annually.See Intergovernmental Panel on Climate Change (IPCC) for additional details.
The primary source of ammonia emissions comes from livestock waste and the application of nitrogen-based fertilizers).</span> 

![](./images/table.jpg)
 <span style="font-size: 10px;">**Source**: Coahuila state Environmental Health Ministry. [Criteria pollutant emissions inventory](https://sma.gob.mx/sga-inventario-de-emisiones-ano-base-2014/)</span> <cite>[^3]</cite>
 
[^3]: <span style="font-size: 11px;">Recent studies on dust and health have been conducted by  Herrera-Molina, E., Gill, T. E., Ibarra-Mejia, G., & Jeon, S. (2021). Associations between dust exposure and hospitalizations in El Paso, Texas, USA. Atmosphere, 12(11), 1413 </span>




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