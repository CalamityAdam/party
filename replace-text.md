```js
javascript:(function replace_text(){const repObj = {Dev: "Butt", Release: "Poop", Pro: "Booger", Underway: "Underwear", Blocked: "Constipated", Done: "Dung", Issues: "Tissues"}; document.body.innerHTML = document.body.innerHTML.replace(/Dev|Release|Pro|Underway|Blocked|Done|Issues/g, function(matched) {return repObj [matched]});})();
```
