---
title:  "제12회 전국 중학생 IT 올림피아드 후기"
excerpt: "실패하면 다시 해보면 되지"

header:
    teaser: /assets/images/review-dimigo-olympiad/teaser.JPG
    
classes: wide

toc: false
toc_sticky: false

published: false

categories:
  - 일상/후기
last_modified_at: 2022-09-04T13:55:00+09:00
sitemap:
  changefreq: daily
  priority: 0.8
---

원하던 고등학교에 입학하기 위해서는 국영수 성적이 매우 좋거나 입상실적이 있어야 합격할 수 있었다. 나는 국영수 성적이 썩 좋지는 않았기 때문에 입상실적이 필요했다. 그래서 이 대회와 정보올림피아드에 참가하기로 했다.

벌써 6년이 지났다. 그래서 잘 기억이 나진 않지만 뒤늦게라도 후기를 기록해두려고 한다.

## 2015년 예선 탈락
사실 제12회 전에 제11회 대회에도 참가했었다. C언어 1년 공부하고 경험삼아 출전했는데 역시 많이 부족했는지 예선에서 탈락해버렸다. 그 당시의 심정은 화가 났던 것 같다. 광주에서 안산까지 3시간 30분이 걸리고 아침에 첫차를 타도 대회 시간안에 도착을 못해서 전 날 근처에 방까지 잡았는데 허무하게 예선에서 탈락해버린 내 자신한테 화가났다.

> *내년에 무조건 다시 온다.*

라고 다짐하고 집가서 1년동안 다시 공부를 한다.

## 2016년 다시 도전
포인터 관련 파트를 다시 복습하고 자료구조까지 어느정도 공부를 했다. 백준 온라인 저지에서 문제도 몇 개 풀고 다시 도전하러 안산으로 출발한다.

예선문제는 필기시험이었다. 기억에 남는 문제는 포인터 연산이랑 파스칼 삼각형 문제였다.

```cpp
int main(void)
{
    int num1 = 10;
    int num2 = 20;
    
    int * ptr1 = &num1;
    int * ptr2 = &num2;
	
    *ptr1 += 5;
    ptr1 = ptr2;
    
    printf("%d \n", *ptr1);
    return 0;
}
````
> 다음 출력 결과는 무엇인가?

대충 이런 식의 문제였다. 중학생 수준이라 포인터를 너무 어렵게 꼬아서 내진 않았었던 거 같다.

![파스칼 삼각형](/assets/images/review-dimigo-olympiad/pascal.PNG){: .align-center width="500"}

파스칼 삼각형은 인접한 상단의 두 수의 합으로 이루어진 삼각형이다. 다음과 같은 코드를 제시하고 출력 결과를 맞추는 문제였다.

```cpp
int pascal(int n, int m)
{
    static int cache[20][20];
    if (n == 1 || m == 1)
        return 1;
    if (cache[n][m] != 0)
        return cache[n][m];
    else
        return cache[n][m] = path(n - 1, m) + path(n - 1, m - 1);
}
```
> pascal(5, 3)의 출력 결과는 무엇인가?

이 때는 재귀함수도 열심히 공부했기 때문에 어렵지 않게 맞출 수 있었다.
점심으로 돈까스가 나왔던 걸로 기억하는데 맛있었다. 꼭 이 학교에 입학해야겠다 싶었다.

점심먹고 예선 결과를 기다리는데 설마 또 떨어지면 어쩌나하는 마음 때문에 더 긴장됐던 거 같다.
다행히 본선 진출자 명단에 내 이름이 있었다.

본선은 컴퓨터로 직접 알고리즘 문제를 풀었는데 문제가 기억이 안난다..

결과 발표를 보기 위해 학교 홈페이지에 들어가봤다.

![결과 발표 공지](/assets/images/review-dimigo-olympiad/awards.JPG){: .align-center width="500"}
한 번 예선에서 떨어지고 다시 도전해서 상을 받아서 그런가 너무 기뻤다.

![디미고 정문 사진](/assets/images/review-dimigo-olympiad/dimigo.JPG){: .align-center width="500"}
![시상식 사진](/assets/images/review-dimigo-olympiad/banner.JPG){: .align-center width="500"}
