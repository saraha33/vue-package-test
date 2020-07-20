
# vue-package-test-x

> An example component library built with Vue CLI 3.

## Installation

### Directly in the browser

Drop the library in with a `<script>` tag alongside Vue:

```html
<div id="app">
<!-- ... use components here ... -->
</div>

<script src="https://unpkg.com/vue"></script>
<script src="https://unpkg.com/vue-package-test-x"></script>
<script>
new Vue({ el: '#app' })
</script>
```

Or, if you only want to use a small subset of components, drop them in individually:

```html
<div id="app">
<!-- ... use component here ... -->
</div>

<script src="https://unpkg.com/vue"></script>
<script src="https://unpkg.com/vue-package-test-x/HelloA"></script>
<script>
new Vue({ el: '#app' })
</script>
```

### In a module system

Install the library with NPM:

```bash
npm install vue-package-test-x
```

Then either import the library and either globally register all components with:

```js
import VuePackageTest from 'vue-package-test-x'

Vue.use(VuePackageTest)
```

or import and locally register a single component with:

```js
import { HelloA } from 'vue-package-test-x'

export default {
components: { VuePackageTest }
}
```

#### Individually packaged components

If you only want to use a small subset of components, import only individually packaged components to reduce the size of your application:

```js
import HelloA from 'vue-package-test-x/HelloA'
import HelloB from 'vue-package-test-x/HelloB'
```
