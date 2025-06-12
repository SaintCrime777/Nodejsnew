# 新NODE開始


``` javascript
console.log("Hello!");

// 公式解
/*function sumSequence(n) {
  return n * (n + 1) / 2; // 等差數列公式
}*/

// for迴圈用reduce取代
function sumSequence(n) {
  return Array.from({length: n}, (_, i) => i + 1)
    .reduce((acc, num) => acc + num, 0);
}
const sum=sumSequence(100);
console.log(sum);