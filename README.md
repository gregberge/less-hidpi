# Less hidpi mixin

`hidpi()` is a Less mixin that automatically serves high resolution graphics to high density (Retina-like) displays.

## How to use

First you must import the mixin :

```less
@import "hidpi"
```

Then you can use the mixin :

```less
.logo {
  .hidpi('logo.png', 100px, 100px);
}
```

Automatically, it will use `logo@2x.png` on high density devices.

## Configuration

You can configure the mixins using some variables :

```less
@hidpi_min_ratio: 1.5;
@hidpi_suffix: "@2x";
```

## Credits

This mixin is inspired by [Retina JS](https://github.com/imulus/retinajs).

## License

MIT