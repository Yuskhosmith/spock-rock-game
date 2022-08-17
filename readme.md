# Rock Paper Scissors Lizard Spock
Enjoy the Explanation from [Sheldon himself](https://www.youtube.com/watch?v=405Nh2H4Ucg){:target="_blank"}. But here it is
| Name | Defeats |
| ----- | ----- |
| Rock | Scissors, Lizard |
| Paper | Rock, Spock |
| Scissors | Paper, Lizard |
| Lizard | Paper, Spock |
| Spock | Scissors, Rock |

## .New 🚀
ES6 Modules - Bundles - Tree Shaking
So, just like modules in every other language but with specificity and an export statement for tree shaking (filtering out things you don't need).

You'll need to add the attribute `type="module"` to your script tag in your HTML file.
```html
<script src="script.js" type="module"></script>
```
At the end of the module, you'll have an export statement like this.
```js
  export { startConfetti, stopConfetti, removeConfetti };
```

At the top of your main JS file, your import statement will look like this
```js
import { startConfetti, stopConfetti, removeConfetti } from "./confetti.js";
```

And you can also do dynamic loading, whereby you load your js module only when you need it.
```js
import('./modules/myModule.js')
  .then((module) => {
    // Do something with the module.
  });
```
Read more about JS Modules [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#dynamic_module_loading)