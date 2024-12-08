# AI Profile Questionnaire

Una aplicación interactiva que ayuda a los usuarios a descubrir su perfil de uso de Inteligencia Artificial y obtener recomendaciones personalizadas para herramientas y proyectos.

## 🎯 Objetivo

Ayudar a los participantes a:
- Identificar qué herramientas de IA se adaptan mejor a su perfil
- Descubrir proyectos potenciales que pueden desarrollar
- Mejorar su capacidad para estructurar prompts efectivos
- Encontrar su camino en diferentes campos profesionales

## 🏗 Estructura del Proyecto

### Sistema de Análisis de Prompts
```
src/utils/prompts/
  ├── evaluation/           # Sistema de evaluación
  │   ├── promptEvaluator.ts
  │   ├── scoreCalculator.ts
  │   └── feedbackGenerator.ts
  ├── types.ts             # Definiciones de tipos
  └── __tests__/          # Pruebas unitarias
```

### Sistema de Mapeo de Dependencias
```
src/utils/dependencies/
  ├── DependencyMap.ts     # Gestión del grafo de dependencias
  ├── DependencyAnalyzer.ts # Análisis de relaciones
  ├── types.ts             # Tipos de dependencias
  └── index.ts             # Exportaciones públicas
```

### Componentes Modulares
```
src/components/
  ├── forms/               # Formularios modulares
  │   ├── basic/          # Formularios básicos
  │   └── prompts/        # Sistema de prompts
  ├── sections/           # Secciones principales
  └── layout/            # Componentes de estructura
```

## 🧪 Sistema de Pruebas

El proyecto incluye pruebas unitarias completas:

```bash
# Ejecutar pruebas
npm run test

# Ver cobertura de código
npm run coverage
```

## 💻 Tecnologías Utilizadas

- React + TypeScript
- Tailwind CSS
- Zustand
- Vite
- Vitest

## 🛠 Mejores Prácticas de Código

### Principio de Responsabilidad Única (SRP)
- Cada archivo tiene una única responsabilidad clara
- Facilita mantenimiento y testing
- Mejora la reutilización de código
- Permite escalabilidad controlada

### Organización de Archivos
- Archivos pequeños y enfocados
- Separación clara de responsabilidades
- Modularización efectiva
- Sistema de mapeo de dependencias

### Sistema de Dependencias
- Análisis de impacto de cambios
- Prevención de dependencias circulares
- Mapeo claro de relaciones entre archivos
- Facilita refactorización segura

### Mantenibilidad
- Código documentado
- Pruebas unitarias completas
- Tipos TypeScript estrictos
- Análisis de dependencias automatizado

## 📦 Gestión de Dependencias

El sistema incluye un analizador de dependencias que permite:

```typescript
const analyzer = new DependencyAnalyzer();

// Analizar impacto de cambios
const impact = analyzer.getImpactAnalysis('src/components/forms/BasicForm.tsx');

// Obtener dependencias
const deps = analyzer.getDependencies('src/utils/prompts/promptEvaluator.ts');
```

## 🤝 Contribución

1. Haz fork del repositorio
2. Crea una rama para tu feature
3. Asegúrate de:
   - Seguir el principio de responsabilidad única
   - Incluir pruebas unitarias
   - Actualizar el mapa de dependencias
4. Envía un pull request

## 📝 Licencia

MIT License