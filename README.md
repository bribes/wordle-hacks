# Wordle Hacks
Many hacks, exploits and cheats for the popular game Wordle. **(Don't use this if you wanna have fun)**

## Ways to execute the script:

### Make a bookmark type `javascript:` then the code.

### Go into Inspect Element then go into the console then paste the script in.

## Get the word of the day

The Script:
```javascript
/* made by github.com/bribes */ fetch(atob('aHR0cHM6Ly93d3cucG93ZXJsYW5ndWFnZS5jby51ay93b3JkbGUvbWFpbi4=')+parent.window.wordle.hash.replace('made by bribes','github.com/bribes')+'.js').then(bybribes => bybribes.text()).then(async madebybribes =>{var ghbribes=await madebybribes.split('La=')[1].split(',Ta=')[0].replace(/[\[\]']+/g,'').replace(/'/g, '').split(','); /* made by github.com/bribes */ function bribes(start,end){const date1=new Date(start);const date2=new Date(end);const oneDay=1000*60*60*24;const diffInTime=date2.getTime()-date1.getTime();const diffInDays = Math.round(diffInTime / oneDay);/* made by github.com/bribes */return diffInDays; /* made by github.com/bribes */ }alert(atob('VG9kYXkncyB3b3JkIGlzLCA=')+ghbribes[bribes(atob('Ni8yMC8yMDIx'),new Date())]+'!'); /* made by github.com/bribes */ console.log(atob('d29yZGxlIHdvcmQgcmV2ZWFsZWQhIC0gZmFhdg=='));
}); /* made by github.com/bribes */
```

# WARNING! All the scripts below here will stay even when you refresh
The only way to remove any trace of manipulating the code is to reset all your stats, so be warned.

The scripts here are mostly harmless.

## Resetting Stats

The Script:

```javascript
localStorage.gameState="";localStorage.statistics=""
```

# Edit the board
For this script everything except letters will be removed from what you input.

![image](https://user-images.githubusercontent.com/52789876/152076636-9e6e12fc-fb74-4a7d-8917-e4e14932556c.png)

The Script:
```javascript
/* made by github.com/bribes */ var ghbribes=prompt(atob("RW50ZXIgdGV4dA=="),"github.com/bribes"); /* made by github.com/bribes */ function bribes(array,length,fill){return length>array.length?array.concat(Array(length-array.length).fill(fill)):array;}var wordedit=JSON.stringify(bribes(ghbribes.replace(/[^A-Za-z]/g,'').match(/.{1,5}/g).splice(0,6), 6, "")); /* made by github.com/bribes */ localStorage.gameState=`{"boardState":${wordedit},"evaluations":[["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"]],"rowIndex":1,"solution":"github.com/bribes","gameStatus":"WIN","lastPlayedTs":${new Date().valueOf()},"lastCompletedTs":${new Date().valueOf()},"restoringFromLocalStorage":true,"hardMode":true}`;window.location.href=window.location.href /* made by github.com/bribes */
```

# Edit yours stats

![image](https://user-images.githubusercontent.com/52789876/152078900-12554a7e-d984-4099-842f-e31ade010e1f.png)

The Script:
```javascript
/* made by github.com/bribes */ var ghbribes1=prompt(atob("UGxheWVk"),"github.com/bribes"); /* made by github.com/bribes */ var ghbribes2=prompt(atob("V2luICU="),"github.com/bribes") /* made by github.com/bribes */ ;var ghbribes3=prompt(atob("Q3VycmVudCBTdHJlYWs="),"github.com/bribes"); /* made by github.com/bribes */ var ghbribes4=prompt(atob("TWF4IFN0cmVhaw=="),"github.com/bribes"); /* made by github.com/bribes */ localStorage.statistics=`{"currentStreak":"${ghbribes3}","maxStreak":"${ghbribes4}","guesses":{"1":69420,"5":0,"3":0,"4":0,"5":0,"6":0,"fail":0},"winPercentage":"${ghbribes2}","gamesPlayed":"${ghbribes1}","gamesWon":100,"averageGuesses":100}`;window.location.href=window.location.href; /* made by github.com/bribes */
```

Create a issue if you're having a problem with the scripts.
