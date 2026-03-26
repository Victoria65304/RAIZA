# Raiza — Diseño desde la Raíz

Sitio web oficial de Raiza, marca ecuatoriana de diseño limitado.

## Estructura

```
raiza/
├── index.html                    → Inicio
├── colecciones.html              → Todas las colecciones
├── trazabilidad.html             → Qué es la trazabilidad
├── nosotros.html                 → El equipo
├── eventos.html                  → Dónde estamos (ferias/bazares)
├── contacto.html                 → WhatsApp + Instagram
├── colecciones/
│   └── riviel/
│       └── index.html            → Colección 01: Riviel
├── styles/
│   └── main.css                  → Estilos globales
└── data/
    └── eventos.json              → ← EDITAR AQUÍ LOS EVENTOS
```

## Cómo actualizar eventos

Abre `data/eventos.json` y edita la lista. Cada evento tiene esta estructura:

```json
{
  "id": 1,
  "nombre": "El Gran Bazar",
  "lugar": "Quito, Ecuador",
  "direccion": "Centro comercial X, Stand 12",
  "fecha_dia": "15",
  "fecha_mes": "ABR",
  "fecha_año": "2025",
  "descripcion": "Descripción breve del evento.",
  "activo": true
}
```

- `activo: true` → muestra "Confirmado"
- `activo: false` → muestra "Próximamente"

Para agregar un evento nuevo, copia un bloque y pégalo en la lista (separado por coma).  
Para eliminar uno, borra el bloque completo.

## Cómo actualizar datos de contacto

Busca en estos archivos las líneas con `"Por confirmar"`:

- `contacto.html` → WhatsApp e Instagram
- `index.html` → datos bancarios en el modal de pago
- `colecciones/riviel/index.html` → datos bancarios en el modal de pago

## Cómo agregar una nueva colección

1. Crea una carpeta: `colecciones/[nombre]/`
2. Copia `colecciones/riviel/index.html` como base
3. Cambia colores, textos y productos
4. Agrégala en `colecciones.html`

## Deploy

El sitio está publicado en [Vercel](https://vercel.com). Cada push a `main` actualiza el sitio automáticamente.
