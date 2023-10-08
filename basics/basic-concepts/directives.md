## Vue Directives Details

Directives are used to modify the behavior of our HTML elements which reside in the DOM. In other words, we can say that directives are one of the important parts of the Vue and it is used just like an HTML element’s attribute added along with any HTML elements into the Vue template.

### 1. `v-bind`

**Usage**: Binds an attribute to an expression.

**Example**:
```html
<!-- binds the 'href' attribute to the 'url' data property -->
<a v-bind:href="url">Link</a>
```

### 2. `v-if`, `v-else-if`, `v-else`

**Usage**: Conditional rendering of elements.

**Example**:
```html
<p v-if="seen">Now you see me</p>
<p v-else-if="someOtherCondition">Now you see something else</p>
<p v-else>Now you don't</p>
```

### 3. `v-show`

**Usage**: Toggles visibility of an element (using the CSS display property).

**Example**:
```html
<p v-show="isVisible">Toggle visibility</p>
```

### 4. `v-for`

**Usage**: Renders a list by iterating over an array.

**Example**:
```html
<ul>
  <li v-for="item in items">{{ item.text }}</li>
</ul>
```

### 5. `v-on`

**Usage**: Attaches event listeners to elements.

**Example**:
```html
<button v-on:click="doSomething">Click me!</button>
```
You can also use event modifiers with `v-on`, like `.prevent` to call `event.preventDefault()` or `.stop` to call `event.stopPropagation()`:
```html
<form v-on:submit.prevent="onSubmit">...</form>
```

### 6. `v-model`

**Usage**: Creates a two-way binding on an `input`, `textarea`, or `select` element.

**Example**:
```html
<input v-model="message">
```
With this, the value of the `input` will bind to the `message` data property, and when the input changes, the `message` will update to reflect those changes.

---


