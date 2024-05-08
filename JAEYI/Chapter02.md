## Chapter - 02 : 이상한 나라의 객체

#### 📌 앨리스와 객체

이상한 나라의 앨리스에서 앨리스의 키가 커지고 작아지는 상황을 생각해보자. 앨리스는 버섯을 먹으면 작아지고 케이크를 먹으면 커진다. </br>
여기서 앨리스의 키를 변화시키는 것은 앨리스의 행동이다. </br>
행동에 따라 앨리스의 상태가 변하게 된다. </br>
</br>
또한 상태에 따라 행동의 결과가 달라진다. </br>
"앨리스의 키(현재 상태) = 이전 키(이전 상태) + 앨리스의 행동(현재 행동)" 이라는 공식이 만들어진다. </br>
</br>
즉, 어떤 행동의 성공 여부는 이전에 어떤 행동들이 발생했는지에 영향을 받는다. </br>
따라서 행동 간의 순서가 중요하다.</br>
</br>
그리고 앨리스는 상태 변화와 무관하게 유일한 존재로 식별 가능하다. </br>
</br>
#### ⭐️ 객체란 식별 가능한 개체, 혹은 사물을 의미한다.
  객체는 셀 수 있고, 생성 시점을 알 수 있으며, 식별 가능하고, 독립적인 하나의 단위로 인식할 수 있어야 한다. </br>
  객체는 상태(state), 행동(behavior), 식별자(identity)를 지닌 실체이다. </br>
  소프트웨어 내에서는 객체는 저장된 상태와 실행 가능한 코드를 통해 구현된다. </br>
<br>

#### 📌 객체의 상태
객체가 어떻게 환경과 상호작용 하는지는 그 시점에 객체에 어떤 일이 발생했느냐로 좌우된다. </br>
행동의 결과는 과거 행동에 영향 받으므로 행동의 과정과 결과를 간단하게 기술하기 위해 상태라는 개념이 고안되었다. </br>
상태를 통해 행동의 결과를 쉽게 예측할 수 있으며 현재를 기반으로 객체의 행동 방식을 이해할 수 있다. </br>

숫자, 문자열, 양, 속도, 시간, 날짜, 참/거짓과 같은 단순한 값들은 객체가 아니다. </br>
단순한 값들은 다른 객체의 특성을 표현(상태를 표현)하는 데 사용된다. </br>
</br>
ex. 앨리스가 음료수를 들고 있는 상태인지 표현하기 </br>
</br>
앨리스 (키 : 130, 위치 : 통로) - 음료 (양 : 0.5L)
- 앨리스와 음료가 연결되어 있음으로 음료를 가진 것으로 볼 수 있다.
- 앨리스의 상태는 앨리스가 가지고 있는 특성(키, 위치)과 다른 객체(음료)로 표현된다.

#### ⭐️ 모든 객체의 상태는 단순한 값과 객체의 조합으로 표현할 수 있다.
객체를 구성하는 모든 특징을 객체의 프로퍼티(property)라고 한다. (앨리스이 경우 키, 위치, 음료) </br>
대부분의 프로퍼티 자체는 정적이다. 그러나 프로퍼티 값 자체는 시간에 따라 변하기 때문에 동적이다. </br>

#### ⭐️ 객체와 객체 사이의 의미 있는 연결을 링크(Link)라고 한다.

객체는 링크를 통해서만 메시지를 주고 받을 수 있다. </br>
링크는 객체가 다른 객체를 참조할 수 있다는 것을 의미한다. </br>
이는 한 객체가 다른 개체의 식별자를 알고 있다는 뜻이다. </br>

#### ⭐️ 객체 간의 선으로 표현되는 링크와 달리 객체를 구성하는 단순한 값은 속성(attribute)라고 한다.

앨리스의 예시에서 키와 위치는 속성이다. 

</br>

#### 📌 객체의 행동 </br>
객체는 자율성이 보장되기 때문에 간접적으로 객체의 상태를 변경하거나 조회할 수 있는 방법이 필요하다. </br>
행동은 다른 객체가 간접적으로 객체의 상태를 변경하는 것을 가능하게 한다. </br>
</br>

#### 📌 객체의 식별자