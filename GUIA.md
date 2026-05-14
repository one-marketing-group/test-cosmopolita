# Test de Piel · Cosmopolita — MVP

## Estructura

```
cosmopolita-test/
├── api/
│   └── rutina.js        ← Backend (proxy seguro a Anthropic)
├── public/
│   └── index.html       ← Frontend del test
├── vercel.json          ← Configuración de Vercel
└── README.md
```

## Cómo hacer deploy en Vercel

### 1. Subir a GitHub

- Crea un repositorio nuevo en github.com
- Sube estos archivos

### 2. Conectar a Vercel

- Ve a vercel.com → "Add New Project"
- Importa el repositorio de GitHub
- Haz click en Deploy

### 3. Agregar la API Key

- En Vercel → tu proyecto → Settings → Environment Variables
- Agrega:
  - **Name:** `ANTHROPIC_API_KEY`
  - **Value:** tu key (empieza con `sk-ant-...`)
- Guarda y haz **Redeploy**

## Obtener API Key gratis

1. Ve a https://console.anthropic.com
2. Regístrate (gratis)
3. Ve a "API Keys" → "Create Key"
4. Copia la key y pégala en Vercel

## Costo estimado

- Menos de $0.003 por test completado
- 500 tests ≈ $1.50 USD
