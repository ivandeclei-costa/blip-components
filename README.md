# blip-components

BLiP components to use in AngularJS (1.x) applications.

## Usage

Install blip-components via npm:

```
$ npm install blip-components
```

Then, use it as module on your angularjs application

```
import * as blipComponents from 'blip-components';
import 'blip-components/dist/blip-components.css';

const componentNames = components =>
    Object.keys(components).map(c => components[c]);

const app = angular
    .module('myApp', [
        ...componentNames(blipComponents)
    ])
    ...
```

You can also use each component separately

```
import { BlipInputComponent } from 'blip-components';
import 'blip-components/dist/blip-components.css';

const app = angular
    .module('myApp', [
        BlipInputComponent
    ])
    ...
```

Remeber to import the css file to style your components

## Building

If you want to contribute to our project, clone this project and, on root directory, run `npm start`. A new process will be started
on port `3000`, and all changes will be tracked.

To finish a build, run `npm run build`.

## License
`blip-components` is under the [ISC license](https://opensource.org/licenses/ISC).
