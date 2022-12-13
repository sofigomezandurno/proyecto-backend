# USO DEL OBJETO PROCESS

Realizar una aplicación en Node.js que permita recibir como parámetros una cantidad ilimitada de números, con los cuales debe confeccionar el siguiente objeto (se imprimirá por consola):

```javascript
{
	datos: {
		numeros: [los, numeros, ingresados],
		promedio: (el promedio entre ellos),
		max: (valor máximo),
		min: (valor mínimo),
		ejecutable: (nombre del ejecutable),
		pid: (process id)
	}
}
```

En el caso de ingresar un número no válido, se creará un objeto de error con el siguiente formato (se imprimirá por consola):

```javascript
{
	error: {
	descripcion: 'error de tipo',
	numeros: [array, de, entrada], // ej.[1, 2, 'pepe', 4, true]
	tipos: [array, con, tipos, de, entrada] // ej.[number, number, string, number, boolean]
	}
}

```

En este caso de error, la aplicación saldrá con código de error -5

Si no ingresó ningún número, el objeto de error será:

```javascript
{
	error: {
		descripcion: 'entrada vacía';
	}
}
```

En este caso de error, la aplicación saldrá con código de error -4

En los casos de error, se representará en consola el código antes de finalizar.
