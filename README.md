# CURSO: APRENDE BLAZOR

# LECCIÓN 26: Restricciones en una ruta a un componente (Route Constraints)

1. Abrir la aplicación con Visual Studio 2022 o VSCode

2. Este es el código del componente que muestra la restricciones en los parámetros.

En primer lugar hemos incluido un parámetro de tipo entero en la ruta, y también hemos incluid un parámetro de tipo buleano en la ruta

```razor
@* Restricciones (Route Constraints) en una ruta en Blazor *@

@page "/"

@page "/home/{id1:int}"

@page "/home/{id1:int}/{parametro2:bool}"

<PageTitle>Home</PageTitle>

<h1>Hello, world!</h1>

Welcome to your new app.

<p>Product ID: @Id1</p>

<p>Product ID: @Parametro2</p>

@code {
    [Parameter]
    public int? Id1 { get; set; }

    [Parameter]
    public bool? Parametro2 { get; set; }
}
```
