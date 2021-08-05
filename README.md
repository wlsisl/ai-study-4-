# ai-study-4-
4주차 인공지능 스터디

<h2>1.tuple</h2>

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

<h2>2.list</h2>

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
  + 포함 유무 확인('py' in l)   
  + 연결(l=l+[1,2,3,]),반복(l*3)   
  + 포함

- 중첩 list: list에 list를 요소로 포함하여 구성하는 방법

- list 메서드(method)   
  + append(): list 마지막 요소로 값을 추가할 때 사용하는 메서드   
  + insert():원하는 위치에 값을 추가할 때 사용하는 메서드(ex: l.list(3,'땡땡') )   
  + slicing기능을 이용하여 list요소 내용을 변경할 수 있다. 
  + 삭제
    
    1. del명령-> del l[0]  
       indexing이나 slicing을 이용하여 원하는 위치의 값 삭제
       
    2. remove()메서드 -> l.remove(100)
       list에서 지정된 값을 검색해서 삭제
       
       검색할 값이 여러 개인 경우에는 처음 찾은 값만 삭제하는 것이다.
       
       검색 실패시 예외발생   
    
    3. pop()메서드 -> l.pop()
    
       list의 마지막 요소를 삭제
       
       삭제한 값을 반환한다.( print(f'remove data : {value}') )
       자료구조 종류중에 stack(스택)
           LIFO( last in first out,후입선출) 구조의 자료구조   
           한 방향으로 입력과 추력을 수행   
           주로 임ㅇ시 데이터 저장용으로 사용
           
    4. clear()메서드:list전체 삭제   

  + index()   
    1. 데이터 검색하여 index반환   
    2. 중복된 데이터에 대해서는 먼저 검색된 데이터의 index반환   
    3. 검색 실패시 예외 발생 

  + count():원하는 값의 개수 파악하는 메서드   
  + sort(정렬)-> l_sorted=sorted(l)

    1. 데이터를 기준에 따라 순서대로 나열하는 Algorithm   
    2. sort(정렬) Algorithm
         정렬 키: 정렬을 하기 위한 기준 값   
         정렬 방향: 작은 ㅇ값에서 큰값순 정렬(Ascending),큰 값에서 작은값순 정렬(Descending)   
    3. sort()메서드:list전체를 내부적으로 (in place)로 정렬   
    4. sorted()함수: list전체를 정렬한 복사본 반환

   + list복사
    
    1. slicing을 이용한 복사:list 전체를 복사할 때 전체 슬라이싱[:] 방법을 이용하여 복사한다.   
    2. copy()메서드를 이용한 복사   
    3. list()함수를 이용한 복사   
    4. 얕은 복사(shallow copy):중첩 list를 복사할 때 내부의 list id 만 복사되는 경우   
      -> 중첩 list를 복사할 때 내부의 list id만 복사되는 경우   
      -> 일반적인 list복사 방법을 적용할 때 발생
      
    5. 깊은복사(deep copy)
      -> 중첩 list복사할 때 내부의 list가 별도로 복사되는 경우   
      -> copy 모듈의 deepcopy()함수를 사용하여 복사
      
    + list 비교: 비교대상 list의 같은 index내용을 비교하고 비교결과가 다를 때 길이를 가지고 비교 결과를 결정한다. 


   
