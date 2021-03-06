# 선택정렬

> 버블정렬이 각 회전이 끝날 때마다 맨 마지막 데이터의 위치가 정해졌던 것과 반대로 **선택 정렬은 n번째 회전이 끝날 때마다 앞에서 n번째 데이터의 위치가 정해진다.**
>
> 1. 먼저 주어진 리스트 중에 최솟값을 찾는다.
> 2. 그 값을 맨 앞에서 위치한 값(가장 왼쪽 값)과 바꾼다.
> 3. 맨 앞을 제외하고 다시 순회하면서 최소값을 찾는다.
> 4. 그 값을 맨 앞 바로 다음 위치(n+1)와 교체한다. ...반복...

<br />
<img src="https://blog.kakaocdn.net/dn/cSAFhj/btqwXd06SNh/kaKR9rl4IGEwH9JFRQSsw0/img.gif" alt="선택정렬"></img>
<br />

## 시간복잡도(Big O)

**- 최악: O(n^2)**: 정렬이 하나도 안되어 있는 경우
**- 최선: O(n^2)**: 이미 정렬이 되어있는 경우

선택정렬은 버블정렬과, 삽입정렬과는 다르게 정렬이 이미 되어있는 경우에도 O(N^2)의 시간 복잡도를 갖는다. 그 이유는 매번 정해진 자리에 올 수 있는 최소값을 찾아야하기 때문이다. 그렇기 때문에 성능이 매우 떨어진다.

## 장점

in place알고리즘이기 때문에 **메모리가 절약된다.** 또한, 직관적이므로 이해하기 쉽고 구현하기도 쉽다.

## 단점

**최선의 경우에도, 최악의 경우에도 O(N^2)**이 시간이 걸리는 만큼 성능 떨어진다.

## Unstable

선택정렬은 데이터가 중복된 경우 위치가 바뀔 수 있다. 따라서, Unstable한 정렬이다.
