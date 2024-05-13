---
title: "ParametrosCompartidos"
description: ""
summary: ""
date: 2024-05-13T12:20:25+02:00
lastmod: 2024-05-13T12:20:25+02:00
draft: false
weight: 50
categories: []
tags: []
contributors: []
pinned: false
homepage: false
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

# Parámetros compartidos

Etiquetas: Lecciones aprendidas

En un determinado momento se pensó que era una buena idea tener un fichero de parámetros compartidos por cliente. La lección aprendida, es que esto puede generar un gran problema.

En la imagen inferior se pueden ver los archivos de **ADIF_Parámetros compartidos_v1.0** y **IN_Parámetros compartidos_v1.1** en ambos ficheros tenemos el parámetro **_IN_Altura_** y cada uno tiene un GUID diferente 😵💥.

<aside>
💡 El **GUID** es la matrícula que Revit lee para poder localizar la información que se almacena en el parámetro. Esta cuestión ha creado problemas 🤬🤬 con familias y en modelos que han partido de la plantilla de ADIF y de INECO.

</aside>

La solución pasa por tener un único fichero unificado. **Las acciones y consecuencias de esta acción** son las siguientes:

1. Unificar el archivo txt, de parámetros compartidos.
   1. Actualizar plantillas (rte) de arquitectura.
   2. Actualizar plantillas (rte) de estructuras.
   3. Actualizar plantillas (rte) de instalaciones.
   4. Actualizar familias clave como: cajetines de planos y otras familias que se hayan visto afectadas por esta cuestión.

![Untitled](https://bimineco.notion.site/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F342db759-9472-4a34-9e3b-149781af4799%2F85d960c1-af17-4e59-9cfc-4f9f9c01b31c%2FUntitled.png?table=block&id=a1cee7c0-3861-40cc-910d-75a3113f4ba5&spaceId=342db759-9472-4a34-9e3b-149781af4799&width=2000&userId=&cache=v2)

<aside>
🚨 Si quieres saber más sobre los criterios de nombrado de los parámetros:

[IN_Parámetros compartidos generales](https://www.notion.so/IN_Par-metros-compartidos-generales-9ec58eb1b1a34615bcbfe75e50e6c50b?pvs=21)

</aside>

<aside>
🚨 Si quieres saber más sobre el estado de avance de las tareas de actualización de parámetros compartidos:

[Unificar parámetros compartidos](https://www.notion.so/Unificar-par-metros-compartidos-56e1f30fd35943e4b8bf6fad19827ce4?pvs=21)

</aside>
