# A continuación se presentan algunos cambios relevantes en el código de forma general.

## En el campo "Estado" de la entidad Orden.java:

Se hizo el cambio en el campo **Estado**:

```
@Column(name = "estado", nullable = false, length = 1)
@Enumerated(EnumType.STRING)
private EstadoOrden estado;
```

## En el campo "Estado" de la entidad Orden.java:

Se hizo el cambio en el campo **Estado**:

```
@Column(name = "estado", nullable = false, length = 20)
    @Enumerated(EnumType.STRING)
    private EstadoOrden estado;
```

## Cambiar el estado usuario por username en Usuario.java.

- Ponerle **nullable = true;**.
- Eliminar el campo en la base de datos (campo usuario).
- Actualizar el campo con:
````
select * from public.usuarios;
UPDATE public.usuarios
SET username = 'cear'
WHERE id = 1;
````
- Regresar el campo a **nullable = false;** (campo de username).
- Ejecutar nuevamente el Proyecto para ver los cambios.

<img width="921" height="121" alt="image" src="https://github.com/user-attachments/assets/135e5d51-994f-4045-b402-a92bfa77ca85" />

