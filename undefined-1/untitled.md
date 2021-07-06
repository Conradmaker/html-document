# 전역속성 정리

## **class**

공백으로 구분된 요소의 별칭을 지정.

CSS 혹은 JavaScript의 요소 선택기\([CSS 선택자](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_%EC%84%A0%ED%83%9D%EC%9E%90)나 [GetElementsByClassName](https://developer.mozilla.org/ko/docs/Web/API/Document/getElementsByClassName), [QuerySelectorAll](https://developer.mozilla.org/ko/docs/Web/API/Document/querySelectorAll) 같은\)를 통해서 요소를 선택하거나 접근.

\*중복가능\*  


## **id**

문서에서 고유한 식별자\(idenifier, ID\)를 정의.

CSS 혹은 JavaScript의 요소 선택기\([CSS 선택자](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_%EC%84%A0%ED%83%9D%EC%9E%90)나 [GetElementsByClassName](https://developer.mozilla.org/ko/docs/Web/API/Document/getElementsByClassName), [QuerySelectorAll](https://developer.mozilla.org/ko/docs/Web/API/Document/querySelectorAll) 같은\)를 통해서 요소를 선택하거나 접근.

\*중복불가\*

\*\*\*\*

## **style**

요소에 적용할 CSS를 선언.



## **title**

요소의 정보\(설명\)을 지정.

\( 커서를 올려놓았을때 나타나는 정보\)

```markup
<p><abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
<p title="Free Web tutorials">W3Schools.com</p>
```



## **lang**

요소의 언어\([ISO 639-1](https://ko.wikipedia.org/wiki/ISO_639-1_%EC%BD%94%EB%93%9C_%EB%AA%A9%EB%A1%9D)\)를 지정.

```markup
<p lang="en">This paragraph is English</p>
<p lang="ko">이 단락은 한글입니다.</p> 
<p lang="fr">Ce paragraphe est défini en français.</p>
```

\*\*\*\*

## **data-\***

사용자 정의 데이터 속성을 지정.

HTML에 JavaScript에서 이용할 수 있는 데이터\(정보\)를 저장하는 용도로 사용.

```markup
<!-- data-custom-data-attributes --> 

<div id="me" data-my-name="conrad" data-my-age="25">conrad</div>

// dataset.customDataAttributes
 const $me = document.getElementById('me');
 console.log($me.dataset.myName); // "conrad"
 console.log($me.dataset.myAge);    // "25"
```



## **draggable**

요소가 [Drag and Drop API](https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API)를 사용 가능한지 여부를 지정.

_명시하지 않으면 auto값을 가진다_

```markup
<div draggable="true">The element to drag.</div>
```



## **hidden**

요소를 숨김.

```markup
<form id="hidden-form" action="/form-action" hidden> 

<!-- 숨겨진 양식들.. -->
</form> 
<button form="hidden-form" type="submit">전송</button>
```



## **tabindex**

**Tab**키를 이용해 요소를 순차적으로 포커스 탐색할 순서를 지정.

[대화형 콘텐츠\(Interactive Content\)](https://developer.mozilla.org/ko/docs/Web/Guide/HTML/%EC%BB%A8%ED%85%90%ED%8A%B8_%EC%B9%B4%ED%85%8C%EA%B3%A0%EB%A6%AC#%EB%8C%80%ED%99%94%ED%98%95_%EC%BD%98%ED%85%90%EC%B8%A0)는 기본적으로 코드 순서대로 탭 순서가 지정됨.

비대화형 콘텐츠에 **tabindex="0"**을 지정하여 대화형 콘텐츠와 같이 탭 순서를 사용.

**tabindex="-1"**을 통해 포커스는 가능하지만 탭 순서에서 제외 가능.

**tabindex="1"** 이상의 양수 값은 논리적 흐름을 방해하기 때문에 사용을 추천하지 않음.

```markup
<h1 tabindex="0">Sign In</h1> 
<label>Username: <input type="text"></label>
<label>Password: <input type="password"></label> 
<label>PS: <input type="text" tabindex="-1"></label>
<input type="submit" value="Sign In">
```



##  **기타 속성들**

\*\*\*\*

<table>
  <thead>
    <tr>
      <th style="text-align:center"><b>&#xC0AC;&#xC6A9; &#xD0DC;&#xADF8;</b>
      </th>
      <th style="text-align:center"><b>&#xC18D;&#xC131;</b>
      </th>
      <th style="text-align:left"><b>&#xC758;&#xBBF8;</b>
      </th>
      <th style="text-align:center"><b>&#xAC12;</b>
      </th>
      <th style="text-align:center"><b>&#xD2B9;&#xC9D5;</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;link /&gt;</b>,</p>
        <p><b>&lt;a&gt;</b>
        </p>
      </td>
      <td style="text-align:center">hreflang</td>
      <td style="text-align:left">&#xD604;&#xC7AC; &#xD398;&#xC774;&#xC9C0;&#xC758; &#xB300;&#xCCB4; &#xC5B8;&#xC5B4;(
        <a
        href="https://ko.wikipedia.org/wiki/ISO_639-1_%EC%BD%94%EB%93%9C_%EB%AA%A9%EB%A1%9D">ISO 639-1</a>)</td>
      <td style="text-align:center"><b>ko</b>, <b>en</b>&#x2026;</td>
      <td style="text-align:center"><a href="https://moz.com/learn/seo/hreflang-tag">&#xB2E4;&#xB978; &#xC5B8;&#xC5B4; &#xB610;&#xB294; &#xC9C0;&#xC5ED;&#xBCC4; &#xC5EC;&#xB7EC; &#xBC84;&#xC804;&#xC758; &#xD398;&#xC774;&#xC9C0;&#xAC00; &#xC788;&#xB294; &#xACBD;&#xC6B0;</a>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;ol&gt;</b>
      </td>
      <td style="text-align:center">reversed</td>
      <td style="text-align:left">&#xD56D;&#xBAA9;&#xC744; &#xC5ED;&#xC21C;&#xC73C;&#xB85C; &#xC124;&#xC815;</td>
      <td
      style="text-align:center"></td>
        <td style="text-align:center">IE &#xC9C0;&#xC6D0; &#xBD88;&#xAC00;</td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;link&gt;</b>,</p>
        <p><b>&lt;img /&gt;</b>,</p>
        <p><b>&lt;video&gt;</b>,</p>
        <p><b>&lt;script&gt;</b>
        </p>
      </td>
      <td style="text-align:center">crossorigin</td>
      <td style="text-align:left">&#xAC00;&#xC838; &#xC624;&#xAE30;&#xAC00; <a href="https://developer.mozilla.org/ko/docs/Web/HTTP/Access_control_CORS">CORS</a>&#xB97C;
        &#xC0AC;&#xC6A9;&#xD558;&#xC5EC; &#xC218;&#xD589;&#xB418;&#xC5B4;&#xC57C;&#xD558;&#xB294;&#xC9C0;
        &#xC5EC;&#xBD80;</td>
      <td style="text-align:center">
        <p><b>anonymous</b>,</p>
        <p><b>use-credentials</b>
        </p>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;img /&gt;</b>
      </td>
      <td style="text-align:center">ismap</td>
      <td style="text-align:left">&#xC11C;&#xBC84; &#xCE21; &#xC774;&#xBBF8;&#xC9C0; &#xB9F5;&#xC73C;&#xB85C;
        &#xC9C0;&#xC815;&#xD574; &#xD074;&#xB9AD;&#xD558;&#xC5EC; &#xC88C;&#xD45C;&#xB97C;
        <a
        href="https://en.wikipedia.org/wiki/Query_string">&#xCFFC;&#xB9AC;&#xC2A4;&#xD2B8;&#xB9C1;</a>&#xC73C;&#xB85C; &#xC11C;&#xBC84;&#xC5D0;
          &#xC804;&#xC1A1;&#xD560;&#xC9C0; &#xC5EC;&#xBD80;</td>
      <td style="text-align:center">&#xBD88;&#xB9B0;(Boolean)</td>
      <td style="text-align:center"><b>&lt;img /&gt;</b>&#xAC00; &#xC720;&#xD6A8;&#xD55C; <b>href</b> &#xC18D;&#xC131;&#xC744;
        &#xAC00;&#xC9C4; <b>&lt;a&gt;</b>&#xC758; &#xD558;&#xC704; &#xC694;&#xC18C;&#xC778;
        &#xACBD;&#xC6B0;&#xC5D0;&#xB9CC; &#xD5C8;&#xC6A9;</td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;img /&gt;</b>
      </td>
      <td style="text-align:center">usemap</td>
      <td style="text-align:left">&#xD074;&#xB77C;&#xC774;&#xC5B8;&#xD2B8; &#xCE21; &#xC774;&#xBBF8;&#xC9C0;
        &#xB9F5;&#xC73C;&#xB85C; &#xC9C0;&#xC815;</td>
      <td style="text-align:center"><b>&lt;map&gt;</b>&#xC758; <b>#</b> + <b>name</b> &#xC18D;&#xC131; &#xAC12;</td>
      <td
      style="text-align:center"><b>&lt;a&gt;</b>, <b>&lt;button&gt;</b>&#xC758; &#xD558;&#xC704; &#xC694;&#xC18C;&#xC778;
        &#xACBD;&#xC6B0; &#xC0AC;&#xC6A9; &#xBD88;&#xAC00;</td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;form&gt;</b>
      </td>
      <td style="text-align:center">accept-charset</td>
      <td style="text-align:left">&#xC11C;&#xBC84;&#xAC00; &#xBC1B;&#xC744; <a href="https://www.iana.org/assignments/character-sets/character-sets.xhtml">&#xBB38;&#xC790;&#xC778;&#xCF54;&#xB529; &#xBC29;&#xC2DD;</a>
      </td>
      <td style="text-align:center"><b>UTF-8</b>, <b>EUC-KR</b>&#x2026;</td>
      <td style="text-align:center"><b>UNKNOWN</b>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;form&gt;</b>
      </td>
      <td style="text-align:center">enctype</td>
      <td style="text-align:left"><b>method</b>&#xC18D;&#xC131;&#xC774; <b>POST</b>&#xC77C; &#xACBD;&#xC6B0;,
        &#xC11C;&#xBC84;&#xB85C; &#xC804;&#xC1A1;&#xD558;&#xB294; &#xCF58;&#xD150;&#xCE20;&#xC758;
        <a
        href="https://developer.mozilla.org/ko/docs/Web/HTTP/Basics_of_HTTP/MIME_types">MIME &#xD0C0;&#xC785;</a>
      </td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;input /&gt;</b>
      </td>
      <td style="text-align:center">accept</td>
      <td style="text-align:left">&#xC11C;&#xBC84;&#xAC00; &#xBC1B;&#xC744; &#xD30C;&#xC77C; &#xC885;&#xB958;</td>
      <td
      style="text-align:center">
        <p>&#xD30C;&#xC77C; &#xD655;&#xC7A5;&#xC790;(<b>.jpg</b>, <b>.png</b>..),</p>
        <p><a href="https://developer.mozilla.org/ko/docs/Web/HTTP/Basics_of_HTTP/MIME_types">MIME &#xD0C0;&#xC785;</a>,</p>
        <p><b>audio/*</b>,</p>
        <p><b>video/*</b>,</p>
        <p><b>image/*</b>
        </p>
        </td>
        <td style="text-align:center"><b>type=&quot;file&quot;</b>
        </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;input /&gt;</b>
      </td>
      <td style="text-align:center">width</td>
      <td style="text-align:left">&#xC774;&#xBBF8;&#xC9C0;&#xC758; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td
      style="text-align:center">&#xC22B;&#xC790;(Number)</td>
        <td style="text-align:center"><b>type=&quot;image&quot;</b>
        </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;input /&gt;</b>
      </td>
      <td style="text-align:center">height</td>
      <td style="text-align:left">&#xC774;&#xBBF8;&#xC9C0;&#xC758; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td
      style="text-align:center">&#xC22B;&#xC790;(Number)</td>
        <td style="text-align:center"><b>type=&quot;image&quot;</b>
        </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;button&gt;</b>
        </p>
      </td>
      <td style="text-align:center">formaction</td>
      <td style="text-align:left">&#xC591;&#xC2DD;&#xC744; &#xC81C;&#xCD9C;&#xD560; &#xB54C; &#xC591;&#xC2DD;
        &#xB370;&#xC774;&#xD130;&#xB97C; &#xBCF4;&#xB0BC; &#xC704;&#xCE58;</td>
      <td
      style="text-align:center">URL</td>
        <td style="text-align:center">
          <p><b>type=&quot;submit&quot;</b>,</p>
          <p><b>type=&quot;image&quot;</b>,</p>
          <p><b>form</b>&#xC758; &#xC18D;&#xC131;&#xBCF4;&#xB2E4; &#xC6B0;&#xC120;</p>
        </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;button&gt;</b>
        </p>
      </td>
      <td style="text-align:center">formenctype</td>
      <td style="text-align:left">&#xC591;&#xC2DD; &#xB370;&#xC774;&#xD130;&#xB97C; &#xC11C;&#xBC84;&#xB85C;
        &#xBCF4;&#xB0B4;&#xAE30; &#xC804;&#xC5D0; &#xC778;&#xCF54;&#xB529; &#xD560;
        &#xBC29;&#xBC95;&#xC744; &#xC9C0;&#xC815;</td>
      <td style="text-align:center">-</td>
      <td style="text-align:center">
        <p><b>type=&quot;submit&quot;</b>,</p>
        <p><b>type=&quot;image&quot;</b>,</p>
        <p><b>form</b>&#xC758; &#xC18D;&#xC131;&#xBCF4;&#xB2E4; &#xC6B0;&#xC120;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;button&gt;</b>
        </p>
      </td>
      <td style="text-align:center">formmethod</td>
      <td style="text-align:left">&#xC591;&#xC2DD; &#xB370;&#xC774;&#xD130;&#xB97C; &#xBCF4;&#xB0B4;&#xB294;
        &#xBC29;&#xBC95;</td>
      <td style="text-align:center"><b>GET</b>, <b>POST</b>
      </td>
      <td style="text-align:center">
        <p><b>type=&quot;submit&quot;</b>,</p>
        <p><b>type=&quot;image&quot;</b>,</p>
        <p><b>form</b>&#xC758; &#xC18D;&#xC131;&#xBCF4;&#xB2E4; &#xC6B0;&#xC120;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;button&gt;</b>
        </p>
      </td>
      <td style="text-align:center">formnovalidate</td>
      <td style="text-align:left">&#xC591;&#xC2DD; &#xB370;&#xC774;&#xD130;&#xC758; &#xC720;&#xD6A8;&#xC131;&#xC744;
        &#xAC80;&#xC0AC;&#xD558;&#xC9C0; &#xC54A;&#xB3C4;&#xB85D; &#xC9C0;&#xC815;</td>
      <td
      style="text-align:center">&#xBD88;&#xB9B0;(Boolean)</td>
        <td style="text-align:center">
          <p><b>type=&quot;submit&quot;</b>,</p>
          <p><b>type=&quot;image&quot;</b>,</p>
          <p><b>form</b>&#xC758; &#xC18D;&#xC131;&#xBCF4;&#xB2E4; &#xC6B0;&#xC120;</p>
        </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;button&gt;</b>
        </p>
      </td>
      <td style="text-align:center">formtarget</td>
      <td style="text-align:left"></td>
      <td style="text-align:center"><b>_self</b>, <b>_blank</b>
      </td>
      <td style="text-align:center">
        <p><b>type=&quot;submit&quot;</b>,</p>
        <p><b>type=&quot;image&quot;</b>,</p>
        <p><b>form</b>&#xC758; &#xC18D;&#xC131;&#xBCF4;&#xB2E4; &#xC6B0;&#xC120;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;,</b>
        </p>
        <p><b>&lt;textarea&gt;</b>
        </p>
      </td>
      <td style="text-align:center">minlength</td>
      <td style="text-align:left">&#xC785;&#xB825; &#xAC00;&#xB2A5;&#xD55C; &#xCD5C;&#xC18C; &#xBB38;&#xC790;
        &#xC218;</td>
      <td style="text-align:center">&#xC22B;&#xC790;(Number)</td>
      <td style="text-align:center">
        <p><b>type=&quot;text&quot;</b>,</p>
        <p><b>type=&quot;email&quot;</b>,</p>
        <p><b>type=&quot;password&quot;</b>,</p>
        <p><b>type=&quot;tel&quot;</b>,</p>
        <p><b>type=&quot;url&quot;</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;input /&gt;</b>
      </td>
      <td style="text-align:center">pattern</td>
      <td style="text-align:left">&#xC591;&#xC2DD;&#xC758; &#xAC12;&#xC744; &#xAC80;&#xC0AC;&#xD558;&#xB294;
        &#xC815;&#xADDC;&#xD45C;&#xD604;&#xC2DD;</td>
      <td style="text-align:center">&#xC815;&#xADDC;&#xD45C;&#xD604;&#xC2DD;(RegExp)</td>
      <td style="text-align:center">
        <p><b>type=&quot;text&quot;</b>,</p>
        <p><b>type=&quot;search&quot;</b>,</p>
        <p><b>type=&quot;tel&quot;</b>,</p>
        <p><b>type=&quot;url&quot;</b>,</p>
        <p><b>type=&quot;email&quot;</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;textarea&gt;</b>,</p>
        <p><b>&lt;select&gt;</b>
        </p>
      </td>
      <td style="text-align:center">required</td>
      <td style="text-align:left">&#xD544;&#xC218; &#xC5EC;&#xBD80;</td>
      <td style="text-align:center">&#xBD88;&#xB9B0;(Boolean)</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;input /&gt;</b>
      </td>
      <td style="text-align:center">size</td>
      <td style="text-align:left">&#xC591;&#xC2DD;&#xC758; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td style="text-align:center">&#xC22B;&#xC790;(Number, <b>20</b>)</td>
      <td style="text-align:center">&#xD3C9;&#xADE0; &#xBB38;&#xC790; &#xB108;&#xBE44;&#xB97C; &#xAE30;&#xC900;</td>
    </tr>
    <tr>
      <td style="text-align:center">
        <p><b>&lt;input /&gt;</b>,</p>
        <p><b>&lt;textarea&gt;</b>
        </p>
      </td>
      <td style="text-align:center">spellcheck</td>
      <td style="text-align:left">&#xB9DE;&#xCDA4;&#xBC95; &#xBC0F; &#xBB38;&#xBC95; &#xAC80;&#xC0AC;&#xC758;
        &#xD544;&#xC694; &#xC5EC;&#xBD80;</td>
      <td style="text-align:center"><b>true</b>, <b>false</b>
      </td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;button&gt;</b>
      </td>
      <td style="text-align:center">value</td>
      <td style="text-align:left">&#xD3FC; &#xB370;&#xC774;&#xD130;&#xC640; &#xD568;&#xAED8; &#xC804;&#xC1A1;&#xB418;&#xB294;
        &#xBC84;&#xD2BC;&#xC758; &#xCD08;&#xAE30;&#xAC12;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center">IE &#xC9C0;&#xC6D0; &#xBD88;&#xAC00;</td>
    </tr>
    <tr>
      <td style="text-align:center"><b>&lt;textarea&gt;</b>
      </td>
      <td style="text-align:center">cols</td>
      <td style="text-align:left">&#xC591;&#xC2DD;&#xC758; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td style="text-align:center">&#xC22B;&#xC790;(Number, <b>20</b>)</td>
      <td style="text-align:center">&#xD3C9;&#xADE0; &#xBB38;&#xC790; &#xB108;&#xBE44;&#xB97C; &#xAE30;&#xC900;</td>
    </tr>
  </tbody>
</table>



