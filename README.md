# lab001-laravel

O objetivo é adicionar uma página intermediária para controlar o carregamento da página subsequente

## Diagrama de sequência

```
[Navegador]                           [Middleware]                          [Server]

 |          acessaPaginaDemorada() ->       |
 |          <- paginaDeEspera()             |
                                            | carregaPaginaDemorada() ->        |
                                            | <- resultadoPaginaDemorada()      |
 |    <- redirecionaPaginaResultado()       |
```
