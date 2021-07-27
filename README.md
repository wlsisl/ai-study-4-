# ai-study-4-
4주차 인공지능 스터디

<h4>tuple</h4>

t라는 이름의 tuple을 생성하면 t=(1,10.5,'python')으로 저장할 수 있다. 즉 여러값을 저장할 수 있는데 그 타입은 정수, 실수 , 문자 모두 혼합해서 저장하는 것이 가능하다. 

 + tuple은 불변(immutable)자료형이므로 초기에 tuple에 저장된 값에 대한 변경, 삭제, 값 추가 동작이 모두 불가능하다.   
 + sequence자료형 공통 연산 - tuple


- indexing을 이용한 tuple요소 읽기
 + indecing: tuple요소(원소)에 대한 읽기 수행. tuple은 불변 자료형이므로 indexing을 통한 tuple요소에 대한 쓰기는 불가능

  t[0], type(t[0])  
  > 위 t=(1,10.5,'python')에서 0에는 1이 저장되어 있겠고 그 type은 int 즉 정수이다.

- slicing:tuple부분 요소 읽기   
- 길이계산:len()함수   
- 포함 유무 확인: in연산   
- 연결   
- 반복   

- 중첩 tuple   
 + tuple의 요소가 tuple인 형태   
 + 중첩 tuple을 구성한 경우 tuple의 요소가 tuple이므로 indexing을 중첩해서 사용해야한다.   
 
- tuple메서드   
 + count()메서드:원하는 값의 개수 확인   
 + index()메서드:원하는 값의 위치값 확인   

- tuple을 이용하여 여러값을 변수에 치환   
- tuple을 이용한 두 변수의 내용 교환   
- tuple을 이용한 packing과 unpacking   
 + packing:하나의 변수에 여러값을 저장하는 방법   
 + unpacking:하나의 변수의 내용을 여러 변수에 나누어 저장하는 방법   
 + 확장 기능을 이용한 unpacking:변수에 '(asterisk)기호를 붙이면 tuple에 포함된 데이터 개수와 상관없이 unpacking가능   

- tuple비교:tuple간의 비교는 크기 비교가 아니고 원소의 수 (길이)비교   

> t1,t2,t3를 지정하고 f1>t2 처럼 관계연산자를 사용하여 참 거짓을 출력하는 것

- tuple도 반복자(literator)를 포함하고 있다.  

<h4>2.list</h4>

- 여러 값을 저장하는 sequence자료형   
- list는 **가변(mutable) 자료형**   
- list는 파이썬 스크립트 작성시 가장 많이 활용하는 sequence자료형  
- list생성 방법   
  + [] 대괄호를 이용하여 생성   
  + list()함수를 이용한 생성   
 
- sequence자료형 공통 연산- list  
  + indexing   
  + slicing   
  + 길이 계산   
  + 포함 유무 확인   
  + 연결   
  + 포함

- 
