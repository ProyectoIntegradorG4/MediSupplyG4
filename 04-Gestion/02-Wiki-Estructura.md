# Estructura de la Wiki - MediSupply

## Páginas Principales de la Wiki

### 1. **Home** (Página Principal)
- Descripción general del proyecto
- Enlaces rápidos a documentación importante
- Estado actual del proyecto
- Equipo de trabajo

### 2. **Arquitectura del Sistema**
- Diagrama de arquitectura general
- Componentes principales
- Stack tecnológico
- Decisiones de diseño
- Patrones arquitectónicos utilizados

### 3. **Guías de Desarrollo**
- Configuración del entorno de desarrollo
- Estándares de código
- Proceso de revisión de código
- Guías de testing
- Convenciones de nomenclatura

### 4. **APIs y Documentación Técnica**
- Documentación de APIs REST
- Especificaciones de endpoints
- Ejemplos de uso
- Códigos de error
- Autenticación y autorización

### 5. **Base de Datos**
- Modelo de datos
- Diagrama ER
- Esquemas de tablas
- Migraciones
- Consultas optimizadas

### 6. **Despliegue y DevOps**
- Configuración de ambientes
- Proceso de despliegue
- Variables de entorno
- Monitoreo y logging
- Backup y recuperación

### 7. **Testing y Calidad**
- Estrategia de testing
- Pruebas unitarias
- Pruebas de integración
- Pruebas de rendimiento
- Criterios de calidad

### 8. **Gestión de Proyecto**
- Metodología de trabajo
- Roles y responsabilidades
- Proceso de toma de decisiones
- Comunicación del equipo
- Retrospectivas

## Contenido Detallado por Página

### Home
```markdown
# MediSupply - Wiki del Proyecto

## Descripción
MediSupply es una plataforma integral para la optimización de la cadena de suministros médicos.

## Estado Actual
- **Fase**: [Arquitectura/Desarrollo/Testing/Despliegue]
- **Sprint**: [X de Y]
- **Progreso**: [X%]

## Enlaces Rápidos
- [Arquitectura del Sistema](./Arquitectura-del-Sistema)
- [Guías de Desarrollo](./Guias-de-Desarrollo)
- [APIs y Documentación](./APIs-y-Documentacion)
- [Base de Datos](./Base-de-Datos)
- [Despliegue y DevOps](./Despliegue-y-DevOps)

## Equipo
- **Product Owner**: [Nombre]
- **Scrum Master**: [Nombre]
- **Tech Lead**: [Nombre]
- **Desarrolladores**: [Nombres]

## Próximas Reuniones
- **Daily Standup**: Lunes a Viernes 9:00 AM
- **Sprint Planning**: Lunes 10:00 AM
- **Sprint Review**: Viernes 2:00 PM
- **Retrospectiva**: Viernes 3:00 PM
```

### Arquitectura del Sistema
```markdown
# Arquitectura del Sistema

## Visión General
Sistema distribuido con arquitectura de microservicios para alta disponibilidad y escalabilidad.

## Componentes Principales

### Frontend Web
- **Tecnología**: React.js
- **Responsabilidades**: Interfaz de usuario para administradores
- **Características**: SPA, responsive, multilenguaje

### Backend APIs
- **Tecnología**: Node.js/Express
- **Responsabilidades**: Lógica de negocio y APIs REST
- **Características**: Stateless, autenticación JWT

### Base de Datos
- **Tecnología**: PostgreSQL
- **Responsabilidades**: Almacenamiento persistente
- **Características**: ACID, replicación, backup automático

### Aplicación Móvil
- **Tecnología**: React Native
- **Responsabilidades**: Interfaz para comerciales y clientes
- **Características**: Offline-first, sincronización

## Diagramas
- [Diagrama de Componentes](./diagramas/componentes.png)
- [Diagrama de Secuencia](./diagramas/secuencia.png)
- [Diagrama de Despliegue](./diagramas/despliegue.png)

## Decisiones Técnicas
- **Base de Datos**: PostgreSQL por ACID y capacidades JSON
- **APIs**: REST por simplicidad y compatibilidad
- **Autenticación**: JWT por stateless y escalabilidad
- **Cache**: Redis para sesiones y datos frecuentes
```

### Guías de Desarrollo
```markdown
# Guías de Desarrollo

## Configuración del Entorno

### Prerrequisitos
- Node.js 18+
- PostgreSQL 14+
- Redis 6+
- Git

### Instalación
```bash
# Clonar repositorio
git clone [url-repositorio]

# Instalar dependencias
npm install

# Configurar variables de entorno
cp .env.example .env

# Ejecutar migraciones
npm run migrate

# Iniciar servidor de desarrollo
npm run dev
```

## Estándares de Código

### JavaScript/TypeScript
- **Linter**: ESLint
- **Formatter**: Prettier
- **Convenciones**: camelCase para variables, PascalCase para clases

### React
- **Componentes**: Funcionales con hooks
- **Estado**: Redux Toolkit
- **Testing**: Jest + React Testing Library

### Base de Datos
- **Migraciones**: Knex.js
- **ORM**: Prisma
- **Convenciones**: snake_case para tablas y columnas

## Proceso de Revisión de Código
1. Crear feature branch desde main
2. Implementar cambios siguiendo estándares
3. Ejecutar pruebas locales
4. Crear Pull Request
5. Revisión por pares obligatoria
6. Aprobación y merge

## Testing
- **Cobertura mínima**: 80%
- **Pruebas unitarias**: Jest
- **Pruebas de integración**: Supertest
- **Pruebas E2E**: Cypress
```

### APIs y Documentación
```markdown
# APIs y Documentación Técnica

## Autenticación
Todas las APIs requieren autenticación mediante JWT.

```http
Authorization: Bearer <token>
```

## Endpoints Principales

### Autenticación
```http
POST /api/auth/login
POST /api/auth/refresh
POST /api/auth/logout
```

### Productos
```http
GET /api/products
GET /api/products/:id
POST /api/products
PUT /api/products/:id
DELETE /api/products/:id
```

### Inventario
```http
GET /api/inventory
GET /api/inventory/:productId
PUT /api/inventory/:productId
```

### Pedidos
```http
GET /api/orders
POST /api/orders
GET /api/orders/:id
PUT /api/orders/:id/status
```

## Códigos de Error
- `400`: Bad Request
- `401`: Unauthorized
- `403`: Forbidden
- `404`: Not Found
- `500`: Internal Server Error

## Ejemplos de Uso
Ver [ejemplos de uso](./ejemplos-api.md)
```

### Base de Datos
```markdown
# Base de Datos

## Modelo de Datos

### Entidades Principales

#### Users
- id (PK)
- email
- password_hash
- role
- created_at
- updated_at

#### Products
- id (PK)
- name
- description
- category
- price
- supplier_id (FK)
- created_at
- updated_at

#### Inventory
- id (PK)
- product_id (FK)
- warehouse_id (FK)
- quantity
- lot_number
- expiry_date
- created_at
- updated_at

#### Orders
- id (PK)
- client_id (FK)
- status
- total_amount
- created_at
- updated_at

## Diagrama ER
[Ver diagrama ER](./diagramas/er-diagram.png)

## Migraciones
```bash
# Crear nueva migración
npm run migrate:create

# Ejecutar migraciones
npm run migrate:up

# Revertir migración
npm run migrate:down
```

## Consultas Optimizadas
Ver [consultas optimizadas](./consultas-optimizadas.md)
```

### Despliegue y DevOps
```markdown
# Despliegue y DevOps

## Ambientes

### Desarrollo
- **URL**: https://dev.medisupply.com
- **Base de Datos**: PostgreSQL local
- **Cache**: Redis local

### Staging
- **URL**: https://staging.medisupply.com
- **Base de Datos**: PostgreSQL en nube
- **Cache**: Redis en nube

### Producción
- **URL**: https://medisupply.com
- **Base de Datos**: PostgreSQL cluster
- **Cache**: Redis cluster

## Variables de Entorno
```env
# Base de Datos
DATABASE_URL=postgresql://user:pass@host:port/db
REDIS_URL=redis://host:port

# JWT
JWT_SECRET=your-secret-key
JWT_EXPIRES_IN=24h

# APIs Externas
REGULATORY_API_URL=https://api.regulatory.com
WEATHER_API_KEY=your-api-key
```

## Proceso de Despliegue
1. Merge a main branch
2. GitHub Actions ejecuta pruebas
3. Build de aplicación
4. Despliegue automático a staging
5. Pruebas en staging
6. Despliegue manual a producción

## Monitoreo
- **Logs**: ELK Stack
- **Métricas**: Prometheus + Grafana
- **Alertas**: PagerDuty
- **Uptime**: Pingdom

## Backup
- **Frecuencia**: Diario
- **Retención**: 30 días
- **Ubicación**: S3
- **Restauración**: 4 horas máximo
```

### Testing y Calidad
```markdown
# Testing y Calidad

## Estrategia de Testing

### Pirámide de Testing
- **Unit Tests**: 70%
- **Integration Tests**: 20%
- **E2E Tests**: 10%

### Pruebas Unitarias
```javascript
// Ejemplo de prueba unitaria
describe('ProductService', () => {
  it('should create a new product', async () => {
    const product = await ProductService.create({
      name: 'Test Product',
      price: 100
    });
    
    expect(product.name).toBe('Test Product');
    expect(product.price).toBe(100);
  });
});
```

### Pruebas de Integración
```javascript
// Ejemplo de prueba de integración
describe('Product API', () => {
  it('should return products list', async () => {
    const response = await request(app)
      .get('/api/products')
      .set('Authorization', `Bearer ${token}`);
    
    expect(response.status).toBe(200);
    expect(response.body).toHaveLength(10);
  });
});
```

### Pruebas E2E
```javascript
// Ejemplo de prueba E2E
describe('Product Management', () => {
  it('should create and edit a product', () => {
    cy.visit('/products');
    cy.get('[data-testid="add-product"]').click();
    cy.get('[data-testid="product-name"]').type('New Product');
    cy.get('[data-testid="save-product"]').click();
    cy.contains('New Product').should('be.visible');
  });
});
```

## Criterios de Calidad
- **Cobertura de código**: ≥80%
- **Duplicación**: ≤3%
- **Complejidad ciclomática**: ≤10
- **Deuda técnica**: ≤5 días
- **Tiempo de respuesta**: ≤2 segundos

## Herramientas
- **Linting**: ESLint
- **Formatting**: Prettier
- **Testing**: Jest, Cypress
- **Coverage**: Istanbul
- **SonarQube**: Análisis de calidad
```

### Gestión de Proyecto
```markdown
# Gestión de Proyecto

## Metodología
- **Framework**: Scrum
- **Sprint Duration**: 2 semanas
- **Daily Standup**: 15 minutos
- **Sprint Planning**: 2 horas
- **Sprint Review**: 1 hora
- **Retrospectiva**: 1 hora

## Roles y Responsabilidades

### Product Owner
- Definir y priorizar backlog
- Aceptar/rechazar entregables
- Comunicar con stakeholders
- Maximizar valor del producto

### Scrum Master
- Facilitar eventos Scrum
- Remover impedimentos
- Mejorar procesos
- Coaching del equipo

### Tech Lead
- Decisiones técnicas
- Arquitectura del sistema
- Estándares de código
- Mentoring técnico

### Desarrolladores
- Implementar features
- Testing y documentación
- Revisión de código
- Mejora continua

## Proceso de Toma de Decisiones
1. **Técnicas**: Tech Lead + equipo
2. **Producto**: Product Owner
3. **Proceso**: Scrum Master + equipo
4. **Estratégicas**: Product Owner + stakeholders

## Comunicación
- **Canal principal**: Slack
- **Documentación**: GitHub Wiki
- **Reuniones**: Google Meet
- **Tracking**: GitHub Projects

## Retrospectivas
- **Frecuencia**: Cada sprint
- **Duración**: 1 hora
- **Formato**: Start/Stop/Continue
- **Acciones**: Seguimiento en GitHub Issues
```

---

**Universidad de los Andes** | Vigilada Mineducación

Reconocimiento como Universidad: Decreto 1297 del 30 de mayo de 1964.
Reconocimiento personería jurídica: Resolución 28 del 23 de febrero de 1949 Minjusticia. 