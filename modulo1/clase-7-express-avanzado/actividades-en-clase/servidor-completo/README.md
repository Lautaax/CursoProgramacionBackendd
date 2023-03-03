# Actividad en Clase: Servidor con GET, POST, PUT, DELETE

Crear una serie de endpoints que trabajen con la siguiente variable:

```
const frase = "Frase inicial";
```

## Especificación Endpoints

<table>
<tr> 
    <th> Verbo http</th>
    <th> Ruta</th>
    <th> Descripción</th>
    <th> Ejemplo Respuesta</th>
</tr>
<tr>
<td> 
<code>
    GET
</code>
</td>
<td>
<code>
/api/frase
</code>
</td>
<td> 
Retorna la frase completa
</td>
<td>

```json
{
  "frase": "frase completa"
}
```

</td>
</tr>

<tr>
<td> 
<code>
    GET
</code>
</td>
<td>
<code>
/api/palabras/:pos
</code>
</td>
<td> 
Retorna la palabra que se encuentra en la posición indicada (pos)
</td>
<td>

```json
{
  "buscada": "palabra"
}
```

</td>
</tr>

<tr>
<td> 
<code>
    POST
</code>
</td>
<td>
<code>
/api/palabras
</code>
</td>
<td> 
Agrega una palabra al final de la frase
</td>
<td>

```json
{
  "agregada": "palabra",
  "pos": 2
}
```

</td>
</tr>

<tr>
<td> 
<code>
    PUT
</code>
</td>
<td>
<code>
/api/palabras/:pos
</code>
</td>
<td> 
Reemplaza una palabra dentro de la frase según la posición dada
</td>
<td>

```json
{
  "palabra": "nueva palabra",
  "anterior": "palabra reemplazada"
}
```

</td>
</tr>

<tr>
<td> 
<code>
DELETE
</code>
</td>
<td>
<code>
/api/palabras/:pos
</code>
</td>
<td> 
Elimina una palabra de la frase según la posición dada
</td>
<td>

```json
{
  "mensaje": "palabra eliminada con exito"
}
```

</td>
</tr>
</table>

##### Nota: ten en cuenta que la primera palabra dentro de la variable `frase` tiene la posición #1