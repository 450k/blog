---
title: "Astroのテーマ「Citrus」を試してみた"
description: "Astroの無料テーマcitrusの使い勝手を検証"
publishDate: "19 Aug 2025"
updatedDate: "19 Aug 2025"
tags: ["Astro", "theme"]
---

## スタティック・サイト・ジェネレータ Astro の無料テーマ Citrus

今回はAstroの無料テーマcitrusを使ってblogサイトを構築します。

### ステップは以下の通り 
- ターミナルからサイトデータを格納するディレクトリへ移動 
- インストールコマンドを入力  
- ローカルサーバーを起動し表示確認 
- GitHub Pages　へコミット

### インストールコマンド

**インストール用のコマンドは以下の通り**
```npm command title="# npm 7+"
npm create astro@latest -- --template artemkutsan/astro-citrus
```  
*I often help with recursion—classic stuff!*  

**JavaScript: Countdown Timer**
```js title="countdown-timer.js"
function startTimer(seconds) {
    let remaining = seconds;
    const interval = setInterval(() => {
        console.log(`Time left: ${remaining} sec.`);
        remaining--;
        if (remaining < 0) {
            clearInterval(interval);
            console.log("Time's up! ⏰");
        }
    }, 1000);
}

startTimer(5); // Starts a 5-second timer
```  
*Async logic? My jam.*  

**SQL: Finding Active Users**
```sql
SELECT users.name, COUNT(orders.id) AS total_orders
FROM users
LEFT JOIN orders ON users.id = orders.user_id
GROUP BY users.name
HAVING total_orders > 3;
```  
*I love structured data and elegant JOINs!*  

#### Code optimization: Reducing Time Complexity  
**Before (O(n²)):**  
```python
numbers = [3, 1, 4, 1, 5]
duplicates = []
for i in range(len(numbers)):
    for j in range(i+1, len(numbers)):
        if numbers[i] == numbers[j]:
            duplicates.append(numbers[i])
```  

**After (O(n)):**  
```python
from collections import defaultdict

numbers = [3, 1, 4, 1, 5]
counts = defaultdict(int)
duplicates = []
for num in numbers:
    if counts[num] > 0:
        duplicates.append(num)
    counts[num] += 1
```  
*Optimizing code is pure magic!*  

### How I Can Help You
- **Explain confusing code** from your project.  
- **Fix memory leaks** in your C++ app.  
- **Choose the right algorithm** for sorting tasks.  
- **Write tests** using pytest or Jest.  
- **Debug "undefined is not a function"** in JS.  

### Favorite Topics
- Machine Learning (PyTorch examples? Sure!).  
- Web Development (Django, React, Flask).  
- Algorithms & Data Structures (graphs, trees, hash tables).  
- Automation with Python (scraping, bots).  

### Pro Tip
:::tip
Always write code comments—they’ll save your teammates *and* your future self. And yes, `console.log` is a temporary fix; tests are better!  
:::

**Ready to tackle your code! Just ask. 😊**