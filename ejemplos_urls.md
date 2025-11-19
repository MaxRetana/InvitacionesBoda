# Ejemplos de URLs con parámetros

## Cómo usar los parámetros en la URL

Ahora puedes personalizar la invitación pasando parámetros por la URL:

### Parámetros disponibles:
- `nombre`: Nombre completo del invitado
- `invitados`: Cantidad de personas (número del 1 al 9)

### Ejemplos de URLs:

#### Solo nombre:
```
index.html?nombre=Juan%20Pérez
```

#### Solo cantidad de invitados:
```
index.html?invitados=2
```

#### Nombre y cantidad de invitados:
```
index.html?nombre=María%20García&invitados=4
```

#### Nombre con acentos y cantidad:
```
index.html?nombre=José%20Rodríguez&invitados=3
```

#### Familia completa:
```
index.html?nombre=Familia%20Martínez&invitados=6
```

### Cómo funciona:

1. **Solo nombre**: El campo nombre se rellena automáticamente y se vuelve de solo lectura
2. **Solo invitados**: Se preselecciona "Sí, asistiré" y la cantidad de personas especificada
3. **Ambos parámetros**: Se rellenan ambos campos y se vuelven de solo lectura
4. **Sin parámetros**: El formulario funciona normalmente, permitiendo edición libre

### Notas técnicas:
- Los espacios en los nombres deben codificarse como `%20`
- Los acentos y caracteres especiales se manejan automáticamente
- La cantidad de invitados debe ser un número entre 1 y 9
- Si se especifica la cantidad de invitados, automáticamente se marca "Sí, asistiré"