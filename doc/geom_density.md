---
title: Geom.density
author: Daniel Jones
order: 7
...

Draw a kernel density estimate from data. An alias for `Geom.line` with
`Stat.density`.

# Aesthetics

  * `x`: Sample to draw density estimate from.

# Examples

```{.julia hide="true" results="none"}
using RDatasets
using Gadfly

Gadfly.prepare_display()
Gadfly.set_default_plot_size(14cm, 8cm)
```

```julia
plot(data("ggplot2", "diamonds"), x="price", Geom.density)
```

```julia
plot(data("ggplot2", "diamonds"), x="price", color="cut", Geom.density)
```
