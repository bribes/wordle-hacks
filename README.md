# Wordle Hacks
Many hacks, exploits and cheats for the popular game Wordle.

## Ways to execute the script:

### Make a bookmark type `javascript:` then the code.

### Go into Inspect Element then go into the console then paste the script in.

## Get the word of the day

The Script:
```javascript
/* made by github.com/bribes */ fetch(atob('aHR0cHM6Ly93d3cucG93ZXJsYW5ndWFnZS5jby51ay93b3JkbGUvbWFpbi4=')+parent.window.wordle.hash.replace('made by bribes','github.com/bribes')+'.js').then(bybribes => bybribes.text()).then(async madebybribes =>{var ghbribes=await madebybribes.split('La=')[1].split(',Ta=')[0].replace(/[\[\]']+/g,'').replace(/'/g, '').split(','); /* made by github.com/bribes */ function bribes(start,end){const date1=new Date(start);const date2=new Date(end);const oneDay=1000*60*60*24;const diffInTime=date2.getTime()-date1.getTime();const diffInDays = Math.round(diffInTime / oneDay);/* made by github.com/bribes */return diffInDays; /* made by github.com/bribes */ }alert(atob('VG9kYXkncyB3b3JkIGlzLCA=')+ghbribes[bribes(atob('Ni8yMC8yMDIx'),new Date())]+'!'); /* made by github.com/bribes */ console.log(atob('d29yZGxlIHdvcmQgcmV2ZWFsZWQhIC0gZmFhdg=='));
}); /* made by github.com/bribes */
```

# Edit the board
For this script everything except letters will be removed from what you input.

![image](https://user-images.githubusercontent.com/52789876/152076636-9e6e12fc-fb74-4a7d-8917-e4e14932556c.png)

The Script:
```javascript
var ghbribes=prompt(atob("RW50ZXIgdGV4dA=="),"github.com/bribes");function padArray(array,length,fill){return length>array.length?array.concat(Array(length-array.length).fill(fill)):array;}var wordedit=JSON.stringify(padArray(ghbribes.match(/.{1,5}/g).splice(0,6), 6, ""));localStorage.gameState=`{"boardState":${wordedit},"evaluations":[["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"]],"rowIndex":1,"solution":"github.com/bribes","gameStatus":"WIN","lastPlayedTs":${new Date().valueOf()},"lastCompletedTs":${new Date().valueOf()},"restoringFromLocalStorage":true,"hardMode":true}`;window.location.href=window.location.href;
```
