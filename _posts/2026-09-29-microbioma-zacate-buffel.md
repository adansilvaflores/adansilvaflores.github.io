---
layout: post
title: "El zacate buffel y sus aliados invisibles: el microbioma de una invasora del desierto de Sonora"
description: "Qué bacterias viven en las raíces del zacate buffel, cómo responden a sus propios compuestos químicos y por qué podría importar para controlar su invasión. Resumen de nuestro artículo en PLOS ONE."
lang: es
tags: [microbioma, desierto de Sonora, especies invasoras, 16S]
---

<!--
NOTAS PARA ADÁN (no se publican):
- Los bloques [HISTORIA] son espacios para tu storytelling personal: escena de apertura,
  tu papel en el estudio, qué te sorprendió y tu reflexión final.
- Las figuras vienen del artículo (licencia CC BY). Puedes cambiarlas por tus fotos:
  súbelas a images/ y usa ![texto](/images/archivo.jpg).
-->

<!-- [HISTORIA] Escena de apertura: tu primer recuerdo de un potrero de buffel en Sonora. -->

Si has manejado por Sonora, seguramente lo has visto: pastizales dorados y uniformes que se extienden hasta el horizonte, justo donde antes había matorral espinoso, cactus y mezquites. Parece un paisaje natural, pero no lo es. Es el **zacate buffel** (*Pennisetum ciliare*, también llamado *Cenchrus ciliaris*), una planta originaria del este de África que llegó a Norteamérica en los años 30 para alimentar al ganado.

Se eligió por buenas razones, desde el punto de vista ganadero: germina con facilidad, crece rápido, produce mucho forraje y rebrota después de un incendio gracias a su enorme sistema de raíces. En el noroeste de México se desmontaron grandes extensiones de matorral para sembrarlo. Esas mismas cualidades lo convirtieron en una de las **plantas invasoras más problemáticas de Norteamérica**.

## Un invasor con química propia

El buffel no solo le gana a las plantas nativas por agua, luz y nutrientes. También hace **guerra química**. A este fenómeno se le llama **alelopatía**: la planta libera compuestos, en el caso del buffel sobre todo **ácidos fenólicos** como el cumárico, el ferúlico o el vainíllico, que frenan la germinación y el crecimiento de otras especies.

El efecto se nota en el paisaje. En el desierto de Sonora, los potreros de buffel pueden tener entre **53 y 73 % menos especies de plantas nativas** que el matorral sin perturbar. Y controlarlo no es sencillo: herbicidas, remoción manual, quemas controladas y pastoreo dirigido no han sido suficientes.

## La pieza que faltaba: sus microbios

Toda planta vive rodeada de microorganismos. La **rizosfera**, la delgada capa de suelo pegada a las raíces, es uno de los ambientes más poblados del planeta: la planta alimenta ahí a bacterias con azúcares y otros compuestos que libera, y muchas de ellas le devuelven el favor con nutrientes, hormonas o protección.

En varias plantas invasoras se ha visto que **sus microbios son parte de su éxito**. Pero en el caso del buffel nadie había descrito qué bacterias viven en sus raíces, ni cómo les afectan los compuestos químicos que la propia planta produce. Esa fue nuestra pregunta:

> ¿Qué bacterias recluta el zacate buffel en su rizosfera, y cómo cambian cuando están expuestas a sus propios compuestos alelopáticos?

## El experimento

<!-- [HISTORIA] Tu papel en el estudio: ¿qué parte hiciste tú? -->

Colectamos **semillas y suelo** de un potrero de buffel en **Rancho Diamante, Sonora**, un sitio donde la vegetación original era matorral espinoso. En el laboratorio germinamos las semillas y, a los 70 días, trasplantamos las plantas a **tubos de PVC curvos** con suelo del mismo rancho. Luego las dividimos en tres grupos:

1. **Exudados de raíz**: en el otro extremo del tubo crecía una segunda planta de buffel, separada por una malla. Sus raíces no se tocaban, pero los compuestos que liberaba sí llegaban.
2. **Lixiviados**: en lugar de agua, las regamos con un extracto de hojas y tallos de buffel, simulando la lluvia que lava la planta y arrastra sus compuestos al suelo.
3. **Control**: solo agua.

![Diseño experimental del estudio: germinación, trasplante a tubos de PVC y tres tratamientos](https://journals.plos.org/plosone/article/figure/image?size=large&id=10.1371/journal.pone.0285978.g001)
*Diseño experimental. Figura 1 de Jara-Servin et al. (2023), PLOS ONE, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*

Tomamos muestras de la rizosfera a los **20 y 40 días**, extrajimos el ADN y secuenciamos un fragmento del gen **16S rRNA**, una especie de "código de barras" que permite identificar bacterias sin tener que cultivarlas. Procesamos las secuencias con **DADA2**, asignamos la taxonomía con la base de datos **SILVA** y analizamos la diversidad y la abundancia diferencial en **R** con phyloseq, vegan y DESeq2.

## Lo que encontramos

**1. Una comunidad diversa, dominada por especialistas en sequía.**
Identificamos **2,164 variantes de secuencia (ASVs)**, que son básicamente tipos distintos de bacterias, pertenecientes a **24 filos**. Dominaron las **Actinobacterias**, un grupo muy común en suelos áridos: sus esporas pueden germinar con muy poca agua, lo que les permite sobrevivir a la sequía.

**2. Un núcleo de 30 géneros que siempre acompaña al buffel.**
Treinta géneros bacterianos aparecieron en todas las plantas, sin importar el tratamiento ni el momento del muestreo. Es el **core microbiome** del buffel, su "equipo base". Entre ellos está *Nitrospira*, capaz de transformar amonio en nitrato, lo que podría ayudar a la planta a conseguir nitrógeno en un suelo desértico pobre. También aparecen géneros como *Bradyrhizobium*, *Sphingomonas* y *Micromonospora*, conocidos en otras plantas por promover el crecimiento o producir antimicrobianos.

![Mapa de calor del microbioma núcleo del zacate buffel a nivel de género](https://journals.plos.org/plosone/article/figure/image?size=large&id=10.1371/journal.pone.0285978.g005)
*Microbioma núcleo a nivel de género; los géneros marcados con estrella forman el core. Figura 5 de Jara-Servin et al. (2023), PLOS ONE, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*

**3. El tiempo pesó más que la química.**
Las comunidades bacterianas cambiaron de forma estadísticamente significativa **entre los 20 y los 40 días**: el microbioma se transforma conforme la planta se desarrolla. En cambio, los tratamientos con exudados y lixiviados, vistos en conjunto, no separaron las comunidades de forma significativa. Además, todas las muestras de raíz se distinguieron claramente del suelo sin planta: el buffel "filtra" y selecciona sus propias bacterias.

![Ordenación CAP y dendrograma UniFrac de las comunidades bacterianas](https://journals.plos.org/plosone/article/figure/image?size=large&id=10.1371/journal.pone.0285978.g003)
*Diversidad beta: las muestras se agrupan por tiempo de muestreo. Figura 3 de Jara-Servin et al. (2023), PLOS ONE, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*

**4. Aun así, la química favoreció a bacterias específicas.**
Aunque la comunidad completa no cambió de golpe, algunas bacterias sí aumentaron con los compuestos del buffel. Con los exudados de raíz se enriquecieron géneros como *Planctomicrobium*, *Aurantimonas*, *Tellurimicrobium*, *Saccharothrix* y *Oxalicibacterium*, y *Caulobacter* aumentó con ambos tratamientos. Varias de estas bacterias son capaces de **vivir entre compuestos fenólicos o incluso metabolizarlos**.

Hay un detalle curioso: el buffel puede acumular **oxalato**, un compuesto que en exceso es tóxico para el ganado. *Oxalicibacterium* y *Tellurimicrobium* pueden usar el oxalato o compuestos relacionados, así que la planta podría estar reclutando bacterias que procesan su propia química.

<!-- [HISTORIA] ¿Qué resultado te sorprendió más? -->

## ¿Por qué importa?

La idea que deja este trabajo es que **el buffel no invade solo**. Recluta bacterias capaces de prosperar en el ambiente químico que él mismo crea, y esa comunidad cambia conforme la planta crece. Entender quiénes son esos aliados invisibles y qué hacen abre una puerta nueva: **estrategias de control que actúen sobre el microbioma**, y no solo sobre la planta.

Este estudio usó 16S, que dice *quiénes* están ahí. El siguiente paso natural es la **metagenómica**, que permite ver *qué pueden hacer*: qué genes tienen para degradar fenoles, fijar nitrógeno o producir antibióticos.

<!-- [HISTORIA] Tu reflexión final: qué significa este trabajo para ti y cómo conecta con lo
     que haces ahora (microbiomas, manglares, bioinformática). -->

## Datos abiertos

Todo el estudio es público y reproducible:

- 📄 **Artículo** (acceso abierto): Jara-Servin A, **Silva A**, Barajas H, Cruz-Ortega R, Tinoco-Ojanguren C, Alcaraz LD (2023). *Root microbiome diversity and structure of the Sonoran desert buffelgrass (Pennisetum ciliare L.)*. PLOS ONE 18(5): e0285978. [doi:10.1371/journal.pone.0285978](https://doi.org/10.1371/journal.pone.0285978)
- 🧬 **Secuencias**: NCBI SRA, proyecto [PRJNA879420](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA879420)
- 💻 **Código del análisis**: [genomica-fciencias-unam/buffelgrass](https://github.com/genomica-fciencias-unam/buffelgrass)
- 📊 **Figuras y tablas**: [FigShare](https://doi.org/10.6084/m9.figshare.c.6605350.v2)

¿Hay buffel cerca de donde vives? Cuéntame en [Instagram](https://www.instagram.com/microbialito/).
