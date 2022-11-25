# markdown

장점

1 - 간결하다
2 - 별도의 도구없이 작성가능하다
3 - 다양한 형태로 변환이 가능하다
4 - 텍스트 ( Text ) 로 저장되기 때문에 용량이 적어 보관이 용이하다
5 - 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다
6 - 지원하는 프로그램과 플랫폼이 다양하다
7 - 문법이 쉽다
8 - 관리가 쉽다
9 - 지원 가능한 플랫폼과 프로그램이 다양하다

단점

1 - 표준이 없다
2 - 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다
3 - 모든 HTML 마크업을 대신하지 못한다

#마크다운 사용법

1 - 헤더 ( Headers )

큰제목 : 문서 제목

```
JO YURI
=============
```

JO YURI
=============


작은제목: 문서 부제목

```
JO YURI
-------------
```

JO YURI
-------------

글머리: 1~6까지만 지원

```
# JO YURI
## JO YURI
### JO YURI
#### JO YURI
##### JO YURI
###### JO YURI
```

# JO YURI
## JO YURI
### JO YURI
#### JO YURI
##### JO YURI
###### JO YURI

이메일에서 사용하는 ```>``` 블럭인용문자를 이용한다.

2 - BlockQuote

```
> JO YURI
>	> JO YURI
>	>	> JO YURI
```

> JO YURI
>	> JO YURI
>	>	> JO YURI

이 안에서는 다른 마크다운 요소를 포함할 수 있다

3 - 목록
순서있는 목록 ( 번호 )
순서있는 목록은 숫자와 점을 사용한다

```
1. 첫번째
2. 두번째
3. 세번째
```

1. 첫번째
2. 두번째
3. 세번째

현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다

```
1. 첫번째
3. 세번째
2. 두번째
```

1. 첫번째
3. 세번째
2. 두번째

순서없는 목록 ( 글머리 기호: ```*``` , ```+``` , ```-```  지원 )
```
* JO YURI
  * JO YURI
    * JO YURI

+ JO YURI
  + JO YURI
    + JO YURI

- JO YURI
  - JO YURI
    - JO YURI
 ```
 
* JO YURI
  * JO YURI
    * JO YURI

+ JO YURI
  + JO YURI
    + JO YURI

- JO YURI
  - JO YURI
    - JO YURI

혼합해서 사용하는 것도 가능하다 ( 내가 선호하는 방식 )

```
* DAY - 1
  - DAY - 2
    + DAY - 3
      + DAY - 4
```

* DAY - 1
  - DAY - 2
    + DAY - 3
      + DAY - 4

4 - 코드
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여 들여쓰지 않은 행을 만날때까지 변환이 계속된다.

4 - 1 들여쓰기

This is a normal paragraph:

    This is a code block.
    
end code block.

실제로 적용해보면,

적용예:

This is a normal paragraph:

    This is a code block.
    
end code block.

한줄 띄어쓰지 않으면 인식이 제대로 안되는 문제가 발생합니다.

```
This is a normal paragraph:
    This is a code block.
end code block.
```

적용예:

This is a normal paragraph:
    This is a code block.
end code block.

적용예:

This is a normal paragraph:

This is a code block.
end code block.

한줄 띄어쓰지 않으면 인식이 제대로 안되는 문제가 발생합니다.

This is a normal paragraph:
    This is a code block.
end code block.
적용예:

This is a normal paragraph: This is a code block. end code block.

2.4.1. 코드블럭
코드블럭은 다음과 같이 2가지 방식을 사용할 수 있습니다:

<pre><code>{code}</code></pre> 이용방식
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>

public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}

코드블럭코드("```") 을 이용하는 방법

```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
깃헙에서는 코드블럭코드("```") 시작점에 사용하는 언어를 선언하여 문법강조(Syntax highlighting)이 가능하다.


```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
2.5. 수평선 <hr/>
아래 줄은 모두 수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 페이지 나누기 용도로 많이 사용한다.

* * *

***

*****

- - -

---------------------------------------
적용예
2.6. 링크
참조링크
[link keyword][id]

[id]: URL "Optional Title here"

// code
Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"
Link: Google

외부링크
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
Link: Google

자동연결
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
외부링크: http://example.com/
이메일링크: address@example.com
2.7. 강조
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
single asterisks
single underscores
double asterisks
double underscores
cancelline
문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.
문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.

2.8. 이미지
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")

