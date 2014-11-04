# sg-wiredep

This is a fork of the original [wiredep](https://github.com/taptapship/wiredep) project maintained by the [SunGard team](https://github.com/SunGard-Labs). It implements the following extra functionalities:

- Supports *multiple dots on file names extensions*, it allows you to have multiple places to insert the same kind of files. See the example below:
```html
<html>
  <head>
    <!-- bower:min.js -->
    <!-- endbower -->
  </head>
  <body>
    <!-- bower:js -->
    <!-- endbower -->
  </body>
</html>
```

- Support to a *files* property on `bower.json`. This was a subset created when trying to overcome some of the limitations from the Bower main property. See an example below:
```json
{
  "name": "test",
  "version": "0.0.0",
  "files": {
    "styles": [
      "app/style/test.css"
    ],
    "scripts": [
      "app/scripts/app.js",
      "app/scripts/test.js"
    ]
  }
}
```

### Grunt plugin
We also support a [fork of the original grunt-wiredep plugin](https://github.com/SunGard-Labs/grunt-wiredep) that uses this fork instead.

You can install it with:

```shell
npm install --save-dev https://github.com/SunGard-Labs/grunt-wiredep/archive/master.tar.gz
```

## License

Copyright (c) 2014 Stephen Sawchuk. Licensed under the MIT license.

