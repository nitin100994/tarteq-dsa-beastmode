# 🚀 Move Zeroes to End — Full Code Understanding

## ✅ Problem Statement

Given an array, move all the `0`s to the end, while maintaining the order of all non-zero elements. You must do this **in-place** without using any extra array.

---

## 🔍 Approach Summary

1. **Use a pointer (`insertPos`)** to track the position where the next non-zero element should be placed.
2. **Loop through the array** once to bring all non-zero values forward.
3. After the loop, **fill the remaining part of the array with zeroes** from `insertPos` to the end.

---

## 💻 Code

```js
function moveZeroes(arr) {
  let insertPos = 0;

  // Move non-zeroes to the front
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] !== 0) {
      arr[insertPos] = arr[i];
      insertPos++;
    }
  }

  // Fill the rest of the array with 0s
  while (insertPos < arr.length) {
    arr[insertPos] = 0;
    insertPos++;
  }

  return arr;
}