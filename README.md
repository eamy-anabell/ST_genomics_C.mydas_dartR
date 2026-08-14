# Análisis genómico de *Chelonia mydas*
El objetivo es investigar la estructura y adaptación genómica de la tortuga verde (*Chelonia mydas*) en la región del
Pacífico Oriental, utilizando SNPs obtenidos mediante la técnica DArTseq. Este estudio busca replicar lo realizado por Álvarez-Varas
et al. (2021) utilizando un genoma de referencia de alta calidad (a nivel cromosómico). 

Las zonas de alimentación consideradas en el EPO comprenden siete ubicaciones clave que incluyen las costas de México,
Costa Rica, Galápagos (Ecuador), Perú, Chile (Arica, Bahía Salada y Rapa Nui), Fiyi y Nueva Zelanda. Estas áreas son cruciales para comprender la variabilidad genética de *Chelonia mydas* en la región, que es conocida por su alta fidelidad y complejos patrones de migración.

# Metodología
Para este estudio se muestrearon un total de nueve áreas de alimentación de *Chelonia mydas*, dos en el Pacífico occidental (Nueva Zelanda y  Fuji) y siete en el Pacífico Oriental (México, Costa Rica, Galápagos-Ecuador, Perú y Chile). Cinco albergan el morfotipo negro y amarillos, basados en forma: Nueva Zelanda, Costa Rica, Galápagos-ecuador, Perú y Chile (Arica, Bahía Salado y Rapa Nui). Se recolectaron muestras de piel y sangre sonservadas en etanol al 90% o soluciones salinas saturadas. Las muestras fueron secuenciadas y genotipadas utilizando la tecnología de genotipado DArTseq Tm en Diversity Arrays Technology, Australia.

Los archivos se filtraron posteriormente para producir puntuaciones DArT e informes de SNP utilizando la plataforma bioinformática DArTtoolbox. Según la secuencia de aparición los loci se identificación como SNP o alelos de referencia según la frecuencia de aparición. Se realizó un filtrado adicional utilizando el paquete DartR implementado en el software RStudio. El filtrado utilizó los siguientes criterios: reproducibilidad (umbral = 1,00), frecuencias alélicas menores (MAF) >0,01, tasa de llamada individual con umbral >0,90, tasa de llamada de locus con umbral >0,85, y descarte de marcadores monomórficos. Los fragmentos que contenían más de un SNP fueron filtrados utilizando el comando gl.filter.secondaries.

Dado que las áreas de alimentación de *C. mydas* albergan individuos con múltiples orígenes se utilizó un enfoque basado en individuos (sin información previa) con todos los individuos y loci, para detectar como se agrupaban las muestras (PCoA, DAPC y STRUCTURE). Se definen los grupos genéticos. De los cuales trabajará con uno, realizando fitros de calidad y PCoA preliminar para ver si este agrupamiento.


# Datos
Los archivos de datos originales (`Report_DStu19-4381_SNP_mapping_1.csv`, `iddata_fgg.txt` y otros relacionados) 
**no se encuentran en este repositorio** debido a su tamaño. Sin embargo, los datos están disponibles bajo solicitud.
