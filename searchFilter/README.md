# 🍎 Fruits Filter - Real-Time Search Demo

A **super simple** real-time search filter built with **HTML**, **CSS**, and **pure JavaScript**. Perfect for beginners to understand **live search functionality**!

## ✨ **Live Demo**
Just save as HTML and open in browser - works instantly!

## 🎮 **Features**
- ✨ **Real-time search** - Type to filter fruits instantly
- 🍎 **6 colorful fruits** with emojis
- 🔍 **Searches entire text** (name + description)
- 📱 **Mobile responsive**
- 🎨 **Smooth hover animations**
- 👶 **Beginner-friendly code** - 25 lines total!

## 🚀 **How It Works (10 Steps)**

1. Page Loads
text
HTML creates 6 fruit boxes + 1 search input
JavaScript finds them: searchBox, fruitItems[6]
Everything visible initially
2. User Types First Letter
text
Type "a" → searchBox.value = "a"
addEventListener('input') triggers instantly
3. Get Search Word
javascript
let searchWord = searchBox.value.toLowerCase();
searchWord = "a"  // All lowercase for easy matching
4. Loop Through ALL Fruits (forEach)
text
forEach visits each fruit 1 by 1:
🍎 Apple → Check it
🍌 Banana → Check it  
🍊 Orange → Check it
... (6 times total)
5. Get Fruit Text
javascript
let fruitText = fruit.textContent.toLowerCase();
🍎 Apple → fruitText = "apple - red fruit, good for health"
6. MAGIC MATCH Check
javascript
if (fruitText.includes(searchWord))
"apple - red fruit".includes("a") → TRUE ✅
"banana - yellow".includes("a") → TRUE ✅  
"orange - citrus".includes("a") → TRUE ✅
7. SHOW Matching Fruit
javascript
fruit.classList.remove("hidden");
✅ Matching fruit → Remove invisible class → VISIBLE!
8. HIDE Non-Matching Fruit
javascript
fruit.classList.add("hidden");
❌ No match → Add invisible class → INVISIBLE!
9. Repeat for All 6 Fruits
text
6 fruits checked → 3 shown + 3 hidden
Page updates instantly (no page reload!)
10. User Types Next Letter
text
Type "ap" → Repeat steps 3-9 instantly
Now only 🍎 Apple shows (has "ap")
Others hidden (no "ap")


