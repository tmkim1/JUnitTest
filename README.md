# JUnitTest

<h2> JUnit이란 </h2>

- 단위 테스트 Framework
- 문자 혹은 GUI기반으로 실행
- 단정문으로 테스트 케이스의 수행 결과를 판별 (assertXXX)
- 간결한 어노테이션 지원 
- 성공, 실패 결과 표시 

</h3> 예시 </h3>
  @Test
  public void Calc() {
    Calculator calculator = new Calculator();
    assertEquals(30, calculator.sum(10,20));
  }

@Test: 해당 어노테이션이 선언된 메서드가 단위 테스트 메서드임을 지정
assertEquals: 기댓값과 결과값이 일치하는지 확인 

<h3> 대표적인 단정문 </h3>

assertArrayEuals(a, b): 배열 a와 b가 일치함을 확인
assertEquals(a, b): 객체 a와 b의 값이 같은지 확인
assertSame(a, b): 객체 a와 b와 같은 객체임을 확인 
assertTue(a): a가 참인지 확인
assertNotNull(a): a객체가 null이 아님을 확인 

<h3> 기본 Annotation </h3>

@BeforeAll 

- 해당 annotation이 달린 메서드가 현재 클래스의 모든 테스트 메서드보다 먼저 실행 됨을 의미
- 해당 메서드는 static 이어야 한다. 
- JUnit5 이전 @BeforeClass와 동일 

@BeforeEach

- 해당 annotation이 달인 메서드가 각 테스트 메서드 전에 실행 됨을 의미
- JUnit5 이전 @Before과 동일 

@AfeterAll

- 해당 annotation이 달린 메서드가 현재 클래스의 모든 테스트 메서드보다 이후에 실행 됨을 의미 
- 해당 메서드는 static 이어야 한다. 
- JUnit5 이전 @AfterClass 동일 

@AfterEach

- 해당 Annotation이 달린 메서드가 각 테스트 메서드 이후에 실행 됨을 의미 
- 이전의 @After와 동일 


@DisplayName

- 테스트 클래스 또는 테스트 메서드의 이름을 정의 

@Disable

- 테스트 클래스 또는 메서드를 비활성화
- 이전의 @Ignore와 동일 




----

참조: nextree.co.kr/p11104/
     http://junit.sourceforge.net/javadoc/org/junit/Assert.html (assert 단정문 문서)
     https://gmlwjd9405.github.io/2019/11/26/junit5-guide-basic.html
  

