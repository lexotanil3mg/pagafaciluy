# PagaFácil UY - Node.js/React Version

## Descripción
PagaFácil UY es una plataforma profesional de recargas para Uruguay desarrollada con tecnologías modernas. Esta versión utiliza Node.js con Express en el backend y React con TypeScript en el frontend.

## Tecnologías Utilizadas
- **Frontend**: React 18 + TypeScript + Vite
- **Backend**: Node.js + Express + TypeScript
- **Styling**: Tailwind CSS + shadcn/ui
- **State Management**: Zustand + TanStack Query
- **Routing**: Wouter
- **Forms**: React Hook Form + Zod
- **Database**: In-memory storage (ready for PostgreSQL)

## Servicios Disponibles
- 📱 **Recarga Celular**: Antel, Claro y Movistar
- 🚌 **STM**: Sistema de Transporte Metropolitano
- 🚗 **Telepeaje**: Rutas nacionales
- 📺 **DirectTV**: TV Satelital
- 🅿️ **Estacionamiento**: Zona azul Montevideo

## Características
- ✅ Interfaz moderna y responsive
- ✅ Integración con bot de Telegram
- ✅ Sistema de carrito de compras
- ✅ Validación robusta de formularios
- ✅ Campos de pago ofuscados para seguridad
- ✅ Optimizado para Google Ads
- ✅ TypeScript para mayor confiabilidad

## Instalación

### Prerrequisitos
- Node.js 18+ 
- npm o yarn

### Pasos
1. Clona el repositorio:
```bash
git clone <tu-repositorio>
cd pagafacil_uy_nodejs
```

2. Instala las dependencias:
```bash
npm install
```

3. Inicia el servidor de desarrollo:
```bash
npm run dev
```

4. Abre tu navegador en `http://localhost:5000`

## Scripts Disponibles

- `npm run dev` - Inicia el servidor de desarrollo
- `npm run build` - Construye la aplicación para producción
- `npm run preview` - Previsualiza la build de producción
- `npm run type-check` - Verifica los tipos de TypeScript

## Configuración del Bot de Telegram

El bot está preconfigurado en `server/routes.ts`:
- Token: `7771329524:AAFcNnRhhs-QTgtWeTlDfcKIJ6aaXwNv5Es`
- Chat ID: `-4962524513`

## Estructura del Proyecto

```
pagafacil_uy_nodejs/
├── client/                 # Frontend React
│   ├── src/
│   │   ├── components/     # Componentes reutilizables
│   │   ├── pages/          # Páginas de la aplicación
│   │   ├── lib/            # Utilidades y servicios
│   │   └── hooks/          # Custom React hooks
├── server/                 # Backend Express
│   ├── index.ts           # Punto de entrada del servidor
│   ├── routes.ts          # Rutas de la API
│   ├── storage.ts         # Sistema de almacenamiento
│   └── vite.ts           # Configuración de Vite
├── shared/                # Esquemas compartidos
│   └── schema.ts         # Tipos y validaciones
└── package.json          # Dependencias y scripts
```

## Deployment

### Replit
El proyecto está optimizado para funcionar en Replit. Solo necesitas:
1. Hacer fork del proyecto
2. Ejecutar `npm run dev`

### Vercel
1. Conecta tu repositorio de GitHub a Vercel
2. Configura las variables de entorno si es necesario
3. Deploy automático

### Otros Hostings
1. Ejecuta `npm run build`
2. Sube la carpeta `dist` a tu hosting
3. Configura el servidor para servir archivos estáticos

## Seguridad
- Campos de pago ofuscados (cod01, x4, dato9)
- Validación de datos con Zod
- TypeScript para prevenir errores
- Headers de seguridad configurados

## API Endpoints

- `GET /api/health` - Health check
- `POST /api/payments` - Procesar pago

## Variables de Entorno

Puedes configurar las siguientes variables:
- `PORT` - Puerto del servidor (default: 5000)
- `NODE_ENV` - Ambiente (development/production)

## Contribución

1. Fork el proyecto
2. Crea una branch para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -am 'Agregar nueva funcionalidad'`)
4. Push a la branch (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## Soporte
Para cualquier consulta técnica o modificación, contactar al desarrollador.

---
© 2024 PagaFácil UY - Todos los derechos reservados