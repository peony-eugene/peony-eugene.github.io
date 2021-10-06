---
layout: single
categories: java
toc: true
---

# 제어문
## switch/case 문
- **입력 변수**의 값과 일치하는 **case입력값**이 있다면 해당 case하위 문장이 실행됨.
- case문마다 break문이 있는데, 해당 case문을 실행 한 후 switch문을 빠져나간다. 만약 break문이 없으면 그 다음 case문이 실행된다


```python
switch(입력변수){
    case 입력값1:...
        break;
    case 입력값2:...
        break;
    ...
    default: ...
        break;
}
```

- 예시   
    - switch문의 입력으로 month값에 1이라는 숫자가 올 경우 January라는 문자열이, 12가 입력으로 올 경우 December라는 문자열이 출력된다.
    아래 예제는 month가 8로 고정되어 있어 August라는 문자열이 출력된다
    - 이렇게 입력값이 정형화된 경우 if문보다 switch/case문이 가독성이 더 좋다


```python
# SwitchDemo.java

public class SwitchDemo {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int month = 8;
		String monthString = "";
		switch (month) {
			case 1: monthString = "January";
					break;
			case 2: monthString = "February";
					break;
			case 3: monthString = "March";
					break;
			case 4: monthString = "April";
					break;
			case 5: monthString = "May";
					break;
			case 6: monthString = "June";
					break;
			case 7: monthString = "July";
					break;
			case 8: monthString = "August";
					break;
			case 9: monthString = "September";
					break;
			case 10:monthString = "October";
					break;
			case 11:monthString = "November";
					break;
			case 12:monthString = "December";
					break;
			default:monthString = "Invalid month";
					break;		
		}
		System.out.println(monthString);
	}
}
```
