# Wordle Hacks (FIXED FOR NY TIMES UPDATE)
Many hacks, exploits and cheats for the popular game Wordle. **(Don't use this if you want to actually have fun)**

The code is a lot less complicated then it looks its just that I obfuscated to stop people from stealing the code and using it as theirs you can use a deobfuscator to try to understand the code.

PS. All the people "Leaking" the Word List all they are doing is right clicking pressing "View Page Source" going to the .js file (Ex. main.92j9aw.js) used to run the site and finding (Ctrl + F) the current word for example "Ultra" and then itll show a Array of all the other words that are next, they are not "hackers" just glorified script kiddies. What I do here isn't too complicated and if you took the time to understand JavaScript it would look super basic.

## 3 ways to execute the scripts:

#### #1 Make a bookmark with `javascript:` then the code as the URL.

#### #2 Type `javascript:` then the code into the URL box and press ENTER.

#### #3 Go into Inspect Element (Ctrl + Shift + I) then go into the console then paste the script in.

## Get the word of the day (WARNING: This is a fun ruiner)
This is possible since the have a list of all the coming words in the source code which is easily accessible via right clicking and pressing "View Page Source" then going the the .js file (Ex. main.92j9aw.js) running the site and also is accessible via JavaScript.

![image](https://user-images.githubusercontent.com/52789876/152241083-64712717-0555-4f04-b1cd-4581bf8dfdc1.png)

The Code:
```javascript
/*made by github.com/bribes*/fetch(atob('aHR0cHM6Ly93d3cubnl0aW1lcy5jb20vZ2FtZXMvd29yZGxlL21haW4u')+wordle.hash.replace('made by bribes','github.com/bribes')+'.js').then(bybribes=>bybribes.text()).then(async madebybribes=>{/*get word list*/function capitalize(string){/*made by github.com/bribes*/return string.charAt(0).toUpperCase()/*made by github.com/bribes*/+/*made by github.com/bribes*/string.slice(1);}var date=new Date().toLocaleDateString();/*made by github.com/bribes*/var yesterdayDate=new Date(new Date().getTime()-24*60*60*1000).toLocaleDateString();/*made by github.com/bribes*/var tommorowDate=new Date(new Date().getTime()+24*60*60*1000).toLocaleDateString();var ghbribes=await madebybribes.split('Ma=')[1].split(',Oa=')[0].replace(/[\[\]']+/g,'').replace(/"/g,'').split(',');/*made by github.com/bribes*/function bribes(start,end){const date1=new Date(start);const date2=new Date(end);const oneDay=1000*60*60*24;const diffInTime=date2.getTime()-date1.getTime();const diffInDays=Math.round(diffInTime/oneDay);/*made by github.com/bribes*/return diffInDays;/*made by github.com/bribes*/}alert(`${yesterdayDate} | Yesterday's Solution: ${capitalize(ghbribes[bribes(atob('Ni8xOS8yMQ=='),yesterdayDate)])}\n${date} | Today's Solution: ${capitalize(JSON.parse(localStorage['nyt-wordle-state']).solution)}\n${tommorowDate} | Tommorow's Solution: ${capitalize(ghbribes[bribes(atob('Ni8xOS8yMQ=='),tommorowDate)])}`);/*made by github.com/bribes*/console.log(atob('d29yZGxlIHdvcmQgcmV2ZWFsZWQhIC0gZmFhdg=='))});/*made by github.com/bribes*/
```

# WARNING! All the scripts below here will stay even when you refresh
The only way to remove any trace of manipulating the code is to reset either the board, stats or even both, so be warned.

The scripts below are mostly harmless.

# Edit the Board
For this script everything except letters will be removed from what you input. This is made possible since the board state is stored in Local Storage which is easily accessible with JavaScript and also Inspect Element (Ctrl + Shift + I).

![image](https://user-images.githubusercontent.com/52789876/152076636-9e6e12fc-fb74-4a7d-8917-e4e14932556c.png)

The Code:
```javascript
/* made by github.com/bribes */ var ghbribes=prompt(atob("RW50ZXIgdGV4dA=="),"github.com/bribes"); /* made by github.com/bribes */ function bribes(array,length,fill){return length>array.length?array.concat(Array(length-array.length).fill(fill)):array;}var wordedit=JSON.stringify(bribes(ghbribes.replace(/[^A-Za-z]/g,'').match(/.{1,5}/g).splice(0,6), 6, "")); /* made by github.com/bribes */ localStorage['nyt-wordle-state']=`{"boardState":${wordedit},"evaluations":[["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"],["correct","correct","correct","correct","correct"]],"rowIndex":1,"solution":"${JSON.parse(localStorage['nyt-wordle-state']).solution}","gameStatus":"WIN","lastPlayedTs":${new Date().valueOf()},"lastCompletedTs":${new Date().valueOf()},"restoringFromLocalStorage":true,"hardMode":true}`;window.location.href=window.location.href /* made by github.com/bribes */
```

Resetting the Board:
```javascript
localStorage['nyt-wordle-state']=""
```

# Edit your Stats
This is made possible since your statistics are stored in Local Storage which is easily accessible with JavaScript and also Inspect Element (Ctrl + Shift + I).

![image](https://user-images.githubusercontent.com/52789876/152078900-12554a7e-d984-4099-842f-e31ade010e1f.png)

The Code:
```javascript
/* made by github.com/bribes */ var ghbribes1=prompt(atob("UGxheWVk"),"github.com/bribes"); /* made by github.com/bribes */ var ghbribes2=prompt(atob("V2luICU="),"github.com/bribes") /* made by github.com/bribes */ ;var ghbribes3=prompt(atob("Q3VycmVudCBTdHJlYWs="),"github.com/bribes"); /* made by github.com/bribes */ var ghbribes4=prompt(atob("TWF4IFN0cmVhaw=="),"github.com/bribes"); /* made by github.com/bribes */ localStorage['nyt-wordle-statistics']=`{"currentStreak":"${ghbribes3}","maxStreak":"${ghbribes4}","guesses":{"1":69420,"5":0,"3":0,"4":0,"5":0,"6":0,"fail":0},"winPercentage":"${ghbribes2}","gamesPlayed":"${ghbribes1}","gamesWon":100,"averageGuesses":100}`;window.location.href=window.location.href; /* made by github.com/bribes */
```

Resetting your Stats:
```javascript
localStorage['nyt-wordle-statistics']=""
```

Create a [issue](https://github.com/bribes/wordle-hacks/issues) if you're having problems with the scripts.
