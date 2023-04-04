# 2장 연습 문제 풀이

## 2.1 다음 계산 시간(입력 크기는 N)을 란다우 빅오 표기법으로 나타내라
$$
\large
\eqalign
{
T_1(N)&=1000N\\
T_2(N)&=5N^2+10N+7\\
T_3(N)&=4N^2+3N\sqrt{N}\\
T_4(N)&=N\sqrt{N}+5N\log{N}\\
T_5(N)&=2^N+N^{2019}\\
}
$$
---
T1(N) = N  
T2(N) = N^2  
T3(N) = N^2  
T4(N) = N√N  
T5(N) = 2^N  

## 2.2 다음 프로그램의 복잡도를 구하고 란다우 빅오 표기법으로 표현하라. 이 프로그램은 N개 중에서 세 개를 고르는 방법을 모두 나열하는 프로그램이다.

<pre><code>{
for (int i = 0; i < N; ++i) {
    for (int j = i + 1; j < N; ++j) {
        for (int k = j + 1; k < N; ++k) {
            
        }
    }
}
}</code></pre>
---
T(n) = NC3

$$
\large
T(N)=\binom{N}{3}=\frac{N(N-1)(N-2)}{6}=O(N^3)
$$


N^3
