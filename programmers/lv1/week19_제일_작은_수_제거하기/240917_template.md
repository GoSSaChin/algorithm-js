[![PRO]][Link]

## 문제 해석

- 제일 작은 수 뺀 나머지 배열만 return
- return할 배열이 비어있으면 [-1]을 리턴

## 최종 제출 코드

```js
function solution(arr) {
    let minArr = Math.min(...arr);
    let newArr = arr.filter(num => num !== minArr);
    if (newArr.length == 0) return [-1];
    return newArr;
}
```

## 시간 복잡도

-   **∴ O(N)**

## 메모

- arr.filter의 매개변수에 유의
  - arr.filter(callback(element, index, array), thisArg);

<!---------------------------------------------------------------------------->

[PRO]: https://github.com/GoSSaChin/algorithm-js/assets/107768516/67c43b52-bc3f-4571-a249-5519021afbb0
[Link]: https://school.programmers.co.kr/learn/courses/30/lessons/12935
