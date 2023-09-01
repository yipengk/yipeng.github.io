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
  <img width="200px" src="miro.medium.com/v2/resize:fit:1400/1*LyZcwuLWv2FArOumCxobpA.png" >
</div>

This is the first WOD homework I completed in ICS314. This question comes from CTIT, which is called "isUnique." This WOD requires us to determine whether a string contains all unique characters, that is, whether each character in the string only appears once.

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
