# Party Time!
[![Generic badge](https://img.shields.io/badge/Version-2.0.1-blue.svg)](https://shields.io/)

[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/Naereen/)
[![ForTheBadge makes-people-smile](http://ForTheBadge.com/images/badges/makes-people-smile.svg)](http://ForTheBadge.com)

## Instructions
1. Bookmark this page
1. Right click the newly created bookmark
1. Click "Edit" (if on Firefox, click "Properties")
1. Rename the bookmark to "party time!" (or, something fun and silly)
1. Copy and Paste the following code into the "URL" section of the bookmark (or "Location" or "Address" depending on the browser)
    ```
    javascript:(function(){function a(){this.randomModifier=rand(-1,1),this.colorPair=m[Math.floor(rand(0,m.length))],this.dimensions={x:rand(l.size.x[0],l.size.x[1]),y:rand(l.size.y[0],l.size.y[1])},this.position={x:h[0],y:h[1]},this.rotation=rand(0,2*Math.PI),this.scale={x:1,y:1},this.velocity={x:.4*rand(-l.initSpeed,l.initSpeed),y:rand(-l.initSpeed,l.initSpeed)},this.flipSpeed=rand(.2,1.5)*l.flipSpeed,this.position.y<=g.h&&(this.velocity.y=-Math.abs(this.velocity.y)),this.terminalVelocity=rand(1,1.5)*l.terminalVelocity,this.update=function(){this.velocity.x*=.98,this.position.x+=this.velocity.x,this.velocity.y+=this.randomModifier*l.drag,this.velocity.y+=l.gravity,this.velocity.y=Math.min(this.velocity.y,this.terminalVelocity),this.position.y+=this.velocity.y,this.scale.y=Math.cos((this.position.y+this.randomModifier)*this.flipSpeed),this.color=0<this.scale.y?this.colorPair.front:this.colorPair.back}}function b(){j.clearRect(0,0,g.w,g.h),k.forEach(function(a){a.update(),j.translate(a.position.x,a.position.y),j.rotate(a.rotation);var b=a.dimensions.x*a.scale.x,c=a.dimensions.y*a.scale.y;j.fillStyle=a.color,j.fillRect(-.5*b,-.5*c,b,c),j.setTransform(1,0,0,1,0,0)}),k.forEach(function(a,b){(a.position.y>g.h||a.position.x<-.5*g.x||a.position.x>1.5*g.x)&&k.splice(b,1)}),window.requestAnimationFrame(b)}function c(){g={w:f.clientWidth,h:f.clientHeight},f.width=g.w,f.height=g.h}function d(b){var c=f.getBoundingClientRect();h=b?[b.clientX-c.left,b.clientY-c.top]:[c.width*Math.random(),c.height*Math.random()];for(var d=0;d<l.number;d++)k.push(new a)}function e(){k=[],window.cancelAnimationFrame(b)}var f=document.createElement("canvas");f.id="confetti",f.class="confetti",f.style.width="100%",f.style.height="100vh",f.style.position="fixed",f.style.zIndex="99999",document.body.insertBefore(f,document.body.firstElementChild);var g,h,j=f.getContext("2d"),k=[];rand=function(a,b){return Math.random()*(b-a)+a};var l={number:70,size:{x:[5,20],y:[10,18]},initSpeed:25,gravity:.65,drag:.08,terminalVelocity:6,flipSpeed:.017},m=[{front:"#3B870A",back:"#235106"},{front:"#B96300",back:"#6f3b00"},{front:"#E23D34",back:"#88251f"},{front:"#CD3168",back:"#7b1d3e"},{front:"#664E8B",back:"#3d2f53"},{front:"#394F78",back:"#222f48"},{front:"#008A8A",back:"#005353"}];c(),b(),f.addEventListener("click",d),window.addEventListener("resize",function(){c(),e()})})();
    ```
1. Click "party time!" bookmark
1. Click anywhere on your screen and party! 🎉

![party time!](https://media.giphy.com/media/9G5bX9nXYfmmatgn0B/giphy.gif)

![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Firefox](https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![IE](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![Opera](https://raw.githubusercontent.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | ![Safari](https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
Latest ✔ | Latest ✔ | 10+ ✔ | Latest ✔ | ❌ |

# Frequently Asked Questions

- [How do I de-confetti the clicker?](#how-do-i-de-confetti-the-clicker)
- [When should I use this?](#when-should-i-use-this)

## How do I de-confetti the clicker?
*Why would you want to do that?*

1. Refresh the page

## When should I use this?

1. Use this tool when you are sad and want to cheer up.
1. Use it when you want to celebrate an accomplishment.
1. ~~Use it when you want to prank a teammate and put it on their computer while they're away from their desk and didn't lock the computer.~~
1. Use it for fun any time of day!


# Want more amusing fun?
Open any of these files, copy the script in that file, follow the same instructions as listed above ☝️ but use the copied script instead of the script listed here.

- [Button Chaos](button-chaos.md) thanks [Josh Friend](https://github.com/joshwhatk)
- [Blur Screen](blur-screen.md)
- [Broken Screen](broken-screen.md) Trick your friends into thinking they broke your screen!
- [Replace Text (kindergarten edition)](replace-text.md) thanks [Isaiah Colson](https://github.com/isaiahcolson)

---
### Like this tool? [Let me know!](mailto:sisk@hey.com?subject=Hey%20I%20really%20like%20party%20time!)
### Have a great idea for another fun prank? [Let me know!](mailto:sisk@hey.com?subject=Hey%20I%20have%20an%20idea%20for%20a%20fun%20prank!)
---


> made with ♥️ by Adam Sisk
