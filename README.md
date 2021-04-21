# parcel-simple-test

This is pretty straightforward: adding the same asset multiple times to an HTML file (for example) results in 404, because the path doesn't get updated globally.

```html
<img src="image.svg" />
<img src="image.svg" />
<img src="image.svg" />
```

becomes

```html
<img src="assets/image.c9a7e9b8.svg" />
<img src="image.c9a7e9b8.svg" />
<img src="image.c9a7e9b8.svg" />
```

instead of

```html
<img src="assets/image.c9a7e9b8.svg" />
<img src="assets/image.c9a7e9b8.svg" />
<img src="assets/image.c9a7e9b8.svg" />
```

## Building and running on localhost

First install dependencies:

```sh
npm install
```

To create a production build:

```sh
npm run build
```

## Credits

Made with [createapp.dev](https://createapp.dev/)
