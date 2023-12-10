# 정의

SW로 해결하고자 하는 문제 영역(ex: 온라인 서점)

# 계층 구성

한 Domain은 다시 하위 Domain으로 나눌 수 있다. 하위 Domain을 어떻게 구성할지 여부는 문제 상황에 따라 달라진다.

ex) Catalog 하위 Domain은 고객에게 구매할 수 있는 상품 목록을 제공, 주문 하위 Domain은 고객의 Order을 처리.

![[ex_ddd_graph.png]]


# 주의

모든 Domain을 SW로 직접 처리하지 않는다.

ex) 배송, 결제와 같은 문제는 외부 시스템을 이용할 수 있다.