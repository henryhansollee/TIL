---
description: 가장 많이 사용되는 리액트 상태관리 라이브러리
---

# 01\_Redux

#### 1-1. 액션

* 상태에 변화가 필요하면 액션\(action\)이 발생.
* 하나의 객체.
* 액션 객체는 type 필드를 반드시 가지고 있어야 함.

```text
{
    type: 'TOGGLE_VALUE'
{
    type: 'ADD_TODO',
    data: {
        id: 1,
        text: '리덕스 배우기'
    }
}
{
    type: 'CHANGE_INPUT'
    text: '안녕하세요.'
}
```

