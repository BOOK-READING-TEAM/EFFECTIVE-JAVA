# null이 아닌, 빈 컬렉션이나 배열을 반환하라

- null을 반환하는 메서드를 사용할 때면 항시 방어 코드를 넣어줘야 한다.
- 성능저하가 우려되는 경우, 빈 배열 인스턴스를 미리 생성, 반환하며 최적화가 가능하다

``ex) private static final Chees[] EMPTY_CHEESE = new Cheese[];``

- 불변 컬렉션을 이용하는 것도 가능 하다.

``ex) Collections.emptyList``