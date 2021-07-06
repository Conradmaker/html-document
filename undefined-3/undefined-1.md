# 표 콘텐츠

## &lt;table&gt;,&lt;tr&gt;,&lt;th&gt;,&lt;td&gt;

​&lt;table&gt; 태이블 표를 만들때 사용        **table** **{** **display: table; }**

&lt;tr&gt; 행\(줄\)을 만들때 사용                     **tr** **{** **display: table-row; }**

&lt;th&gt; 제목                                                 **th,** **td** **{** **display: table-cell; }**

&lt;td&gt; 데이터을 만들때 사용                    &gt;블록요소와 유사한 특성을 가진다.

```markup
<table>                 //표영역
  <tr>                  //1줄
    <th>타입</th>        //header
    <th>값</th>
  </tr>
  <tr>                  //2줄
    <td>알파벳</td>      //data
    <td>A</td>
  </tr>
  <tr>
   <td>숫자</td>
   <td>2</td>
  </tr>
</table>
```

### \*\*\*\*

### **&lt;th&gt;**

‘머리글 칸’을 지정

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>&#xC18D;&#xC131;</b>
      </th>
      <th style="text-align:left"><b>&#xC758;&#xBBF8;</b>
      </th>
      <th style="text-align:left"><b>&#xAC12;</b>
      </th>
      <th style="text-align:left"><b>&#xAE30;&#xBCF8;&#xAC12;</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">abbr</td>
      <td style="text-align:left">&#xC5F4;&#xC5D0; &#xB300;&#xD55C; &#xAC04;&#xB2E8;&#xD55C; &#xC124;&#xBA85;</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">headers</td>
      <td style="text-align:left">&#xAD00;&#xB828;&#xB41C; &#xD558;&#xB098; &#xC774;&#xC0C1;&#xC758; &#xB2E4;&#xB978;
        &#xBA38;&#xB9AC;&#xAE00; &#xCE78; <b>id</b> &#xC18D;&#xC131; &#xAC12;</td>
      <td
      style="text-align:left"></td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">colspan</td>
      <td style="text-align:left">&#xD655;&#xC7A5;&#xD558;&#xB824;&#xB294;(&#xBCD1;&#xD569;) &#xC5F4;&#xC758;
        &#xC218; (2&#xBA74; 2&#xCE78;&#xBCD1;&#xD569;)</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"><b>1</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">rowspan</td>
      <td style="text-align:left">&#xD655;&#xC7A5;&#xD558;&#xB824;&#xB294;(&#xBCD1;&#xD569;) &#xD589;&#xC758;
        &#xC218; (2&#xBA74; 2&#xCE78;&#xBCD1;&#xD569;)</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"><b>1</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">scope</td>
      <td style="text-align:left">&#xC790;&#xC2E0;&#xC774; &#xB204;&#xAD6C;&#xC758; &#x2018;&#xBA38;&#xB9AC;&#xAE00;
        &#xCE78;&#x2019;&#xC778;&#xC9C0; &#xBA85;&#xC2DC;</td>
      <td style="text-align:left">
        <p><b>col</b>: &#xC790;&#xC2E0;&#xC758; &#xC5F4;</p>
        <p><b>colgroup</b>: &#xBAA8;&#xB4E0; &#xC5F4;</p>
        <p><b>row</b>: &#xC790;&#xC2E0;&#xC758; &#xD589;</p>
        <p><b>rowgroup</b>: &#xBAA8;&#xB4E0; &#xD589;</p>
        <p><b>auto</b>
        </p>
      </td>
      <td style="text-align:left"><b>auto</b>
      </td>
    </tr>
  </tbody>
</table>

```markup
<tr>
  <th colspan="2" id="th-data">데이터</th> //2칸을 차지(병합)
</tr>

<tr>                 
  <th abbr="type" headers="th-data">타입</th> //부가설명,ID에 종속되는 표이다. 
  <th abbr="value" headers="th-data">값</th>
</tr>
```

\*_과거에는 테이블로 레이아웃을 구성하기도 하였지만 현재는 하지말자!\*_

\_\_

### **&lt;caption&gt;** __**{** **display: table-caption; }**

​표의 제목을 설정. 

 -열리는 TABLE 태그 바로 다음에 작성해야 함.

 -&lt;table&gt; 당 하나의 &lt;caption&gt;만 사용 가능.



###  

### **colgroup** **{** **display: table-column-group; }**

### **col** **{** **display: table-column; }**

 표의 열들을 공통적으로 정의하는 컬럼\(**&lt;col&gt;**\)과 그의 집합\(**&lt;colgroup&gt;**\).



```markup
<table>
        <caption>데이터 타입과 값</caption> //항상 태이블태그 아래
        <colgroup>
            <col style="background-color: blue;"> //1번째 줄에 스타일 적용
            <col style="background-color: blue;" span="2"> //여기부터 2줄 적용
        </colgroup>
        <tr>
            <th></th>
            <th>타입</th>
            <th>값</th>
        </tr>
        <tr>
            <th>1</th>
            <td>알파벳</td>
            <td>A</td>
        </tr>
        <tr>
            <th>2</th>
            <td>숫자</td>
            <td>2</td>
        </tr>
</table>
```

​

### ​**&lt;thead&gt;, &lt;tbody&gt;, &lt;tfoot&gt;**

​표의 머리글\(**&lt;thead&gt;**\), 본문\(**&lt;tbody&gt;**\), 바닥글\(**&lt;tfoot&gt;**\)을 지정.

_\*테이블의 레이아웃에 영향을 주지 않는다.\*_

```markup
<table>
        <caption>Fruits</caption>
        <colgroup>
            <col span="2" style="background-color: yellowgreen;"> //1번부터 2개 적용
            <col style="background-color: tomato;"> //3번줄 적용
        </colgroup>
        <thead>
            <tr>
                <th>ID</th>
                <th>Name</th>
                <th>Price</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>F123A</td>
                <td>Apple</td>
                <td>$22</td>
            </tr>
            <tr>
                <td>F098B</td>
                <td>Banana</td>
                <td>$19</td>
            </tr>
        </tbody>
</table>
```

![&#xC774;&#xB7F0; &#xACB0;&#xACFC;&#xAC00; &#xB098;&#xC628;&#xB2F5;&#xB2C8;&#xB2E4;](../.gitbook/assets/image%20%285%29.png)

