# components-example

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


To create a component you first need to create a file, go to the component's directory and create a file with a .vue extension (remember to always use best practice naming).
After that, you go to the file you want to import, import the component and reference it on the component property of the export default, then you just need to place it on your page e.g. "<yourComponent></yourComponent>"

You might also use components that are rendered once in a while. In a large scale project, it will be a long wait until all your components load, so you can load then asynchronously, to do that, remove your component's import of the page, and in you components property, pass a function as the value of the component importing it using the method import(). You can see an example in my HelloWorld.vue component.  