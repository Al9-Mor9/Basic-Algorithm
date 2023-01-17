# #1920 수찾기 풀이
## Goal
길이 N의 정수 배열 A를 입력받은 후, M개의 정수 X들을 입력받을 때, 각 X가 배열 A에 들어있는지를 확인합니다. 

## Caution
N과 M이 각각 최대 100,000이므로, 만약 A 전체를 돌면서 각 X를 확인하려한다면 최대 10,000,000,000번의 연산을 해야하므로 **시간 초과** (시간복잡도 : **O(NM)**)

## Solution1 (binary search를 이용한 풀이)
i) 배열 A를 정렬하고(O(logN))
ii) 이진탐색을 통해 각 X가 A에 들어있는지를 확인합니다(O(logN))


## Solution2 (set을 이용한 풀이)
i) N개의 수들을 입력받아 모두 set에 넣습니다.(O(NlogN)) 
> set : 집합. 중복 허용하지 않음.

ii) 이후 M개의 수를 입력받으면서, 각각이 set에 들어있는지를 확인합니다. (O(1))