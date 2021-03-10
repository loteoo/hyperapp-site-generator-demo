# Getting started


## Starter template 🚀

To easiest way to get started is to use this [starter template](https://github.com/loteoo/hyperstatic-starter).

---  

## Installation in an existing hyperapp project  

#### Prerequisite

Your environment (browser or bundling setup) needs to support [dynamic imports](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import#dynamic_imports).

#### Steps

1. `npm i hyperstatic`

2. Create a `routes` object with your routes patterns in it.   
[Example](https://github.com/loteoo/hyperstatic-starter/blob/master/src/main.tsx#L8-L15)

3. Replace hyperapp's `app` call with `hyperstatic`. Add the extra `routes` attribute that is needed.   
[Example](https://github.com/loteoo/hyperstatic-starter/blob/master/src/main.tsx#L24)  


4. Add the hyperstatic `Router` component that will render the pages   
[Example](https://github.com/loteoo/hyperstatic-starter/blob/master/src/components/core/App/index.tsx#L11)  

5. Link to your pages using the `Link` component.   
[Example](https://github.com/loteoo/hyperstatic-starter/blob/master/src/components/core/Header/index.tsx#L11)

6. For prerendering, add this helper command in your package.json scripts:  

```
"scripts": {
  "prerender": "npm run build && hyperstatic"
}
```
