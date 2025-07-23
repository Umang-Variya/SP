# SP

This project prints multiple common star (`*`) patterns using JavaScript **without using any built-in string functions** like `.repeat()` or helper methods.

## ✅ Patterns Covered

1. Square
2. Left-Aligned Triangle
3. Right-Aligned Triangle
4. Pyramid
5. Inverted Left-Aligned Triangle
6. Inverted Right-Aligned Triangle
7. Inverted Pyramid
8. Diamond

---

## 📜 Source Code

```javascript
let n = 5;

// 1. Square
console.log("Square:");
for (let i = 0; i < n; i++) {
  let line = '';
  for (let j = 0; j < n; j++) {
    line += '*';
  }
  console.log(line);
}

// 2. Left-Aligned Triangle
console.log("\nLeft-Aligned Triangle:");
for (let i = 1; i <= n; i++) {
  let line = '';
  for (let j = 0; j < i; j++) {
    line += '*';
  }
  console.log(line);
}

// 3. Right-Aligned Triangle
console.log("\nRight-Aligned Triangle:");
for (let i = 1; i <= n; i++) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < i; j++) {
    line += '*';
  }
  console.log(line);
}

// 4. Pyramid
console.log("\nPyramid:");
for (let i = 1; i <= n; i++) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < 2 * i - 1; j++) {
    line += '*';
  }
  console.log(line);
}

// 5. Inverted Left-Aligned Triangle
console.log("\nInverted Left-Aligned Triangle:");
for (let i = n; i >= 1; i--) {
  let line = '';
  for (let j = 0; j < i; j++) {
    line += '*';
  }
  console.log(line);
}

// 6. Inverted Right-Aligned Triangle
console.log("\nInverted Right-Aligned Triangle:");
for (let i = n; i >= 1; i--) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < i; j++) {
    line += '*';
  }
  console.log(line);
}

// 7. Inverted Pyramid
console.log("\nInverted Pyramid:");
for (let i = n; i >= 1; i--) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < 2 * i - 1; j++) {
    line += '*';
  }
  console.log(line);
}

// 8. Diamond
console.log("\nDiamond:");
for (let i = 1; i <= n; i++) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < 2 * i - 1; j++) {
    line += '*';
  }
  console.log(line);
}
for (let i = n - 1; i >= 1; i--) {
  let line = '';
  for (let j = 0; j < n - i; j++) {
    line += ' ';
  }
  for (let j = 0; j < 2 * i - 1; j++) {
    line += '*';
  }
  console.log(line);
}
```

---

## \u{1F5A5️} Output (n = 5)

```
Square:
*****
*****
*****
*****
*****

Left-Aligned Triangle:
*
**
***
****
*****

Right-Aligned Triangle:
    *
   **
  ***
 ****
*****

Pyramid:
    *
   ***
  *****
 *******
*********

Inverted Left-Aligned Triangle:
*****
****
***
**
*

Inverted Right-Aligned Triangle:
*****
 ****
  ***
   **
    *

Inverted Pyramid:
*********
 *******
  *****
   ***
    *

Diamond:
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
```

---