# Sort


## C++ STL sort() 함수

sort() 함수의 사용법은 아래 예시와 같이 배열의 시작점 주소와 마지막 주소+1 을 매개변수로 대입한다
```cpp
#include <iostream>
#include <algorithm>

using namespace std;

int main(void)
{
    int arr[10] = {0,.3 ,5, 6, 2, 4, 2, 1, 3, 2};
    sort(arr, arr+10);
    for(int i = 0; i < 10; i++)
    {
        cout << arr[i] << ' ';
    }

    return 0;
}

```

또한 sort 함수의 새번째 매개변수로 함수를 받아 자신이 원하는 방식으로 정렬을 할 수 있게 한다.

```cpp
#include <iostream>
#include <algorithm>

using namespace std;

/* 내림차순 정렬 함수 */
bool compare(int a, int b)
{
    return a > b;
}
int main(void)
{
    int arr[10] = {0,.3 ,5, 6, 2, 4, 2, 1, 3, 2};
    sort(arr, arr+10, compare);
    for(int i = 0; i < 10; i++)
    {
        cout << arr[i] << ' ';
    }

    return 0;
}

```

또한 특정 class 변수 혹은 구조체 변수일 경우 다음과 같은 방식으로 특정 변수를 기준으로 정렬이 가능해진다.
