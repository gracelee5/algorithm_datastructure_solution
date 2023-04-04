# 2장 연습 문제 풀이

## 2.1 다음 계산 시간(입력 크기는 N)을 란다우 빅오 표기법으로 나타내라
$$
\large
\eqalign{
T_1(N)&=1000N\\
T_2(N)&=5N^2+10N+7\\
T_3(N)&=4N^2+3N\sqrt{N}\\
T_4(N)&=N\sqrt{N}+5N\log{N}\\
T_5(N)&=2^N+N^{2019}\\
}
$$

***

$$
\large
\eqalign{
T_1(N)&=O(N)\\
T_2(N)&=O(N^2)\\
T_3(N)&=O(N^2)\\
T_4(N)&=O(N\sqrt{N})\\
T_5(N)&=O(2^N)\\
}
$$


## 2.2 다음 프로그램의 복잡도를 구하고 란다우 빅오 표기법으로 표현하라. 이 프로그램은 N개 중에서 세 개를 고르는 방법을 모두 나열하는 프로그램이다.

```c++
for (int i = 0; i < N; ++i) {
    for (int j = i + 1; j < N; ++j) {
        for (int k = j + 1; k < N; ++k) {
            
        }
    }
}
```

$$
\large
T(N)=\binom{N}{3}=\frac{N(N-1)(N-2)}{6}=O(N^3)
$$

## 2.3 다음 프로그램의 복잡도를 구하고 란다우 빅오 표기법으로 표현하라. 이 함수는 양의 정수 N이 소인수인지 판정한다.

```c++
bool is_prime(int N){
    if ( N <= 1 ) return false;
    for ( int p = 2; p *p <= N; ++p){
        if ( n % p == 0 ) return false;
    }
    return true;
}
```
---
