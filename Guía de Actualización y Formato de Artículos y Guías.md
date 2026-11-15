---
title: "Guía Oficial de Actualización y Formato de Artículos y Guías Contables"
channel: "Contabletip"
type: "documentacion-editorial"
date: 2026-11-15
tags:
  - guia-editorial
  - documentacion
  - contabletip
  - contabilidad
  - tributaria
  - niif
  - normas-estandar
---

# 📖 Guía Oficial de Actualización y Formato: Bóveda Contabletip

> [!abstract] 🎯 Propósito del Estándar
> Esta guía establece la norma editorial y metodológica para la catalogación, redacción y estructuración de notas de contabilidad, tributación, derecho laboral, finanzas y plantillas en la bóveda de Obsidian de **Contabletip**.

---

## 🗂️ 1. Arquitectura de Directorios y Organización

La bóveda se organiza en directorios temáticos modulares según las grandes áreas del ejercicio contable y financiero:

```text
📁 C:\Users\rolando\Desktop\contabletip\
├── 📑 00 - Índice General.md                  <-- MOC y Directorio Central Maestro
├── 📑 Guía de Actualización y Formato...md    <-- Norma editorial (este documento)
├── 📁 Categorias/
│   ├── 📁 01 - Contabilidad General/
│   │   ├── 📑 01 - Contabilidad General.md   <-- Hub temático del área
│   │   └── 📁 Articulos/ (Notas individuales YYYY-MM-DD)
│   ├── 📁 02 - Tributaria e Impuestos/
│   ├── 📁 03 - Normas Internacionales (NIIF-NIC)/
│   ├── 📁 04 - Laboral y Nómina/
│   ├── 📁 05 - Finanzas y Costos/
│   └── 📁 06 - Plantillas y Formatos Excel/
```

---

## 🏷️ 2. Convención de Nomenclatura de Archivos

Cada artículo o guía debe guardarse con fecha de publicación sanitizada en formato ISO 8601:
`YYYY-MM-DD <Título del Artículo o Guía>.md`

- **Ejemplo correcto:** `2024-03-15 Tratamiento Contable de los Activos Fijos bajo NIIF para PYMES.md`
- **Caracteres prohibidos:** Se deben omitir caracteres no válidos para el sistema de archivos (`\`, `/`, `:`, `*`, `?`, `"`, `<`, `>`, `|`).

---

## 📄 3. Estructura Estándar de una Nota Contable

Toda nota técnica dentro de las carpetas de artículos debe seguir esta plantilla:

```markdown
---
title: "Título Oficial del Artículo o Guía"
date: YYYY-MM-DD
category: "[[Nombre de la Categoría]]"
url_fuente: "https://contabletip.blogspot.com/..."
tags:
  - contabletip
  - categoria/tributaria # o niif, laboral, etc.
  - tipo/guia # o plantilla, caso-practico
---

**Categoría:** [[Nombre de la Categoría]]  
**Fuente Oficial:** [Artículo en Contabletip.blogspot.com](https://contabletip.blogspot.com/...)  
**Índice General:** [[00 - Índice General]]

## Contenido Técnico

### 📌 Resumen Ejecutivo y Marco Normativo
Explicación clara del tema contable o tributario, contexto normativo vigente y a quién aplica.

### 🔑 Fundamentos y Marco Legal
- **Norma Aplicable:** Decretos, estatuto tributario o sección NIIF correspondiente.
- **Principio Contable:** Devengo, causación, prudencia o materialidad.
- **Sanciones o Riesgos:** Consecuencias del incumplimiento o error en la liquidación.

### 📊 Caso Práctico y Asiento Contable
| Código / Cuenta | Descripción | Debe | Haber |
| :--- | :--- | :---: | :---: |
| 1435 | Mercancías no fabricadas por la empresa | $ 10.000.000 | |
| 2408 | IVA Descontable (19%) | $ 1.900.000 | |
| 2365 | Retención en la fuente (2.5%) | | $ 250.000 |
| 2205 | Proveedores Nacionales | | $ 11.650.000 |

### 📈 Flujo de Proceso o Auditoría (Mermaid)
```mermaid
flowchart LR
    Factura["📄 Recepción Factura Electrónica"] --> Val["🔍 Validación DIAN / XML"]
    Val --> Asiento["⚙️ Registro Contable y Causación"]
    Asiento --> Pago["💰 Tesorería y Programación de Pago"]
```

### 💡 Puntos Clave y Recomendaciones del Experto
- Consejos prácticos de auditoría y conciliación fiscal.
- Verificación cruzada entre libros contables y declaraciones tributarias.
```
