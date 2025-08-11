# MediSupply - Proyecto Final MISW4501-202514

## Equipo de Trabajo - Grupo 4

| Integrantes	| Nombres	| Apellidos	| Correo electrónico @uniandes.edu.co |
|---|---|---|---|
| 1	| Juan Pablo	| Rodriguez Morales	| jp.rodriguezm@uniandes.edu.co| 
| 2 |	Luz Stella | 	Ochoa Marin	| ls.ochoa@uniandes.edu.co|
| 3 |	Julio César	| Forero Orjuela	| jc.foreroo1@uniandes.edu.co|
| 4 |	Wilson	| Aponte García	| w.aponte@uniandes.edu.co|

## Descripción del Proyecto

MediSupply es una empresa multinacional dedicada a la distribución de insumos médicos, medicamentos de alta complejidad y equipos biomédicos a instituciones de salud en América Latina. El proyecto consiste en desarrollar una plataforma tecnológica integral que optimice la cadena de suministros médicos.

## Estructura del Proyecto

```
MediSupplyG4/
├── 
├── wiki/                          # Wiki del proyecto (submódulo Git)
│   └── MediSupplyG4.wiki/        # Contenido de la wiki
│       ├── Home.md
│       ├── Semana-1.md
│       ├── Semana-2.md
│       ├── Semana-3.md
│       ├── Semana-4.md
│       ├── Semana-5.md
│       ├── Semana-6.md
│       ├── Semana-7.md
│       ├── Semana-8.md
│       ├── 05-Entregables/
│       └── DocumentosOficiales/
├── LICENSE
└── README.md
```

## Cronograma del Proyecto

- **Semanas 1-8**: Diseño de arquitectura y pruebas de concepto
- **Semanas 9-16**: Desarrollo de la primera versión de la aplicación
- **Semana 16**: Entrega final del prototipo

## Stack Tecnológico Seleccionado

### Backend
- **Framework**: Python Flask
- **Base de Datos**: PostgreSQL/MySQL
- **Autenticación**: JWT (JSON Web Tokens)
- **APIs**: RESTful APIs con documentación Swagger

### Frontend Web
- **Framework**: React.js
- **Estado**: Redux/Context API
- **UI**: Material-UI o Ant Design
- **Internacionalización**: i18next

### Aplicación Móvil
- **Framework**: React Native
- **Plataformas**: Android e iOS
- **Navegación**: React Navigation
- **Estado**: Redux Toolkit

### Infraestructura
- **Cloud**: AWS (Amazon Web Services)
- **Contenedores**: Docker
- **CI/CD**: GitHub Actions
- **Monitoreo**: CloudWatch, Sentry

### Calidad y Testing
- **Backend**: pytest, coverage
- **Frontend**: Jest, React Testing Library
- **Móvil**: Jest, Detox
- **E2E**: Cypress, Appium

## Enlaces Importantes

- [Acta de Constitución](./DocumentacionProyecto/01-Planificacion/01-Acta-Constitucion.md)
- [Épicas y Features](./DocumentacionProyecto/01-Planificacion/02-Epicas-Features.md)
- [Planificación de Sprints](./DocumentacionProyecto/01-Planificacion/03-Planificacion-Sprints.md)
- [Documento de Alcance](./DocumentacionProyecto/02-Arquitectura/01-Documento-Alcance.md)
- [Wiki del Proyecto](./wiki/MediSupplyG4.wiki/Home.md)

## Estado del Proyecto

### ✅ Completado (Semana 1)
- [x] Acta de Constitución del Proyecto
- [x] Épicas y Features del Sistema
- [x] Planificación de Sprints
- [x] Guía para Video de Entrega

### 🔄 En Progreso (Semana 2)
- [x] Documento del Alcance (EDT) - Completado
- [x] Hoja de Trabajo con Objetivos y Restricciones - Completado
- [x] Documento de Estrategia de Pruebas - Completado
- [ ] Visión de Arquitectura - En desarrollo
- [ ] Modelos de Arquitectura (Contexto, Dominio, Componentes, Despliegue)
- [ ] Board del Proyecto actualizado
- [ ] Showcase de la Semana 2

### 📋 Pendiente
- [ ] Experimentos de Arquitectura
- [ ] Prototipos de Prueba de Concepto
- [ ] Desarrollo de la Aplicación

## Clonación del Proyecto

### Clonar todo (proyecto + submódulos):
```bash
git clone --recurse-submodules git@github.com:ProyectoIntegradorG4/MediSupplyG4.git
```

### Si ya clonado:
```bash
git submodule update --init --recursive
```

### Actualizar submódulos:
```bash
git submodule update --remote
```

## Flujo de Trabajo con Git

### Hacer cambios en el repositorio principal:
```bash
# 1. Verificar estado del repositorio
git status

# 2. Agregar cambios
git add .

# 3. Hacer commit
git commit -m "Descripción de los cambios realizados"

# 4. Subir cambios
git push origin main
```

### Hacer cambios en la wiki (submódulo):
```bash
# 1. Navegar al directorio de la wiki
cd wiki/MediSupplyG4.wiki

# 2. Verificar estado
git status

# 3. Agregar cambios
git add .

# 4. Hacer commit
git commit -m "Actualización de la wiki: descripción de cambios"

# 5. Subir cambios de la wiki
git push

# 6. Volver al directorio principal
cd ../..

# 7. Actualizar la referencia del submódulo en el repo principal
git add wiki
git commit -m "Actualizar referencia del submódulo wiki"
git push
```

### Flujo completo para cambios en ambos repositorios:
```bash
# Si haces cambios en ambos repositorios, sigue este orden:

# 1. Primero actualiza la wiki
cd wiki/MediSupplyG4.wiki
git add .
git commit -m "Cambios en la wiki"
git push
cd ../..

# 2. Luego actualiza el repositorio principal
git add .
git commit -m "Cambios en el proyecto principal + actualización de wiki"
git push origin main
```

### Comandos útiles para gestión de submódulos:
```bash
# Ver estado de todos los submódulos
git submodule status

# Inicializar submódulos si no están configurados
git submodule init

# Actualizar submódulos a la última versión
git submodule update --remote

# Ver diferencias en submódulos
git diff --submodule
```

## Entregables de la Semana 2

### ✅ Completados
- **Documento del alcance**: EDT en formato árbol y tabular
- **Hoja de trabajo**: Objetivos, restricciones y requisitos de calidad
- **Estrategia de pruebas**: Componentes, alcance y tipos de pruebas

### 🔄 En Desarrollo
- **Visión de arquitectura**: Modelos de contexto, dominio, componentes y despliegue
- **Board del proyecto**: Actualización del tablero Kanban
- **Showcase**: Video de presentación de la semana 2

---

**Última actualización**: Semana 2 - Proyecto MISW4501-202514


