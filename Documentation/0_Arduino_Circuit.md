<참고> 
1. [http://ardunityproject.blogspot.com/2016/06/blog-post.html](http://ardunityproject.blogspot.com/2016/06/blog-post.html)
2. [https://m.blog.naver.com/PostView.nhn?blogId=ndb796&logNo=221242719701&proxyReferer=https%3A%2F%2Fwww.google.com%2F](https://m.blog.naver.com/PostView.nhn?blogId=ndb796&logNo=221242719701&proxyReferer=https%3A%2F%2Fwww.google.com%2F)

<회로 설계 추천>
1. [https://www.circuito.io/](https://www.circuito.io/)


# Arduino Circuit

회로(Circuit)란 필요로 하는 전기적 특성을 얻을 수 있도록 전원과 부품을 접속한 것을 의미합니다. 회로가 잘 작성되어야 실질적으로 필요한 신호 혹은 에너지를 처리할 수 있는 기능을 갖추게 됩니다.

회로상 전류가 흐르게 해야 하는데, 전류가 흐른다는 것은 전위가 높은 곳에서 전위가 낮은 곳으로 흐르는 것을 의미합니다.

전위란 전기장 내에서 단위 전하가 가지는 위치에너지를 말하는 것으로 전위는 낮은곳(Ground)로 흐르게 됩니다. 전압이란 전위의 차이를 말하는데, 전류가 흐를 때 발생합니다. 가장 많이 사용되는 전위는 3.3V, 5V, 12V입니다. 자신이 사용하고자 하는 전위와 목적에 맞는 전원 공급이 필요합니다.

## 브래드 보드(Breadboard)
![브레드보드](https://www.makeall.com/member/file_guest/1893400515_iYce2jT1_BEC6B5CEC0CCB3EB3.png)

브래드 보드는 납떔없이 아두이노 회로를 꾸밀 수 있는 기판입니다. 내부에는 한 줄씩 철들이 있어 같은 철에 꽂힌 부품들끼리 연결되게 설계되어 있습니다. 한 부품의 단자들을 모두 한 줄에 연결하면 쇼트현상이 발생하고 작동이 안되니, 반드시 서로 다른 줄에 연결시켜야합니다.

![브레드 보드 연결 설명](https://t1.daumcdn.net/cfile/tistory/2504E94757D6482C20)

참고 : [http://www.makeshare.org/bbs/board.php?bo_table=Parts&wr_id=46](http://www.makeshare.org/bbs/board.php?bo_table=Parts&wr_id=46)

## 점퍼선
![점퍼와이어](http://makeshare.org/data/editor/1703/thumb-b8fba66967061747fae5723bede39439_1489481019_55_700x222.png)

브레드보드 사용시 전류가 흐르도록하며 배선을 편리하게 하기위해서 사용하는 핀이 꼽힌 전선입니다. 점퍼선에 핀이 튀어나온 부분이 (M) 수단자 부분, 튀어나오지 않은 부분을 (F) 암단자 부분이라고 합니다. 양쪽 핀이 둘다 튀어나와 있으면 M-M 타입 점퍼선, 들어가 있으면 F-F 타입 점퍼선, 한 쪽은 나오고 한쪽은 들어가 있다면 M-F타입 점퍼선 입니다. 

## 핀 맵(Pin Out)
![아두이노 우노 핀맵](http://mblogthumb2.phinf.naver.net/MjAxNzExMjJfMTQ2/MDAxNTExMzExNjE1Nzk4.7FnhAgmW9G5aA3SUf89CMnS5Zv8EC_6tlJk4fgQXB5cg.fURVwHjYgj-FmYk5-c6mrE_9RW7d4lsc-Bs0ifm-ZKwg.PNG.compass1111/image.png?type=w800)

회로에 사용되는 모든 부품은 핀(Pin)이라 부르는 전선을 연결하기 위한 부분이 존재합니다. 각 핀은 명칭이 있으며 용도가 정해져 있습니다. 이 핀 맵에 맞게 회로를 연결해야 문제 없이 잘 작동합니다. 현재 사용 중인 부품의 핀에 대한 정보를 알기 위해서는 데이터 시트(Datasheet)라 부르는 문서를 봐야합니다. 칩이 아닌 LED와 같은 부품들도 핀 맵이 존재합니다.

## 외부 전원

외부 전원이란 배터리나 어댑터 등을 통해 전원을 공급 받는 것을 말 합니다. 외부 전원을 이용한다면 USB연결 없이도 아두이노 보드는 독립적으로 작동할 수 있습니다. 

참고 : [https://deneb21.tistory.com/545](https://deneb21.tistory.com/545)



## VCC and GND

모든 회로는 (+)극에서 (-)극으로 끝납니다. 전자 회로에서는 (+)극을 VCC라고 부르고 (-)극을 GND(Ground)라고 부릅니다. 

VCC는 항상 전압 크기를 같이 표기합니다. 예를 들어 VCC(5V)등으로 표기합니다. VCC를 생략하고 5V로만 표기하는 경우도 있는데 모두 (+)극을 의미합니다.

GND(Ground)는 전압의 크기와 상관 없이 모두 공통으로 사용합니다. 즉 GND1, GND2등의 구분 없이 1개의 GND로만 불리기 떄문에 GND가 표기되어 있는 것은 모두 연결해야 합니다. 이것을 공통 그라운드(Common Ground)라고 말합니다. 


## 쇼트(Short)

전자 회로에서 쇼트는 (+)극과 (-)극이 직접 연결되는 것을 말하며 이런 일이 발생하면 회로에 엄청난 전류가 흘러 부품이 타버리는 상황이 발생합니다.

