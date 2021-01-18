# just4fun - JavaScript
### some senseless coding stuff
by Moritz Petzka<br>
[petzka.com](https://petzka.com)<br>
info@petzka.com<br>
<br>

## Browser Console Scripts
open any website and copy and paste one of the following scripts to the javascript development console* of your browser and enjoy...

(* to open the console press 12)

#### all div elements shaking and moving:
```javascript
var r =()=>{return Math.random()*2-1;},mE=(e,a,b,c)=>{a=a+r();b=b+r();c=c+r()/1000;e.style.transform='translate('+a+'px ,'+b+'px) scale('+c+')';setTimeout(()=>{mE(e, a , b, c);},1000/24);},sE=(t)=>{var e=document.getElementsByTagName(t);for(var i=0;i<e.length;i++){mE(e[i],0,0,1);};};sE('div');
```

#### random colors for all div elements:
```javascript
var rc=()=>{return 'hsla('+(Math.random()*360)+',100%,50%,'+Math.random() + ')';},cre=(e, t)=>{e.style.backgroundColor=rc();e.style.color=rc();setTimeout(()=>{cre(e)},Math.random()*1000+150);},cE=(t)=>{var e=document.getElementsByTagName(t);for(var i=0;i<e.length;i++){cre(e[i]);};};cE('div');
```

