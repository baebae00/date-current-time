# Today's date and current-time
### Informing Today's date and current time

```python
import time

x=time.ctime() #변수 x에 time함수를 선언해준다 이때 x는 리스트함수로 각 문자가 위치에 따른 번호를 부여받는다

h=int(x[11:13])-12 #리스트 x의 11~12번 위치에 해당하는 문자열을 int를 통해 정수로 변환해 준 후 12를 빼준다 그리고 이것을 h에 할당한다

a=("오늘의 나짜: %s년 %s월 %s일\n현재 시간: %s시 %s분 %s초"%(x[20:24],x[4:7],x[8:10],h,x[14:16],x[17:19])) 
#%s를 이용하면 여러개의 변수를 여러 군데에 한번에 저장시킬 수 있다(for 편의성), \n는 줄 바꿈을 나타내는 특수 문자열이다

print(a) #a를 출력한다

```
