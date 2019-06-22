---
title: compact set
layout: post
image:
  background: triangular.png
tags:
- study
---

pma로 해석학을 독학하다보니 생략한부분이 너무많아서 참고도서를 한권더 활용하기로했다
참고도서명은 introduction to real analysis

나는 지금 compact set의
closed and bounded -> compact를 heine-borel theorem으로 증명하는 과정을 공부하고있다.

compact set이 되기위한 조건중 하나가 compact set k is contained in the union of finite number of sets in G인데 

이 증명의 핵심이 closed set에 있어서
k is not contained in the union of any finite number of sets in G의 모순점을 찾는것이다

난 사실 이 과정이 조금 이해가 안간다.

이 증명에 따르면 이 집합을 잘게잘게 쪼갰을때 그중 하나의 집합이 원소 m에 수렴하게되며 
그 원소 m를 포함하는 임의의 open set을 잡으면 그 set은 원소 m주변의 작은 집합을 포함하므로
모든 작은 집합에 대해서 각각의 집합을 union of finite number of set 으로 표현가능하다

라는건데 

이 논리를 그대로 open set에 가져오면 m가 무한히 0에 수렴할때
(0, m&#124; 를 포함하는 cover(0, 2m)을 잡으면 저 집합을 항상 포함하게되므로
결국 open set도 compact set이 된다. 
cover의 크기를 어떻게 잡든간에 항상 저 집합보다 크므로..

하지만 open set에서는 분명이 예외적인 경우가 발생하는데
그 예외적인 경우는 (0, m&#124; 를 무한히 많은 cover로 포함해야하는것이 아니라(결론적으로는 맞긴한데)

근본적으로 (0, k&#124; 를 온전히 포함하는 cover가 없어도 (0, 1)을 포함하는 cover의 모임이 존재한다..라는것이다

조금더 쉽게 예를들어 설명하자면 closed set에서 m주변의 영역을 무한한 cover로 덮어야 하는게 아니라 m주변의 영역을 한방에 덮는 cover가 아예 없을수도 있다는것이다.
하지만 closed set의 경우에는 이 m을 포함하지않으면 cover에다가 극한값을 취해도 다가갈수없으니까 m을 포함하는 cover가 최소 하나는 있어야한다 라는것이 좀더 엄밀한 증명이다.

그러니까 이건 음.. cover의 개수가 무한이고 유한이고가중요한게 아니라
극한값을 취했을때 다가갈수있는냐 없느냐의 문제인데

그걸 대체할만한 수학적인 표현수단이 cover의 개수가 무한이냐 유한이냐 이런말인거같다.

결정적으로 내가 궁금한건 극한값을 취했을때 다가갈수없을때, cover의 개수가 유한으로 표현 가능하고 극한값을 취했을때 다가갈수 있을때 cover의 개수가 무한이 될수 있느냐로 완벽하게 대체 가능한지이다.

사실 이거때문에 pma 2.41에서 every infinite subset of E has a limit point in E라는것이 E is compact라는것과 동치인가를 논하는것같다.