
## Introducing Token

토큰은 입력으로 사용할 수 있는 개별 유닛이다. 최초 신경망은 문자 수준의 학습을 했다. 다음 문자(character)로 무엇이 올 것인지 예상했다. 이는 모델에 너무 많은 것을 요구했다. 모델이 문자로 조합할 수 있는 모든 단어들이 어떻게 변경되고 어떤 의믜를 갖는지 모두 알고 있어야 했다. 

다음은 단어 수준의 학습을 했다. 다음에 어떤 단어가 필요한지 예상했다. 엄청난 어휘가 필요했다. 이는 또 다른 한계를 마주쳤다.

묶음 단위에 단어들을 만들고 이를 토큰이라고 했다. 토큰을 입력하고, 토큰을 출력하는 방식으로 모델을 설계했다. 전체 단어를 사용하거나 단어의 일부부만 조합하여 토큰을 만들었다. 

GPT's tokenizer 사이트에서 문장을 어떻게 토큰으로 만드는지 확인할 수 있다. 

일반적으로 영어에서 토큰화할 떄 규칙은 다음과 같다.

- 1 토큰은 4개의 글자로 이뤄진다.
- 1 토크은 평균적인 단어의 글자수를 고려해봤을 때 0.75개의 단어를 의마한다.
- 1000 토큰은 750개의 단어를 의미한다.
