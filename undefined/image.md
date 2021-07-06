# Image

## **&lt;img /&gt;**

​이미지를 삽입하는 태그

| **속성** | **의미** | **값** |  |
| :--- | :--- | :--- | :--- |
| src | \(필수\)이미지 URL | URL |  |
| alt | \(필수\)이미지의 대체텍스트 |  |  |
| width | 이미지의 가로 너비 |  |  |
| height | 이미지의 세로 너비 |  |  |
| srcset | 브라우저에게 제시할 이미지 URL과 원본 크기의 목록을 정의 | **w**, **x** |  |
| sizes | 미디어 조건과 해당 조건일 때 이미지 최적화 크기의 목록을 정의 |  |  |

 \*크기를 조절할때는 weight/height 둘중하나만 사용 추천! \(비율유지\)\*

 srcset,sizes속성은 반응형웹을 만들때 사용



### **srcset 속성**

​반응형 웹에 맞에 브라우저가 사용할 이미지 후보의 경로와 원본의 크기를 명시

-사용할 이미지를 사이즈별로 2장이상 준비하여 srcset 속성에 작성.

 \*이미지크기는 px가 아닌 w/x단위 입력

 \*작은사이즈에서 큰사이즈로 명시

 \*브라우저는 최적화 이미지를 찾을때 이미지를 늘리는것보다 축소한다

 \*고정된 이미지 크기를 유지하려면 width속성 추가한다

w : 가로너비를 의미한다.

 ex\) 400x300px의 w 값은 400w이다.

```markup
<img srcset="images/123_small.png 400w,

                         images/123_medium.png 700w, 

                         images/123_large.png 1000w"

               src="images/123.png" 

               alt="123" />
```

\*\*\*\*

### **sizes 속성**

미디어조건과 그 조건에 해당하는 이미지의 '최적화 출력크기'를 지정

```markup
<img srcset="images/123_small.png 400w,

                         images/123_medium.png 700w, 

                         images/123_large.png 1000w"

              sizes="(min-width: 1000px) 700px"

               src="images/123.png" 

               alt="123" />
```

위 예제의 결과로,

뷰포트 너비가 400px 이하일 때 **123\_small.png**\(400px\)가 사용됩니다.

뷰포트 너비가 401~700px 일 때 **123\_medium.png**\(700px\)가 사용됩니다.

뷰포트 너비가 701~999px 일 때 **123\_large.png**\(1000px\)가 사용됩니다.

뷰포트 너비가 1000px 이상일 때**123\_medium.png**\(700px\)가 사용됩니다.



width: 이미지의 '출력크기'만 지정한다.

sizes: 이미지의 ‘출력 크기’ + ‘최적 크기’도 함께 지정

​

_\*srcset/sizes는 IE를 지원하지 않음\*_

