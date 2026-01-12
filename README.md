# Visualización Electoral — Alcaldía Coyoacán (2021)

Proyecto de visualización y análisis territorial de resultados electorales a nivel **sección electoral** para la Alcaldía Coyoacán (CDMX) que principalmente, presenta dos insumos:

1) **Participación ciudadana (2021):** distribución espacial del porcentaje de participación del electorado por sección electoral.  
2) **Zonas competitivas (2021) con potencial electoral (2025):** identificación de secciones con contiendas cerradas (margen < 5%) y estimación del volumen de electores potenciales (Lista Nominal, nov-2025) para dimensionar “cuántos votos están en juego” en zonas competitivas.

> **Nota:** este repositorio presenta un ejercicio de análisis espacial y comunicación de datos públicos. No promueve partidos, candidaturas ni estrategias proselitistas.

---

## Mapas (salidas principales)

### 1) Participación electoral por sección — 2021
El mapa muestra qué tanto salió a votar la ciudadanía en cada sección electoral de Coyoacán. Los colores más claros representan zonas con menor participación, mientras que los tonos más oscuros indican secciones con mayor participación.

**Análisis territorial:**
- Secciones con baja participación pueden asociarse a dinámicas de **desconexión** o **baja activación comunitaria**, relevantes para análisis de inclusión, acceso a información y participación.  
- Secciones con participación alta reflejan comunidades con mayor involucramiento cívico, donde variaciones pequeñas pueden ser significativas para entender cambios locales.
![Participación Ciudadana](https://github.com/user-attachments/assets/df0d8803-49f3-4550-a30a-5e3074fe4c18)
![Competitividad electoral](https://github.com/user-attachments/assets/52790560-3eba-4b97-9fa3-2be95e128e91)


---

### 2) Zonas competitivas (2021) con potencial electoral (2025)
Este mapa identifica las secciones donde la contienda fue cerrada en 2021 (**margen < 5%**) y agrega etiquetas con el **tamaño actual del electorado** (Lista Nominal a nov-2025) en dichas secciones.


**¿Qué aporta?**
- Distingue **dónde** ocurrió la competencia cerrada y **cuánto** electorado está involucrado hoy en esas áreas.  
- Permite interpretar el territorio electoral combinando **geografía del voto (2021)** y **magnitud del electorado (2025)**.


---

## Visualización interactiva (Leaflet)
Este proyecto cuenta con una visualización interactiva (Leaflet) para explorar capas electorales y atributos por sección.
![MapaInteractivo](https://github.com/user-attachments/assets/2d672c4f-cbbb-4617-ac98-6a49aa95a147)




---

## Datos y fuentes
- **Resultados electorales y cartografía de secciones electorales:** datos públicos descargados de fuentes oficiales del **Marco Geográfico Electoral, 2021**.  
- **Lista Nominal (nov-2025):** insumo oficial para dimensionar el electorado actual.

> Por política de uso y para proteger el empaquetado del producto, este repositorio no incluye la base original completa. Se documenta el flujo y se muestran salidas (mapas/capturas) como evidencia del trabajo.

---

## Metodología
1) Descarga y preparación de resultados y secciones electorales.  
2) Estandarización de llaves (IDs de sección) y validación (faltantes/duplicados).  
3) Derivación de indicadores:
   - % participación por sección (2021).
   - margen de victoria (2021) y filtro de competitividad (< 5%).
   - unión con Lista Nominal (nov-2025) para etiquetado de secciones competitivas.
4) Representación cartográfica (rangos, simbología, elementos cartográficos).  
5) Visualización interactiva en Leaflet para exploración de atributos.

Detalles adicionales: ver `docs/notas_metodologicas.md`.

---

## Consideraciones éticas y privacidad
- Se usan datos agregados a nivel sección electoral, sin información personal identificable.
- El objetivo es analítico y de comunicación pública.

---

## Tecnologías / Herramientas
- SIG (cartografía temática y diseño de simbología)
- Visualización web (Leaflet)
- Procesamiento y limpieza de datos
- Creación de leaflet en RStudio

---

## Autora
**María Fernanda González Mora**  
