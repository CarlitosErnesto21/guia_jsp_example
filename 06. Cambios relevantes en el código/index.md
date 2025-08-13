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
