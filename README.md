# :100: sebact

My own React (heavily inspired by [Didact](https://engineering.hexacta.com/didact-learning-how-react-works-by-building-it-from-scratch-51007984e5c5))

## Elements

Describes what needs to be rendered and have two required properties: `type` and `props`

```javascript
const myElement = {
  type: 'div',
  props: {
    id: 'container',
    children: [
      { type: 'input', props: { value: 'foo', type: 'text' } },
      { type: 'a', props: { href: '/bar' } },
      { type: 'span', props: {} }
    ]
  }
};
```

Which is translated to the DOM in the following way:

```html
<div id="container">
  <input value="foo" type="text" />
  <a href="/bar" />
  <span></span>
</div>
```
