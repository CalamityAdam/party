```js
javascript:(function() {[].forEach.call(document.querySelectorAll('a, button, input, details'), el => {el.addEventListener('mouseover', (event) => {event.currentTarget.style.transform = `translate3d(${Math.round(Math.random()) ? '-' : ''}${Math.floor(Math.random() * 201)}px, ${Math.round(Math.random()) ? '-' : ''}${Math.floor(Math.random() * 201)}px, ${Math.round(Math.random()) ? '-' : ''}${Math.floor(Math.random() * 201)}px)`;});el.style.transition = '.2s cubic-bezier(.3,0,.5,1)';el.style.position = 'relative';el.style.zIndex = '100000000';el.style.transitionProperty = 'transform';if(el.localName === 'a') {el.style.display = 'inline-block';}});})();

```
