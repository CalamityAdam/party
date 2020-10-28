1. Bookmark this page
2. right click the newly created bookmark
3. click "Edit"
4. paste the following code into the URL and rename the bookmark to "party time!"
```
javascript:(function(){const confetti=document.createElement("canvas");confetti.id="confetti",confetti.class="confetti",confetti.style.width="100%",confetti.style.height="100vh",confetti.style.position="fixed",confetti.style.zIndex="99999",document.body.insertBefore(confetti,document.body.firstElementChild);const confettiCtx=confetti.getContext("2d");let container,clickPosition,confettiElements=[];rand=((t,i)=>Math.random()*(i-t)+t);const confettiParams={number:70,size:{x:[5,20],y:[10,18]},initSpeed:25,gravity:.65,drag:.08,terminalVelocity:6,flipSpeed:.017},colors=[{front:"#3B870A",back:"#235106"},{front:"#B96300",back:"#6f3b00"},{front:"#E23D34",back:"#88251f"},{front:"#CD3168",back:"#7b1d3e"},{front:"#664E8B",back:"#3d2f53"},{front:"#394F78",back:"#222f48"},{front:"#008A8A",back:"#005353"}];function Conf(){this.randomModifier=rand(-1,1),this.colorPair=colors[Math.floor(rand(0,colors.length))],this.dimensions={x:rand(confettiParams.size.x[0],confettiParams.size.x[1]),y:rand(confettiParams.size.y[0],confettiParams.size.y[1])},this.position={x:clickPosition[0],y:clickPosition[1]},this.rotation=rand(0,2*Math.PI),this.scale={x:1,y:1},this.velocity={x:.4*rand(-confettiParams.initSpeed,confettiParams.initSpeed),y:rand(-confettiParams.initSpeed,confettiParams.initSpeed)},this.flipSpeed=rand(.2,1.5)*confettiParams.flipSpeed,this.position.y<=container.h&&(this.velocity.y=-Math.abs(this.velocity.y)),this.terminalVelocity=rand(1,1.5)*confettiParams.terminalVelocity,this.update=function(){this.velocity.x*=.98,this.position.x+=this.velocity.x,this.velocity.y+=this.randomModifier*confettiParams.drag,this.velocity.y+=confettiParams.gravity,this.velocity.y=Math.min(this.velocity.y,this.terminalVelocity),this.position.y+=this.velocity.y,this.scale.y=Math.cos((this.position.y+this.randomModifier)*this.flipSpeed),this.color=this.scale.y>0?this.colorPair.front:this.colorPair.back}}function updateConfetti(){confettiCtx.clearRect(0,0,container.w,container.h),confettiElements.forEach(t=>{t.update(),confettiCtx.translate(t.position.x,t.position.y),confettiCtx.rotate(t.rotation);const i=t.dimensions.x*t.scale.x,e=t.dimensions.y*t.scale.y;confettiCtx.fillStyle=t.color,confettiCtx.fillRect(-.5*i,-.5*e,i,e),confettiCtx.setTransform(1,0,0,1,0,0)}),confettiElements.forEach((t,i)=>{(t.position.y>container.h||t.position.x<-.5*container.x||t.position.x>1.5*container.x)&&confettiElements.splice(i,1)}),window.requestAnimationFrame(updateConfetti)}function setupCanvas(){container={w:confetti.clientWidth,h:confetti.clientHeight},confetti.width=container.w,confetti.height=container.h}function addConfetti(t){const i=confetti.getBoundingClientRect();clickPosition=t?[t.clientX-i.left,t.clientY-i.top]:[i.width*Math.random(),i.height*Math.random()];for(let t=0;t<confettiParams.number;t++)confettiElements.push(new Conf)}function hideConfetti(){confettiElements=[],window.cancelAnimationFrame(updateConfetti)}setupCanvas(),updateConfetti(),confetti.addEventListener("click",addConfetti),window.addEventListener("resize",()=>{setupCanvas(),hideConfetti()});})()

```
5. click "party time!" bookmark
6. click anywhere on your screen and party!
