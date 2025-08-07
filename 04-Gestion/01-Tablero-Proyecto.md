# Tablero del Proyecto - MediSupply

## Estructura del Tablero en GitHub Projects

### Columnas del Tablero

#### 1. **Backlog**
- Features pendientes de asignación
- Tareas de investigación y análisis
- Bugs reportados
- Mejoras identificadas

#### 2. **To Do**
- Features asignadas al sprint actual
- Tareas listas para desarrollo
- Documentación pendiente
- Pruebas por realizar

#### 3. **In Progress**
- Features en desarrollo activo
- Tareas de implementación
- Revisión de código
- Testing en progreso

#### 4. **Review**
- Features completadas pendientes de revisión
- Pull requests abiertos
- Documentación por revisar
- Pruebas por validar

#### 5. **Testing**
- Features en fase de pruebas
- Validación de criterios de aceptación
- Pruebas de integración
- Pruebas de rendimiento

#### 6. **Done**
- Features completadas y validadas
- Documentación finalizada
- Entregables listos
- Funcionalidades desplegadas

### Etiquetas (Labels)

#### Por Tipo
- `feature` - Nueva funcionalidad
- `bug` - Corrección de errores
- `documentation` - Documentación
- `research` - Investigación y análisis
- `testing` - Pruebas y validación

#### Por Componente
- `web` - Componente web
- `mobile` - Aplicación móvil
- `api` - APIs y servicios
- `database` - Base de datos
- `infrastructure` - Infraestructura

#### Por Prioridad
- `high` - Alta prioridad
- `medium` - Prioridad media
- `low` - Baja prioridad

#### Por Sprint
- `sprint-1` - Semanas 1-4 (Arquitectura)
- `sprint-2` - Semanas 5-8 (Pruebas de concepto)
- `sprint-3` - Semanas 9-12 (Desarrollo Web)
- `sprint-4` - Semanas 13-16 (Desarrollo Móvil)

### Milestones (Hitos)

#### Milestone 1: Diseño de Arquitectura (Semanas 1-4)
- **Objetivo**: Definir arquitectura del sistema
- **Entregables**:
  - Documento de arquitectura
  - Diagramas de componentes
  - Decisiones técnicas
  - Stack tecnológico definido

#### Milestone 2: Pruebas de Concepto (Semanas 5-8)
- **Objetivo**: Validar decisiones técnicas
- **Entregables**:
  - Prototipos funcionales
  - Pruebas de rendimiento
  - Validación de integraciones
  - Documentación de APIs

#### Milestone 3: Desarrollo Web (Semanas 9-12)
- **Objetivo**: Implementar aplicación web
- **Entregables**:
  - Módulos principales web
  - APIs funcionales
  - Base de datos operativa
  - Sistema de autenticación

#### Milestone 4: Desarrollo Móvil (Semanas 13-16)
- **Objetivo**: Implementar aplicación móvil
- **Entregables**:
  - App móvil funcional
  - Integración con APIs
  - Pruebas de usuario
  - Documentación final

### Issues Template

#### Template para Features
```markdown
## Descripción
[Descripción clara de la funcionalidad]

## Criterios de Aceptación
- [ ] Criterio 1
- [ ] Criterio 2
- [ ] Criterio 3

## Estimación
- Tiempo estimado: [X] horas
- Complejidad: [Alta/Media/Baja]

## Dependencias
- [ ] Dependencia 1
- [ ] Dependencia 2

## Archivos a modificar
- [ ] Archivo 1
- [ ] Archivo 2

## Pruebas
- [ ] Prueba unitaria
- [ ] Prueba de integración
- [ ] Prueba de usuario
```

#### Template para Bugs
```markdown
## Descripción del Bug
[Descripción clara del problema]

## Pasos para reproducir
1. Paso 1
2. Paso 2
3. Paso 3

## Comportamiento esperado
[Lo que debería pasar]

## Comportamiento actual
[Lo que está pasando]

## Información adicional
- Navegador: [Chrome/Firefox/Safari]
- Versión: [X.X.X]
- Dispositivo: [Desktop/Mobile]
```

### Workflow de Desarrollo

#### 1. **Planificación Semanal**
- Revisión del backlog
- Asignación de tareas
- Estimación de esfuerzo
- Definición de criterios de aceptación

#### 2. **Desarrollo Diario**
- Stand-up diario (15 min)
- Actualización de estado de tareas
- Resolución de bloqueos
- Comunicación de progreso

#### 3. **Revisión de Código**
- Pull requests obligatorios
- Revisión por pares
- Pruebas automatizadas
- Documentación actualizada

#### 4. **Testing y Validación**
- Pruebas unitarias
- Pruebas de integración
- Pruebas de usuario
- Validación de criterios de aceptación

#### 5. **Despliegue**
- Despliegue en ambiente de desarrollo
- Pruebas en ambiente de staging
- Despliegue en producción
- Monitoreo post-despliegue

### Métricas del Proyecto

#### Velocidad del Equipo
- Story points completados por sprint
- Tiempo promedio por feature
- Tasa de completación

#### Calidad
- Bugs reportados vs resueltos
- Cobertura de pruebas
- Tiempo de resolución de bugs

#### Progreso
- Features completadas vs total
- Milestones alcanzados
- Entregables entregados a tiempo

### Automatizaciones

#### GitHub Actions
- Pruebas automáticas en pull requests
- Despliegue automático en staging
- Generación de reportes de cobertura
- Notificaciones de estado

#### Integraciones
- Slack para notificaciones
- Jira para tracking detallado (opcional)
- SonarQube para análisis de código
- Docker para containerización

---

**Universidad de los Andes** | Vigilada Mineducación

Reconocimiento como Universidad: Decreto 1297 del 30 de mayo de 1964.
Reconocimiento personería jurídica: Resolución 28 del 23 de febrero de 1949 Minjusticia. 