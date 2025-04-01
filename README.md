# Comparación de Tecnologías Frontend y Mobile

## 1 React vs Vue

### React
- Es una librería
- Tiene una comunidad más grande
- Utiliza formato JSX/TSX (HTML en JavaScript)

### Vue
- Framework progresivo
- Sintaxis basada en templates
- Curva de aprendizaje menor

### Recomendación
React es más recomendable para proyectos grandes y equipos que ya dominen esta tecnología. Vue es bueno para proyectos pequeños que requieren desarrollo rápido. Ambos pueden usarse para lo mismo.

## 2 Flutter vs React Native

### Flutter
- Alto rendimiento gracias a la compilación a código nativo
- Soporte para 120fps (Dispositivos android con 120hz o iPhone con Pro-motion se benefician de la fluidez)
- Diseño más consistente entre iOS y Android (Me pasa que Flutter es más Pixel perfect que react native)



## 3 Gestión de Estado

### React
- **Redux**: Patrón global recomendado para estados complejos
- **Context API**: Gestión de estado simple por defecto, pero no recomendada por su baja optimización

### Flutter
- **Provider**: Ofrece simplicidad sin renunciar a la eficienci
- **Bloc**: Patrón basado en eventos y streams, ideal para código escalable
- **Riverpod**: Evolución de Provider, más flexible y mejor rendimiento

## 4 Mejores Prácticas

### React.js
- Utilizar `React.memo` y `useMemo` para evitar renders innecesarios
- Implementar carga lazy de componentes (`React.lazy` y `Suspense`)
- Minimizar actualizaciones innecesarias en el estado global

### Flutter
- Evitar reconstrucciones innecesarias con `const` widgets y `ValueNotifier`
- Preferir `ListView.builder` sobre `ListView` estático
- Optimizar imágenes con `cached_network_image`
- Evitar el uso excesivo de `setState`, preferir soluciones como `Provider`, `Bloc` o `Riverpod` para una gestión de estado más eficiente

### React Native
- Implementar `React.memo` y `FlatList` en lugar de `ScrollView`

## 5 Despliegues

