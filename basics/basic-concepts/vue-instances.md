In Vue.js, an instance is essentially an object that ties together the data, template, and logic necessary to power a Vue application or component. It serves as the root of a Vue app and provides the context in which Vue's reactive data-binding system operates. 

When you create a new Vue instance using `new Vue()`, you're creating an isolated, reusable component. This instance has its own data, methods, lifecycle hooks, and so on. The most basic form of a Vue instance looks like this:

```javascript
var vm = new Vue({
  el: '#app',           // element to mount to
  data: {
    message: 'Hello Vue!'
  }
});
```

Here's a breakdown of the properties:

- `el`: Specifies a DOM element to mount the Vue instance. In this case, Vue will look for an element with the ID of "app" and mount itself there.

- `data`: An object that holds the data for the Vue instance. This is where you define properties that you want to be reactive.

Once you have a Vue instance, you can access its properties and methods using the variable you assigned it to. In the example above, that's the `vm` variable.

```javascript
console.log(vm.message); // logs "Hello Vue!"
```

The Vue instance also exposes several lifecycle hooks, like `created`, `mounted`, `updated`, and `destroyed`, which you can use to run code at specific stages in the component's life.

A Vue application typically starts by creating a root Vue instance with `new Vue()`, which mounts to a DOM element and encompasses the whole app. From there, you can create reusable Vue components, each of which can also be thought of as smaller Vue instances with their own state, methods, and lifecycle.

In essence, the Vue instance serves as the foundation of how Vue's reactive system works, linking the data model to the DOM and allowing for data-driven UI updates.
