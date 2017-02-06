# custom-snippets
> Custom snippets for the web.

## [cel] CustomElement

```js
class ${2:MyElement} extends ${3:HTMLElement} {
  static get is() {
    return '${1:my-element}';
  }
  // attributes to observe
  static get observedAttributes() {
    return [];
  }
  constructor() {
    super();
    this.root = this.attachShadow({mode: 'open'});
    $0
  }
  attributeChangedCallback(name, oldVal, newVal) {
    console.log(name, oldVal, newVal);
  }
}
customElements.define(${2:MyElement}.is, ${2:MyElement})
```

## [gtask] gulp task

```js
${2:gulp.}task($1, () => {
  $0
});
```
