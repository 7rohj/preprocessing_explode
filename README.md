# preprocessing_explode

## 엄청 오랫동안 시간 잡고 만든 코든데, 한줄로 되버리는..


![image](https://user-images.githubusercontent.com/99319638/196689202-6219a793-6abc-4df7-972c-9eacd0d658bb.png)

위 테이블에서 end 열의 길이를 1로 만들어주고 싶었다. <br/>
그래서 길이를 구하고 1인경우, 2인경우, 3인경우.. 나눠서 end에서의 0번째, 1번째 .. 또 나눠주고 <br/>
그걸 빈 리스트에 담고 append 시키고 데이터프레임으로 만들어주고 <br/>
그랬는데 ............... <br/>

한줄로 가능한 것이였다.

![image](https://user-images.githubusercontent.com/99319638/196690172-3a8734d2-b0b6-48da-9d2b-425cd9c89fbb.png)

length 가 2인 경우만 캡쳐한 사진 `^.^` (5까지 반복 후 concat으로 결합) <br/>
for 문으로 했을때 [i]가 안먹기에 다 나눠줘서 코드를 짰지만..

```
table.explode('start').explode('end')
```
한 줄로 모든 걸 해결! 😅

![image](https://user-images.githubusercontent.com/99319638/196690741-18c6b384-6738-45bd-a247-2f21102cb205.png)
