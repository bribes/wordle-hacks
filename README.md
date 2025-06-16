# Wordle Hacks (WORKING 2025)
Many hacks and cheats for the popular game Wordle. **(Don't use this if you want to actually have fun)**

## 3 ways to execute the scripts:

#### #1 Make a bookmark with `javascript:` then the code as the URL.

#### #2 Type `javascript:` then the code into the URL box and press ENTER.

#### #3 Go into Inspect Element (Ctrl + Shift + I) then go into the console then paste the script in.

## Get the word of the day (WARNING: This is a fun ruiner)
This is possible since the have a list of all the coming words in the source code which is easily accessible via right clicking and pressing "View Page Source" then going the the .js file (Ex. main.92j9aw.js) running the site and also is accessible via JavaScript.

![image](https://user-images.githubusercontent.com/52789876/152241083-64712717-0555-4f04-b1cd-4581bf8dfdc1.png)

The Code:
```javascript
/*made by github.com/bribes*/const fetchWordle=async e=>{const t=await fetch(`https://www.nytimes.com/svc/wordle/v2/${e}.json`);return(await t.json()).solution},showWordles=async()=>{const e=(new Date).toISOString().split("T")[0],t=new Date(Date.now()-864e5).toISOString().split("T")[0],o=new Date(Date.now()+864e5).toISOString().split("T")[0];try{const[r,s,n]=await Promise.all([fetchWordle(e),fetchWordle(t),fetchWordle(o)]);alert(`Wordle Answers:\nYesterday: ${s.toUpperCase()}\nToday: ${r.toUpperCase()}\nTomorrow: ${n.toUpperCase()}`)}catch(e){console.error("Error fetching Wordle answers:",e)}};showWordles()/*made by github.com/bribes*/
```

# WARNING! All the scripts below here will stay even when you refresh
The only way to remove any trace of manipulating the code is to reset either the board, stats or even both, so be warned.

The scripts below are mostly harmless.

# Edit the Board
For this script everything except letters will be removed from what you input. This is made possible since the board state is stored in Local Storage which is easily accessible with JavaScript and also Inspect Element (Ctrl + Shift + I).

![image](https://user-images.githubusercontent.com/52789876/152076636-9e6e12fc-fb74-4a7d-8917-e4e14932556c.png)

The Code:
```javascript
/* made by github.com/bribes */const fetchWordle=async t=>{const e=await fetch(`https://www.nytimes.com/svc/wordle/v2/${t}.json`);return(await e.json()).id};var today=(new Date).toISOString().split("T")[0],ghbribes=prompt(atob("RW50ZXIgdGV4dA=="),"github.com/bribes");function bribes(t,e,r){return e>t.length?t.concat(Array(e-t.length).fill(r)):t}var wordedit=bribes(ghbribes.replace(/[^A-Za-z]/g,"").match(/.{1,5}/g).splice(0,6),6,"");localStorage["games-state-wordleV2/ANON"]=`{"states":[{"data":{"boardState":${JSON.stringify(wordedit)},"currentRowIndex":${wordedit.filter((t=>t)).length},"status":"${wordedit.filter((t=>t)).length===6?'WIN':'IN_PROGRESS'}"},"puzzleId":"${await fetchWordle(today)}"}]}`,location.reload()/* made by github.com/bribes */
```

Resetting the Board:
```javascript
localStorage['games-state-wordleV2/ANON']=""
```

Create a [issue](https://github.com/bribes/wordle-hacks/issues) if you're having problems with the scripts.
