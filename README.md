# A parcel-lodash-scope-hoisting example
Example repo which demonstrates a weird thing with parcel, scope hoisting and lodash

## Without --experimental-scope-hoisting
```bash
npm run build
```

Open `dist/index.html` in a browser, no error


## With --experimental-scope-hoisting
```bash
npm run build:scope-hoisting
```

Open `dist/index.html` in a browser, see the console:

```
ReferenceError: require is not defined
```
