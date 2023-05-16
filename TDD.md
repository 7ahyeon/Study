
# Test-Driven-Development(TDD)
> # 프로그램을 작성하기 전에 테스트 먼저 하라!
> > **Test the program before you write it!**
> > - ‹TDD by Example> Kent Beck
</br>

- **테스트 주도 개발**
- 프로그램을 작성하기 전에 **테스트를 먼저 작성하는 것**
- 업무 코드를 작성하기 전에 테스트 코드를 먼저 작성하는 것
- 명시적인 코드로 **개발 종료 조건**을 정해놓은 것
</br>

# TDD 목표
> # 잘 동작하는 깔끔한 코드!
> > **Clean code that works**
> > - Ron Jeffries
</br>

- 제대로 동작할 뿐 아니라 **명확한 의미를 전달하는(Clean)** 코드!
</br>

# 개발에 있어 TDD 위치
- **소프트웨어 개발에서의 TDD :** 개발자가 자신을 위해 처음 수행하는 테스트
- 전통적 테스트 방법론에서의 단위 테스트는 기능 테스트에 가까움
- **TDD에서의 단위 테스트(unit test case) :** 메소드 혹은 함수 단위의 테스트 → 이후 발생하는 테스트 단계(통합/인수)에서의 결함발생 비용 절감
</br>

# TDD 진행 방식
|방식|내용|비고|
|:---:|:---|:---|
|질문(Ask)|테스트 작성을 통해 시스템에 질문한다.|테스트 수행 결과 실패|
|응답(Respond)|테스트를 통과하는 코드를 작성해서 질문(Ask)에 답한다.|테스트 수행 결과 성공|
|정제(Refine)|아이디어를 통합하고 불필요할 시 제거, 모호할 시 명확화하여 대답을 정제한다.|리팩토링|
|반복(Repeat)|다음 질문(Ask)을 통해 대화를 계속 반복한다.||
</br>

![TDD 순서도](https://github.com/7ahyeon/Study/assets/107123698/d6262548-9495-478d-8288-161184ffed11)

- TDD를 이용한 개발 : **질문 → 응답 → 정제**의 반복
- TDD 테스트 작성 : 단위 테스트 프레임워크(Unit Test Framework)를 사용
</br>

# TDD 장점
* 개발의 방향을 잃지 않게 유지해줌!
- 어떤 기능을 개발하고 있고 어디까지 와 있는지 살펴볼 수 있음
- 남은 단계와 목표를 잊지 않게 도와줌
- (개발 도중 자리를 비우게 될 때 작성하는 테스트 케이스를 일부러 실패하게 만들어서 돌아왔을 때 재시작 시점을 바로 알 수 있도록 함)
* 품질 높은 소프트웨어 모듈 보유!
- TDD를 통해 만들어진 애플리케이션은 필요한만큼 테스트를 거친 '품질이 검증된 부품(모듈)'을 가짐
- 연구 결과 : TDD 미사용 개발팀에 비해 TDD 사용 팀의 **결함률이 최대 1/10 정도까지 감소됨**(2003/2006 IBM/Microsoft 개발팀 대상)
* 자동화된 단위 테스트 케이스 갖게됨!
- 자동화된 단위 테스트 케이스 : 개발자가 필요한 시점에 언제든지 수행 가능 및 현재까지 작성된 시스템에 대한 이상 유무 즉시 확인 가능
- 회귀 테스트에 대한 부담 감소 / 콘솔에서 원하는 부분의 로그를 찾아내야 하는 수고 감소

</br>


</br>

> # 테스트 주도 개발 : 고품질 쾌속 개발을 위한 TDD 실천법과 도구
> > - 채수원