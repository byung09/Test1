> # Git 명령어 
&nbsp;

  <dl>
  
  <dt><li> &nbsp; &nbsp; git config --global --unset-all user.email</li></dt>
  <dd>: &nbsp; 전체 사용자 이메일을 삭제하는 명령어로 -all을 빼고 email 옆에 사용자이메일을 입력하면 사용자이메일을 설정하여 <br>삭제하는 명령어. 
  </dd>
  
  <dt><li> &nbsp; &nbsp; git config --global --unset-all user.name</li></dt>
  <dd>: &nbsp; 전체 사용자 이름을 삭제하는 명령어로 -all을 빼고 name옆에 사용자이름을 입력하면 사용자이름을 설정하여 삭제하는 명령어. 
  </dd>
  
  <dt><li> &nbsp; &nbsp; git config - -global - -list</li></dt>
  <dd>: &nbsp; 위에서 설정한 정보가 제대로 삭제 되었는지 리스트확인을 할 수 있는 명령어.
  </dd>
  
  </dl>

---

  <dl>
  
  <dt><li> &nbsp; &nbsp; git init</li></dt>
  <dd>: &nbsp; cd를 이용하여 원하는 폴더로 이동후 폴더 기준으로 git이 활동할 수 있는 영역을 미리 만들어 주기위해 <br>초기화(init)을 한다. 해당 폴더의 터미널에서 git init 명령어로 미리 환경을 구성해준다. 최초 한번만 해주면된다.
  </dd>
  
  <dt><li> &nbsp; &nbsp; ls -al</li></dt>
  <dd>: &nbsp; 제대로 구성이 되었다면 위 명령어를 통해 .git이라는 파일을 확인할 수 있다.</dd>
  
  <dt><li> &nbsp; &nbsp; git clone <저장소url></li></dt>
  <dd>: &nbsp; 말그대로 해당 소스를 그대로 복제해온다는 의미로, git repository 전체를 가져온다
<br>clone과 pull의 차이점은 clone은 git repository전체를 가져오는것이고, pull은 파일만 가져온다는점이다.
  </dd>
  
  </dl>
  
---
  
  <dl>
  <dt><li> &nbsp; &nbsp; git add <파일></li></dt>
  <dd>: &nbsp; 내가 커밋하고 싶은 파일을 지정해서 스테이지에 올리거나 파일을 새로 추적할 때 사용
  </dd>
  </dl>

---

  <dl>
  <dt><li> &nbsp; &nbsp; git commit -m “<메시지>”</li></dt>
  <dd>: &nbsp; add된 txt파일에 대해 변경사항을 적용하고 새로이 저장할 수 있다. git add후 수정을 했다면 commit전에 <br>다시한번 add를 해야 커밋에 수정사항이 반영된다.
  </dd>
  
  <dt><li> &nbsp; &nbsp;git commit -a</li></dt>
  <dd>: &nbsp; 스테이지않된 상태의 파일까지 모두 스테이지 시킨후 함께 커밋한다.
  </dd>
  
  <dt><li> &nbsp; &nbsp; git rm <파일명></li></dt>
  <dd>: &nbsp; git에서 파일을 제거하며, 실제 디렉토리에서도 삭제가된다. 일반적인 방법으로 삭제를하게되면 파일은 삭제되어도 unstage항목에 계속 남아있게된다.
  </dd>
 
  <dt><li> &nbsp; &nbsp; git reset HEAD<파일명></li></dt>
  <dd>: &nbsp; 이미 stage된 파일을 다시 unstage하고싶을 때 사용한다. 
파일을 unstage상태로 변경한다.
  </dd>
  </dl>
  
---
  
  <dl>
  <dt><li> &nbsp; &nbsp; git remote add <원격 저장소> <저장소 url></li></dt>
  <dd>: &nbsp; 원격저장소를 관리할 수 있는 명령어로서, 원격저장소는 기본값이 origin이고 필요에 따라 다른이름을 주면된다. 
remote하기전에는 현재 디렉토리가 init으로 저장소화 되어있어야한다.<br>
순서를 정하자면 init, add, commit, remote, push순으로 볼 수 있다.
  </dd>
    
  <dt><li> &nbsp; &nbsp; git remote -v</li></dt>
  <dd>: &nbsp; remote 저장소가 어디인지를 확인할 수 있다.
  </dd>
  </dl>
  
---

<dl>
  <dt><li> &nbsp; &nbsp; git fetch <원격 저장소></li></dt>
  <dd>: &nbsp; 원격저장소의 소스를 로컬 저장소로 가져오는작업
  </dd>
  
  <dt><li> &nbsp; &nbsp; git pull <원격 저장소></li></dt>
  <dd>: &nbsp; 가져온 모든 commit들을 현재 작업중인 곳으로 집어넣는다. 내가 검토하지않고 commit들을 합해준다. pull을 하게되면 fetch를 한후 merge작업까지 자동으로 실행해주는 것으로 
pull은 자동으로 내가 할 일을 대신 해준다고 생각하면된다.
  </dd>
  
  <dt><li> &nbsp; &nbsp; git push <원격 저장소> <지역 브랜치></li></dt>
  <dd>: &nbsp; 작업을 한 파일을 저장소에 올려주는 역할로 예로 add를 통해 txt파일을 만들다. 만약 추가할려는 파일이 여러개일 경우  " git add. "을 이용한다. 모든파일이 올려지는게 아니라 저장소를 비교했을 때 변동사항이 생긴 파일이나 폴더에 한해서만 업로드된다. 후에 commit을 통해 메시지를 작성하고 push를 이용해 git저장소에 파일을 추가한다.
  </dd>
      
</dl>
<br> 

> # Markdown 문법
&nbsp;

## 1. Headers

<dl><dt><li> &nbsp; &nbsp; 큰제목 ( 문서 제목 ) </li></dt></dl> 

**명령어 &nbsp; ]**

```
This is an H1
=============    
```
    
**결과&nbsp;]**

This is an H1
=============
</br>

<dl><dt><li> &nbsp; &nbsp; 작은제목 ( 문서 부제목 ) </li></dt></dl>

**명령어&nbsp;&nbsp;]**

```
This is an H2
-------------
```
    
**결과  ]**
    
This is an H2
-------------
</br>

<dl><dt><li> &nbsp; &nbsp; 글머리 ( 1~6까지만 지원 ) </li></dt></dl> 

**명령어  ]**

```
# Header1
## Header2
### Header3
#### Header4
##### Header5
###### Header6
```

**결과  ]**

# Header1
## Header2
### Header3
#### Header4
##### Header5
###### Header6
</br>

---

## 2. BlockQuote

**명령어  ]**

```
> blockqute 입니다.

```
**결과  ]**

> blockqute 1개 사용입니다.
>	> blockqute 2개 사용입니다.
>	>	> blockqute 3개 사용입니다.
</br>

<dl><dt><li> &nbsp; &nbsp; blockqute문법안에서는 다른 마크다운 문법를 포함할 수 있다. </li></dt></dl>

**[ 예시 ]**

> ## Header2
> * List
>	```
>	content
>	```
</br>

---

## 3. 목록

<dl><dt><li> &nbsp; &nbsp; 순서있는 목록은 숫자와 점을 사용한다. </li></dt></dl>

**명령어  ]**

```
1. 첫번째 목록
2. 두번째 목록
3. 세번째 목록
```

**결과  ]**

1. 첫번째 목록
2. 두번째 목록
3. 세번째 목록
</br>

<dl><dt><li> &nbsp; &nbsp; 목록의 순서상관없이 순서는 내림차순으로 정의된다. </li></dt></dl>

**[ 예시 ]**

**명령어  ]**

```
1. 첫번째 목록
3. 세번째 목록
2. 두번째 목록
```

**결과  ]**

1. 첫번째 목록
3. 세번째 목록
2. 두번째 목록
</br>

<dl><dt><li> &nbsp; &nbsp; 순서없는 목록 </li></dt></dl>

**명령어  ]**

```
* 목록1
  * 목록2

+ 목록1
  + 목록2

- 목록1
  - 목록2
```

**결과  ]**

* 목록1
  * 목록2

+ 목록1
  + 목록2

- 목록1
  - 목록2
</br>

<dl><dt><li> &nbsp; &nbsp; 목록문법들을 혼합하여 사용해도 적용된다. </li></dt></dl>

**[ 예시 ]**

**명렁어  ]**

```
* 목록1
  - 목록2 
    + 목록3
            
```
**결과  ]**

* 목록1
  - 목록2
    + 목록3
</br>

---

## 4. 수평선
<dl><dt><li> &nbsp; &nbsp; 아래 줄은 모두 수평선을 만든다. 마크다운 문서를 출력할 때 페이지를 나누는 용도로 사용된다. </li></dt></dl>

**문법  ]**

```
* * *

***

*****

- - -

---------------------------------------
```
**결과  ]**

* * *
***
*****
- - -
---------------------------------------
</br>

---

## 5. 링크

<dl><dt><li> &nbsp; &nbsp; 인라인링크 </li></dt></dl>

**문법  ]**
```
[Inline Link](https://www.naver.com/ "This is Link")
```
**결과  ]**

[Inline Link](https://www.naver.com/ "This is Link")

</br>

<dl><dt><li> &nbsp; &nbsp; 참조링크 </li></dt></dl>

**문법  ]**
```
[Reference Link][Link ID]
[Link ID]: http://www.naver.com "THis is second Link."
```
**결과  ]**

[Naver][naverlink]
[naverlink]"http://www.naver.com "THis is second Link."

</br>

<dl><dt><li> &nbsp; &nbsp; 자동연결링크 </li></dt></dl>

**문법  ]**
```
https://www.naver.com/ 문법과 <https://www.naver.com/> 문법은 서로 같은결과를 나타내는 링크문법이다.
```
**결과  ]**

https://www.naver.com/ 문법과 <https://www.naver.com/> 문법은 서로 같은결과를 나타내는 링크문법이다. 

</br>

---

## 6. 구문강조
<dl><dt><li> &nbsp; &nbsp; single backtick을 사용하여 inline comde를 적용할수있다. </li></dt></dl>

**문법  ]**
```
this is `inline code`
```

**결과  ]**

this is `inline code`

</br>

<dl><dt><li> &nbsp; &nbsp; 3개의 backtick을 사용하여 어떤 언어의 코드인지 명시할수있다. </li></dt></dl>

**문법  ]**

```
```javascript
var str = "javascript";
```


**결과  ]**

```javascript
var str = "javascript";
```
</br>

<dl><dt><li> &nbsp; &nbsp; 4 space를 이용하여 3 backtick을 사용한것과 같은결과를 나태낼수있다. </li></dt></dl>

**문법  ]**
```
    this is also code
```

**결과  ]**

    this is also code
</br>

---

## 7. Table
<dl><dt><li> &nbsp; &nbsp;
 
` | `기호와 `---` 기호를 사용하여 테이블을 만들수있다 
  
( `---` 는 반드시 3개 이상이 되어야 구분자로 쓸수있다.)

( `|` 기호는 생략이 가능하며, 다른 강조문법도 사용가능하다. 또한 `:` 기호를 통해 정렬방식을 바꿀수있다.) </li></dt></dl>

**문법  ]**
```
this is table

| Name  | age | level |
|-------|:---:|------:|
| byung | 23  | Lv.96 |
```

**결과  ]**

this is table

| Name  | age | level |
|-------|:---:|------:|
| byung | 23  | Lv.96 |
</br>

---

## 8. HTML코드
<dl><dt><li> &nbsp; &nbsp; HTML코드를 이용할수있다. </li></dt></dl>

**문법  ]**
```
<dl>
  <dt>제목</dt>
  <dd>내용</dd>
</dl>
```

**결과  ]**

<dl>
  <dt>제목</dt>
  <dd>내용</dd>
</dl>
<br>

---

## 9. 라인 분리
<dl><dt><li> &nbsp; &nbsp; 줄바꿈을 하고플때는 Enter키를 2번이상 눌러야한다. 1번 누를시 문장이 이어진다. </li></dt></dl>

**문법  ]**
```
---

Apple1
Apple2

Apple3
```

**결과  ]**

Apple1
Apple2

Apple3

</br>

---

## 10. 글자 강조

**문법  ]**
```
This is *italic* string.
This is _italic_ string.

This is **bold** string.
This is __bold__ string.

This is ~~cancel~~ string.

This is *__combination__*string.
```

**결과  ]**

This is *italic* string.
This is _italic_ string.

This is **bold** string.
This is __bold__ string.

This is ~~cancel~~ string.

This is *__combination__* string.

</br>

---

## 11. 이미지

**문법   ]**
```
![Alt text](/path/to/img.jpg)
```

**결과  ]**

![default](https://user-images.githubusercontent.com/42789897/46569315-6c7dac00-c942-11e8-9cf9-5463c0167972.jpg)
</br>
