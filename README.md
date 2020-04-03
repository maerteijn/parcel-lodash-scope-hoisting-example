# A parcel-lodash-scope-hoisting example
Example repo which demonstrates a weird thing with parcel, scope hoisting and lodash.

This branch is using parcel with the the (4410-parcel-1-fix-global-insertions)[https://github.com/maerteijn/parcel/tree/4410-parcel-1-fix-global-insertions] branch

## Before testing:
```
yarn run parcel-dev
yarn run install
```

See https://github.com/parcel-bundler/parcel/issues/4410

See also the `with-4410-parcel-1-fix-global-insertions` branch with a proposed fix

## Without --experimental-scope-hoisting
```bash
yarn run build
```

Open `dist/index.html` in a browser, no error


## With --experimental-scope-hoisting
```bash
yarn run build:scope-hoisting
```

Open `dist/index.html` in a browser, no error as well, so the scope hoisting works now as expected!
