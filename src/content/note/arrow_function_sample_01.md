---
title: タイトル
description: ディスクリプション
publishDate: "2025-08-17T19:00:00+09:00"
---

## arrow functionの書き方

Arrow function syntax may look strange but it's actually simple.

1. function callMe(name) { 
2.     console.log(name);
3. }

which you could also write as:

1. const callMe = function(name) { 
2.     console.log(name);
3. }

becomes: 

1. const callMe = (name) => { 
2.     console.log(name);

**Important:** 

When having **no arguments**, you have to use empty parentheses in the function declaration:

1. const callMe = () => { 
2.     console.log('Max!');
3. }

When having **exactly one argument**, you may omit the parentheses:

1. const callMe = name => { 
2.     console.log(name);
3. }

When **just returning a value**, you can use the following shortcut:

1. const returnMe = name => name

That's equal to:

1. const returnMe = name => { 
2.     return name;
3. }