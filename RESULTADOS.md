# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 8 correctas de 18 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.44 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.34 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.38 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.52 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_asignatura,id_curso_escolar, PRIMARY,nif, PRIMARY

---

## ❌ Query 8: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1 @@
 nombre
-Informática
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, id_profesor,id_grado, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ❌ Query 10: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
-departamento | apellido1 | apellido2 | nombre
-Agronomía | Monahan | Murray | Micaela
-Economía y Empresa | Fahey | Considine | Antonio
-Economía y Empresa | Lemke | Rutherford | Cristina
-Educación | Ruecker | Upton | Guillermo
-Educación | Spencer | Lakin | Esther
-Educación | Streich | Hirthe | Carmen
-Informática | Hamill | Kozey | Manolo
-Informática | Ramirez | Gea | Zoe
-Matemáticas | Kohler | Schoen | Alejandro
-Matemáticas | Schmidt | Fisher | David
-Química y Física | Schowalter | Muller | Francesca
-Química y Física | Stiedemann | Morissette | Alfredo
+nombre | apellido1 | apellido2 | departamento
+Micaela | Monahan | Murray | Agronomía
+Antonio | Fahey | Considine | Economía y Empresa
+Cristina | Lemke | Rutherford | Economía y Empresa
+Guillermo | Ruecker | Upton | Educación
+Esther | Spencer | Lakin | Educación
+Carmen | Streich | Hirthe | Educación
+Manolo | Hamill | Kozey | Informática
+Zoe | Ramirez | Gea | Informática
+Alejandro | Kohler | Schoen | Matemáticas
+David | Schmidt | Fisher | Matemáticas
+Francesca | Schowalter | Muller | Química y Física
+Alfredo | Stiedemann | Morissette | Química y Física
```

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 11: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SELECT departamento.nombre
FROM departamento
LEFT JOIN profesor
    ON profesor.' at line 16


## ❌ Query 12: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,63 @@
-nombre
-Filología
-Derecho
-Biología y Geología
+id | nombre
+22.00 | Ingeniería de Requisitos
+23.00 | Integración de las Tecnologías de la Información en las Organizaciones
+24.00 | Modelado y Diseño del Software 1
+25.00 | Multiprocesadores
+26.00 | Seguridad y cumplimiento normativo
+27.00 | Sistema de Información para las Organizaciones
+28.00 | Tecnologías web
+29.00 | Teoría de códigos y criptografía
+30.00 | Administración de bases de datos
+31.00 | Herramientas y Métodos de Ingeniería del Software
+32.00 | Informática industrial y robótica
+33.00 | Ingeniería de Sistemas de Información
+34.00 | Modelado y Diseño del Software 2
+35.00 | Negocio Electrónico
+36.00 | Periféricos e interfaces
+37.00 | Sistemas de tiempo real
+38.00 | Tecnologías de acceso a red
+39.00 | Tratamiento digital de imágenes
+40.00 | Administración de redes y sistemas operativos
+41.00 | Almacenes de Datos
+42.00 | Fiabilidad y Gestión de Riesgos
+43.00 | Líneas de Productos Software
+44.00 | Procesos de Ingeniería del Software 1
+45.00 | Tecnologías multimedia
+46.00 | Análisis y planificación de las TI
+47.00 | Desarrollo Rápido de Aplicaciones
+48.00 | Gestión de la Calidad y de la Innovación Tecnológica
+49.00 | Inteligencia del Negocio
+50.00 | Procesos de Ingeniería del Software 2
+51.00 | Seguridad Informática
+52.00 | Biologia celular
+53.00 | Física
+54.00 | Matemáticas I
+55.00 | Química general
+56.00 | Química orgánica
+57.00 | Biología vegetal y animal
+58.00 | Bioquímica
+59.00 | Genética
+60.00 | Matemáticas II
+61.00 | Microbiología
+62.00 | Botánica agrícola
+63.00 | Fisiología vegetal
+64.00 | Genética molecular
+65.00 | Ingeniería bioquímica
+66.00 | Termodinámica y cinética química aplicada
+67.00 | Biorreactores
+68.00 | Biotecnología microbiana
+69.00 | Ingeniería genética
+70.00 | Inmunología
+71.00 | Virología
+72.00 | Bases moleculares del desarrollo vegetal
+73.00 | Fisiología animal
+74.00 | Metabolismo y biosíntesis de biomoléculas
+75.00 | Operaciones de separación
+76.00 | Patología molecular de plantas
+77.00 | Técnicas instrumentales básicas
+78.00 | Bioinformática
+79.00 | Biotecnología de los productos hortofrutículas
+80.00 | Biotecnología vegetal
+81.00 | Genómica y proteómica
+82.00 | Procesos biotecnológicos
+83.00 | Técnicas instrumentales avanzadas
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: id_profesor

---

## ❌ Query 13: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'SELECT COUNT(*) AS total
FROM persona
WHERE tipo = 'alumno'' at line 8


## ❌ Query 14: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near ',
    AND YEAR(fecha_nacimiento) = 1999' at line 5


## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,7 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
+total | nombre
+3.00 | Educación
+2.00 | Informática
+2.00 | Matemáticas
+2.00 | Economía y Empresa
+2.00 | Química y Física
+1.00 | Agronomía
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_departamento

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,10 @@
-total
-12.00
+departamento | total
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Educación | 3.00
+Agronomía | 1.00
+Química y Física | 2.00
+Filología | 0.00
+Derecho | 0.00
+Biología y Geología | 0.00
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,11 @@
-total
-2.00
+grau | total
+Grado en Ingeniería Informática (Plan 2015) | 51.00
+Grado en Biotecnología (Plan 2015) | 32.00
+Grado en Ingeniería Agrícola (Plan 2015) | 0.00
+Grado en Ingeniería Eléctrica (Plan 2014) | 0.00
+Grado en Ingeniería Electrónica Industrial (Plan 2010) | 0.00
+Grado en Ingeniería Mecánica (Plan 2010) | 0.00
+Grado en Ingeniería Química Industrial (Plan 2010) | 0.00
+Grado en Ciencias Ambientales (Plan 2009) | 0.00
+Grado en Matemáticas (Plan 2010) | 0.00
+Grado en Química (Plan 2009) | 0.00
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 18: Error
- **Descripción**: 'NoneType' object is not iterable

