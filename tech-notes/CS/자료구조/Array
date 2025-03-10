# 배열 (Array)
> 배열(Array)은 같은 타입의 데이터를 연속된 메모리 공간에 저장하는 자료구조입니다.

## 1️⃣ 배열의 특징
- **인덱스를 사용하여 데이터에 접근** (O(1))
- **연속된 메모리 공간을 차지** (중간 삽입/삭제가 비효율적)
- **고정된 크기** (동적 배열을 사용하면 크기 변경 가능)

## 2️⃣ 배열의 시간 복잡도
| 연산 | 평균 시간 복잡도 | 설명 |
|------|----------------|------|
| 접근 (Access) | O(1) | 인덱스를 통해 즉시 접근 가능 |
| 탐색 (Search) | O(n) | 원하는 요소를 찾을 때 최악의 경우 끝까지 탐색 |
| 삽입 (Insert) | O(n) | 중간에 삽입할 경우, 나머지 요소들을 이동해야 함 |
| 삭제 (Delete) | O(n) | 중간 요소를 삭제할 경우, 나머지 요소들을 이동해야 함 |

## 3️⃣ 배열과 연결 리스트 비교
|  | 배열 (Array) | 연결 리스트 (Linked List) |
|---|-------------|------------------|
| 메모리 | 연속된 공간 | 임의의 메모리 할당 |
| 접근 속도 | O(1) (인덱스로 접근) | O(n) (순차 탐색) |
| 삽입/삭제 | O(n) | O(1) |

## 4️⃣ 배열의 활용 사례
✅ **리더보드 (Leaderboard)**  
   → 점수 순으로 저장하고 빠르게 접근 가능  

✅ **2D 그래픽 처리**  
   → 행렬(Matrix) 연산을 수행할 때 유용  

✅ **캐시(Cache) 메모리**  
   → 데이터를 빠르게 가져오기 위해 배열 사용  

## 5️⃣ 배열 구현 예제 (JavaScript)
```javascript
class MyArray {
  constructor() {
    this.data = [];
    this.length = 0;
  }

  push(item) {
    this.data[this.length] = item;
    this.length++;
    return this.length;
  }

  pop() {
    if (this.length === 0) return undefined;
    const lastItem = this.data[this.length - 1];
    delete this.data[this.length - 1];
    this.length--;
    return lastItem;
  }

  get(index) {
    return this.data[index];
  }
}

const arr = new MyArray();
arr.push(10);
arr.push(20);
console.log(arr.get(1)); // 20
arr.pop();
console.log(arr.get(1)); // undefined
