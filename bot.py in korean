import random
from googletrans import Translator

# 랜덤 응답을 담은 리스트
random_responses = ["That is quite interesting, please tell me more.",
                    "I see. Do go on.",
                    "Why do you say that?",
                    "Funny weather we've been having, isn't it?",
                    "Let's change the subject.",
                    "Did you catch the game last night?"]

translator = Translator()

print("안녕하세요, 저는 간단한 로봇 Marvin입니다.")
print("언제든지 '잘가'라고 입력하시면 대화를 마칠 수 있어요.")
print("각 답변을 입력한 후 '엔터'를 누르세요.")
print("오늘은 어떠세요?")

while True:
    # 사용자 입력 받기
    user_input = input("> ")
    if user_input.lower() == "잘가":
        # 'bye' 입력 시 대화 종료
        break
    else:
        # 랜덤 응답 선택
        response = random.choice(random_responses)
        # 응답을 한국어로 번역
        response_translated = translator.translate(response, dest='ko').text
    print(response_translated)

print("대화해 주셔서 감사합니다. 안녕히 가세요!")
