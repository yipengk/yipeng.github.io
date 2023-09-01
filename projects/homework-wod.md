---
layout: project
type: project
image: miro.medium.com/v2/resize:fit:1400/1*LyZcwuLWv2FArOumCxobpA.png
title: "Homework WOD"
date: 2023-08-31
published: true
labels:
  - Software engineering
  - Javascript
  - Technology
summary: "My first homework WOD in ICS314."
---

  <div class="text-center p-4">
  <img width="200px" src="https://miro.medium.com/v2/resize:fit:1400/1*LyZcwuLWv2FArOumCxobpA.png" class="img-thumbnail" >
 
</div>

This is the first WOD homework I completed in ICS314. This question comes from CTIT, which is called "isUnique." This WOD requires us to determine whether a string contains all unique characters, that is, whether each character in the string only appears once. When I got this wod, my original idea was to do two loops to compare, and if there's the same character, it's definitely not unique. My code is as follows:

```javascript
function isUnique(str){
    for(let i=0;i<str.length;i++){
        for(let j=i+1;j<str.length;j++){
            if(str[i]===str[j]){
                return false;
            }
        }
    }
    return true;
}

let str='apple';
console.log(isUnique(str));
```
Even though my original idea is simple, it is not good because it is inefficient, and its time complexity is O(n^2), which means that as the input string increases, the required time grows quadratically. So, I watched the instructor's solution.Below is the instructor's solution: 

```javascript
function isUnique(str){
    let chars={};
    for(let i=0;i<str.length;i++){
        if(chars[str[i]]){
            return false;
        }
        chars[str[i]]=true;
    }
    return true;
}
let str='apple';
console.log(isUnique(str));
```
He uses objects to track characters that have already appeared in the string, and the time complexity is O(n), which is much more efficient. I think in the future. I should think more about the question from all aspects before solving it because solving it is not enough. How to solve the question more efficiently is what we should work on.
