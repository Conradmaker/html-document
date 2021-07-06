# &lt;figure&gt;,&lt;iframe&gt;,&lt;script&gt;

## &lt;figure&gt;

는 이미지나 삽화, 도표 등의 영역을 설정.

&lt;figcaption&gt;는&lt;figure&gt; 에 포함되어 이미지나 삽화 등의 설명을 표시한다.

```markup
<figure> 
<img src="milk.jpg" alt="A milk"> 
<figcaption>Milk is a nutrient-rich, white liquid food produced
            by the mammary glands of mammals.</figcaption> </figure>
```

​

## &lt;iframe&gt;

​다른 HTML문서를 페이지 안에 삽입

\(중첩된 브라우저 컨텍스트\(프레임\)를 표시\)

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>&#xC18D;&#xC131;</b>
      </th>
      <th style="text-align:left"><b>&#xC758;&#xBBF8;</b>
      </th>
      <th style="text-align:left"><b>&#xAC12;</b>
      </th>
      <th style="text-align:left"><b>&#x200B;</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">name</td>
      <td style="text-align:left">&#xD504;&#xB808;&#xC784;&#xC758; &#xC774;&#xB984;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">src</td>
      <td style="text-align:left">&#xD3EC;&#xD568;&#xD560; &#xBB38;&#xC11C;&#xC758; URL</td>
      <td style="text-align:left">URL</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">width</td>
      <td style="text-align:left">&#xD504;&#xB808;&#xC784;&#xC758; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">height</td>
      <td style="text-align:left">&#xD504;&#xB808;&#xC784;&#xC758; &#xC138;&#xB85C; &#xB108;&#xBE44;</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">allowfullscreen</td>
      <td style="text-align:left">&#xC804;&#xCCB4; &#xD654;&#xBA74; &#xBAA8;&#xB4DC; &#xC0AC;&#xC6A9; &#xC5EC;&#xBD80;</td>
      <td
      style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">frameborder</td>
      <td style="text-align:left">&#xD504;&#xB808;&#xC784; &#xD14C;&#xB450;&#xB9AC; &#xC0AC;&#xC6A9; &#xC5EC;&#xBD80;</td>
      <td
      style="text-align:left"><b>0</b>, <b>1</b>
        </td>
        <td style="text-align:left"><b>1</b>
        </td>
    </tr>
    <tr>
      <td style="text-align:left">sandbox</td>
      <td style="text-align:left">&#xBCF4;&#xC548;&#xC744; &#xC704;&#xD55C; &#xC77D;&#xAE30; &#xC804;&#xC6A9;&#xC73C;&#xB85C;
        &#xC0BD;&#xC785;</td>
      <td style="text-align:left">
        <p>&#xBD88;&#xB9B0;(Boolean) or</p>
        <p><b>allow-form</b>: &#xC591;&#xC2DD; &#xC81C;&#xCD9C; &#xAC00;&#xB2A5;,</p>
        <p><b>allow-scripts</b>: &#xC2A4;&#xD06C;&#xB9BD;&#xD2B8; &#xC2E4;&#xD589;
          &#xAC00;&#xB2A5; ,</p>
        <p><b>allow-same-origin</b>: &#xAC19;&#xC740; &#xCD9C;&#xCC98;(&#xB3C4;&#xBA54;&#xC778;)&#xC758;
          &#xB9AC;&#xC18C;&#xC2A4; &#xC0AC;&#xC6A9; &#xAC00;&#xB2A5;</p>
      </td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

```markup
<iframe width="900"        //가로
        height="720"       //높이
        src="https://youtu.be/0NRekDwcQU4" 
        frameborder="1"    //프레임의 유무
        allowfullscreen>   //전체화면
 </iframe>
```



## **&lt;canvas&gt;**

[Canvas API](https://developer.mozilla.org/ko/docs/Web/HTML/Canvas)이나 [WebGL API](https://developer.mozilla.org/ko/docs/Web/API/WebGL_API)를 사용하여 그래픽이나 애니메이션을 랜더링.

| **속성** | **의미** |
| :--- | :--- |
| width | 캔버스의 가로 너비 |
| height | 캔버스의 세로 너비 |

```markup
<canvas id="myCanvas" width="200" height="100"></canvas>
```

_\*이상태는 공간만 만들어준 상태이다\*_

_\*자바스크립트를 통해 공간을 채워야한다\*_

\_\_

## &lt;script&gt;

​스크립트 코드를 문서에 포함 or 참조

| **속성** | **의미** | **값** | **특징** |
| :--- | :--- | :--- | :--- |
| async | 스크립트의 비동기적\(Asynchronously\) 실행 여부 | 불린\(Boolean\) | **src** 속성 필수 |
| defer | 문서 파싱\(구문 분석\) 후 작동 여부 | 불린\(Boolean\) | **src** 속성 필수 |
| src | 참조할 외부 스크립트 URL | URL | 포함된 스크립트 코드는 무시됨 |
| type | [MIME 타입](https://developer.mozilla.org/ko/docs/Web/HTTP/Basics_of_HTTP/MIME_types) | **text/javascript**\(기본값\) |  |

### defer속성

\*html문서는 위에서 아래로 순서대로 해석하기때문에

 위에서 script를 실행하면 아래의 내용을 읽지 않은 상태가 된다.

 그렇게 되면 오류가 발생할 수 있는데 이때 ​defer속성을 사용하면

 html문서 전체를 해석한 후 script를 실행하게 한다.\*

### 

### &lt;noscript&gt;

​스크립트가 실행할 수 없는 환경에 사용

\*&lt;iframe&gt;에서 sandbox를 사용할 경우 script지원을 막을 수 있다.\*

 이때 script가 실행되지 않을때 나타낼 내용을 지정하는 태그이다.

​

