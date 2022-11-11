---
layout: post
title: 없는 숫자 더하기
subtitle: 프로그래머스(level1)
categories: algorithm
tags: [algorithm]
---

오늘 내가 한 일

- 깃허브 레포지토리 생성
- intellij - 학생인증 완료
- 프로그래머스 코딩문제 풀이
- 최초 커밋

### 오늘 내가 푼 코딩테스트 문제

level1 - 없는 숫자 더하기

 ⇒ [https://school.programmers.co.kr/learn/courses/30/lessons/86051](https://school.programmers.co.kr/learn/courses/30/lessons/86051)

```kotlin
class Solution {
    fun solution(numbers: IntArray): Int {
    var answer:Int = 0

    var numberarray = arrayListOf(0, 1, 2, 3, 4, 5, 6, 7, 8, 9)

    var array = ArrayList<Int>()

    for(i in 0 until numbers.size){
        if(numberarray.contains(numbers[i])){
            numberarray.remove(numbers[i])
        }
    }

    for(i in numberarray){
        answer += i
    }

    return answer
    }
}
```


