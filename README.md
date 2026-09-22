Taller Integrador — Auditoría y corrección de un sitio web

Nombre completo: Marcos David Montenegro Perez
Curso: Buenas Prácticas de Desarrollo de Software - 24512 — CUC

**Descripción**
Este repositorio contiene la auditoría, corrección y despliegue de una página web que calcula el promedio de tres notas. La página original funcionaba correctamente, pero no seguía las buenas prácticas de nomenclatura, limpieza de código y estructura vistas en el curso. Este repositorio documenta el proceso de corrección usando un flujo de ramas y commits convencionales.

**Auditoría de hallazgos**

* **Archivos Mi Pagina De Notas.HTML / Estilos Del Sitio.CSS**
* **Por qué era un problema:** Espacios y mayúsculas inconsistentes en el nombre.
* **Cómo lo corregí:** Renombrados a `index.html` y `styles.css`.


* **Variables a, b, c**
* **Por qué era un problema:** No indican qué almacenan.
* **Cómo lo corregí:** Renombradas a `nota1`, `nota2`, `nota3`.


* **Variable x**
* **Por qué era un problema:** Número mágico sin nombre que explique su uso.
* **Cómo lo corregí:** Reemplazada por la constante `CANTIDAD_NOTAS`.


* **Variable TempValue2**
* **Por qué era un problema:** Nombre sin sentido y sin convención clara.
* **Cómo lo corregí:** Renombrada a `promedio`.


* **Variable data1**
* **Por qué era un problema:** Declarada y nunca usada.
* **Cómo lo corregí:** Eliminada.


* **Función calc()**
* **Por qué era un problema:** No describe qué hace la función.
* **Cómo lo corregí:** Renombrada a `calcularPromedio()`.


* **IDs n1, n2, n3, r, r2**
* **Por qué era un problema:** No describen su contenido.
* **Cómo lo corregí:** Renombrados a `nota1`, `nota2`, `nota3`, `resultadoPromedio`, `resultadoEstado`.


* **`<title>pagina</title>`**
* **Por qué era un problema:** No identifica la página en el navegador.
* **Cómo lo corregí:** Cambiado a "Calculadora de Promedio de Notas".


* **Función comentada calcularAntiguo**
* **Por qué era un problema:** Código muerto que no cumple ninguna función.
* **Cómo lo corregí:** Eliminada.


* **console.log(...) sueltos**
* **Por qué era un problema:** Restos de depuración innecesarios.
* **Cómo lo corregí:** Eliminados.


* **onclick="calc()" inline en el HTML**
* **Por qué era un problema:** Mezcla HTML y lógica JS.
* **Cómo lo corregí:** Reemplazado por `addEventListener`.


* **`<label>` sin atributo for**
* **Por qué era un problema:** No están asociadas a su `<input>` (accesibilidad).
* **Cómo lo corregí:** Se añadió `for` enlazando cada label a su input.


* **Clase CSS .cont1**
* **Por qué era un problema:** Nombre no descriptivo.
* **Cómo lo corregí:** Renombrada a `.contenedor`.



**Sitio publicado**
🔗 [URL de Netlify aquí]

**Estructura de ramas**

* **main:** versión estable y publicada.
* **dev:** integración de features antes de pasar a main.
* **pruebas:** rama de pruebas.
* **feature/correcciones:** rama de trabajo donde se aplicaron las correcciones.
