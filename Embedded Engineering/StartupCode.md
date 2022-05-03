# 스타트업(Startup) 코드란?

프로그램이 작동되기 위해서 필요한 준비 과정을 위한 코드로 여러 초기화 작업과 C에서 사용할 메모리(스택, 힙) 등을 할당하고 마지막에 main() 함수를 호출하여 프로그램을 동작하게 한다.

'''
스타트업 코드의 일반적인 수행 순서

1. 모든 인터럽트 중지
2. 초기화된 데이터를 ROM to RAM 복사
3. 초기화되지 않은 데이터 영역 0으로 초기화
4. 스택을 위한 공간을 할당하고 초기화
5. 프로세서의 스택 포인터 초기화
6. 힙을 생성하고 초기화
7. 인터럽트 활성화
8. main() 함수 호출
'''