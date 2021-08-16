# JUnitTest

<h2> JUnit이란 </h2>

- 단위 테스트 Framework
- 문자 혹은 GUI기반으로 실행
- 단정문으로 테스트 케이스의 수행 결과를 판별 (assertXXX)
- 간결한 어노테이션 지원 
- 성공, 실패 결과 표시 

<code>
@Test
public void Calc() {
  Calculator calculator = new Calculator();
  assertEquals(30, calculator.sum(10,20));
}
</code>




----

참조: nextree.co.kr/p11104/
  

