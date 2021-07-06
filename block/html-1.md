# 콘탠츠 영역 HTML태그

### **header** **{** **display: block; }**

header/Footer는 태그 안에 &lt;addrss&gt;,&lt;header&gt;&lt;footer&gt;태그를 사용할 수 없다.

&lt;div&gt;는 의미를 가지지 않는 태그이지만 &lt;header&gt;,&lt;footer&gt;태그들은 의미를 가지고 있다

​ 의미를 가지는 태그들은 브라우저 내에서 해석됨.



###  **h1,** **h2,** **h3,** **h4,** **h5,** **h6** **{** **display: block; }**

&lt;h1&gt;~&lt;h6&gt;요소는 6단계의 문서 제목을 구현한다.

\#\# 제목폰트의 크기를 줄이기 위해 낮은 단계를 사용하면 안된다!!!

     &gt;&gt;&gt;대신css이용해서 font-size를 조정하자!

 because 브라우저가 h1부터 순차적으로 정보를 찾기 때문에 정보가 건너뛰어질 수 있다.

 h1태그는 1페이지 1개씩 써주는게 better

1.h1

   1.h2

   2.h2

      1.h3

   3.h2                요런식으로 말이다.

###  

### **main** **{** **display: block; }**

&lt;main&gt;태그는 &lt;body&gt;의 주요내용을 나타낸다.

&lt;base&gt;태그처럼 1문서에 1개의 태그만 사용해야 한다.

\*IE 지원 불가\*

### 

###  **article** **{** **display: block; }**

독립적으로 구분되거나 재사용 가능한 영역

 안에&lt;h1&gt;태그가 사용되있다

주로 기사나 블로그글 같은 부분

\*독립적으로 나가서 재사용되도 작동하여야 한다\*

###  

### section **{** **display: block; }**

문서의 일반적인 영역을 설정

article과 마찬가지로 &lt;h&gt;를 포함하여 식별

section안에 article이, article안에 section이 있을수도 있다.

 div는 의미가 없는 태그이지만 section,article은 제목부터해서 의미를 가지고 있음.

\*쉽게말해 의미의 강도는 article &gt; section &gt; div 라고 봐도 무방함

###  

### aside **{** **display: block; }**

문서의 별도 콘텐츠를 설정 \(광고나, 링크\)

###  

### nav **{** **display: block; }**

다른 페이지 링크를 제공하는 영역을 설정

\(Navigation, 보통 메뉴를 구성한다\)

```markup
<nav>

  <a href="/html/">HTML</a> |

  <a href="/css/">CSS</a> |

  <a href="/js/">JavaScript</a> |

  <a href="/jquery/">jQuery</a>

</nav>

​
```

###  

### address **{** **display: block; }**

 **&lt;body&gt;**, **&lt;article&gt;**, **&lt;footer&gt;** 등에서 연락처 정보를 제공하기 위해 포함하여 사용.

사용자의 환경에 맞게 링크가 넘어간다.

```markup
<address>

<a href="mailto:jim@rock.com">jim@rock.com</a><br>

<a href="tel:+13115552368">(311) 555-2368</a>

</address>
```

###  

### **div** **{** **display: block; }**

본질적으로는 아무것도 나타내지 않는 콘텐츠 영역을 설정\(Division\)

꾸미는 목적으로 자주 사용

   









