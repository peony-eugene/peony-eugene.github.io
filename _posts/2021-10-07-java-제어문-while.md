# 제어문
## while문
- 반복해서 문장을 수행해야 할 경우 while문을 사용한다
- 조건문이 참인 동안 while문 아래 문장을 계속해서 수행한다
- 무한 루프: 무한히 반복한다는 의미


```python
while (조건문) {
    <수행할 문장1>
    <수행할 문장2>
    <수행할 문장3>
    ...
}
```

- 예제
    - 열 번 찍어 안 넘어 가는 나무 없다
    - 아래 예제에서 while문의 조건문은 treeHit<10 으로 treeHit이 10보다 작은 동안 while 문을 수행한다. 
    - treeHit이 10이 되면 treeHit<10이라는 조건문이 거짓이 되어 while문을 빠져나가게 된다


```python
int treeHit = 0;
while(treeHit <10) {
    treeHit++;
    System.out.println("나무를 "+ treeHit +"번 찍었습니다.");
    if(treeHit == 10) {
        System.out.println("나무 넘어갑니다.");
    }
}
```

- 위 코드 실행 결과


```python
나무를  1번 찍었습니다.
나무를  2번 찍었습니다.
나무를  3번 찍었습니다.
나무를  4번 찍었습니다.
나무를  5번 찍었습니다.
나무를  6번 찍었습니다.
나무를  7번 찍었습니다.
나무를  8번 찍었습니다.
나무를  9번 찍었습니다.
나무를  10번 찍었습니다.
나무 넘어갑니다.
```

## while문 빠져 나가기(break)

- break를 통해서 while문을 강제로 빠져나간다

- 예제  
    - 커피가 자판기 안에 충분하게 있을 때는 항상 "돈을 받으면 커피를 줘라" 라는 조건문을 가진 while문이 수행된다. 
    - 커피의 양을 따로이 검사를 해서 커피가 다 떨어지면 while문을 멈추게 하고 "판매중지"란 문구를 보인다


```python
int coffee = 15;
while (coffee > 0){
	System.out.println(coffee +"돈을 받으면 커피를 주세요");
	coffee--;

	if(coffee == 0){
		System.out.println("판매중지");	
		break;
	} 
}
```

## continue  
while문 조건문으로 돌아가기
- while문 안의 문장을 수행 할 때, 어떤 조건을 검사해서 조건에 맞지 않는 경우, while문의 맨 처음 조건문으로 돌아가게 한다


- 예
    - 1부터 10까지의 수중에서 홀수만을 출력


```python
int num = 0;
while(num < 9) {
    
    num++;
    
    if(num % 2 == 0) {
        continue; // 해당 조건 일 때 조건문의 처음으로 돌아간다
                        
    }
    System.out.println(num);
}		  
```
