# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 13 correctas de 22 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.23 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.15 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.13 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.11 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.17 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura,id_curso_escolar, PRIMARY,nif

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.20 ms
✅ Se usó índice(s) en la consulta: id_profesor,id_grado, PRIMARY,id_departamento, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.15 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.26 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.20 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.16 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 13: Error
- **Descripción**: 1054 (42S22): Unknown column 'asignatura_id_profesor' in 'on clause'


## ✅ Query 14: Correcto

⏱ Tiempo: 0.17 ms
✅ Se usó índice(s) en la consulta: id_profesor

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,5 +1,4 @@
 nombre
-Informática
 Matemáticas
 Economía y Empresa
 Educación
```

⏱ Tiempo: 0.20 ms
✅ Se usó índice(s) en la consulta: id_profesor, id_departamento

---

## ❌ Query 16: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'AND profesor.id_profesor IS NOT NULL' at line 1


## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
 total
-2.00
+12.00
```

⏱ Tiempo: 0.16 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 18: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,2 @@
-departamento | total
-Educación | 3.00
-Informática | 2.00
-Matemáticas | 2.00
-Economía y Empresa | 2.00
-Química y Física | 2.00
-Agronomía | 1.00
+total
+2.00
```

⏱ Tiempo: 0.16 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,7 @@
 departamento | total
+Educación | 3.00
 Informática | 2.00
 Matemáticas | 2.00
 Economía y Empresa | 2.00
-Educación | 3.00
+Química y Física | 2.00
 Agronomía | 1.00
-Química y Física | 2.00
-Filología | 0.00
-Derecho | 0.00
-Biología y Geología | 0.00
```

⏱ Tiempo: 0.21 ms
✅ Se usó índice(s) en la consulta: id_departamento, PRIMARY

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,10 @@
-grau | total
-Grado en Ingeniería Informática (Plan 2015) | 51.00
-Grado en Biotecnología (Plan 2015) | 32.00
-Grado en Ingeniería Agrícola (Plan 2015) | 0.00
-Grado en Ingeniería Eléctrica (Plan 2014) | 0.00
-Grado en Ingeniería Electrónica Industrial (Plan 2010) | 0.00
-Grado en Ingeniería Mecánica (Plan 2010) | 0.00
-Grado en Ingeniería Química Industrial (Plan 2010) | 0.00
-Grado en Ciencias Ambientales (Plan 2009) | 0.00
-Grado en Matemáticas (Plan 2010) | 0.00
-Grado en Química (Plan 2009) | 0.00
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

⏱ Tiempo: 0.18 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 21: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,11 @@
 grau | total
 Grado en Ingeniería Informática (Plan 2015) | 51.00
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

⏱ Tiempo: 0.18 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 22: Error
- **Descripción**: 'NoneType' object is not iterable

