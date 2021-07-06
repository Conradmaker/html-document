# AUDIO / VIDEO

## **&lt;audio&gt;**

​소리 콘텐츠\(MP3\)를 삽입.

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>&#xC18D;&#xC131;</b>
      </th>
      <th style="text-align:left"><b>&#xC758;&#xBBF8;</b>
      </th>
      <th style="text-align:left"><b>&#xAC12;</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">autoplay</td>
      <td style="text-align:left">&#xC900;&#xBE44;&#xB418;&#xBA74; &#xBC14;&#xB85C; &#xC7AC;&#xC0DD;</td>
      <td
      style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
    </tr>
    <tr>
      <td style="text-align:left">controls</td>
      <td style="text-align:left">&#xC81C;&#xC5B4; &#xBA54;&#xB274;&#xB97C; &#xD45C;&#xC2DC;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
    </tr>
    <tr>
      <td style="text-align:left">loop</td>
      <td style="text-align:left">&#xC7AC;&#xC0DD;&#xC774; &#xB05D;&#xB098;&#xBA74; &#xB2E4;&#xC2DC; &#xCC98;&#xC74C;&#xBD80;&#xD130;
        &#xC7AC;&#xC0DD;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
    </tr>
    <tr>
      <td style="text-align:left">preload</td>
      <td style="text-align:left">&#xD398;&#xC774;&#xC9C0;&#xAC00; &#xB85C;&#xB4DC;&#xB420; &#xB54C; &#xD30C;&#xC77C;&#xC744;
        &#xB85C;&#xB4DC;&#xD560;&#xC9C0;&#xC758; &#xC9C0;&#xC815;(&#xD78C;&#xD2B8;
        &#xC81C;&#xACF5;)</td>
      <td style="text-align:left">
        <p><b>none</b>: &#xB85C;&#xB4DC;&#xD558;&#xC9C0; &#xC54A;&#xC74C;,</p>
        <p><b>metadata</b>: &#xBA54;&#xD0C0;&#xB370;&#xC774;&#xD130;&#xB9CC;(&#xAE30;&#xBCF8;),</p>
        <p><b>auto</b>: &#xC804;&#xCCB4; &#xD30C;&#xC77C; &#xB85C;&#xB4DC;</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">src</td>
      <td style="text-align:left">&#xCF58;&#xD150;&#xCE20; URL</td>
      <td style="text-align:left">URL</td>
    </tr>
    <tr>
      <td style="text-align:left">muted</td>
      <td style="text-align:left">&#xC74C;&#xC18C;&#xAC70; &#xC5EC;&#xBD80;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
    </tr>
  </tbody>
</table>

```markup
 <audio

    controls //컨트롤러

    autoplay //자동재생

    muted    //음소거

    src="/media/examples/t-rex-roar.mp3">

    </audio>
```

 _\*몇초부터 재생할지등의 옵션은 자바스크립트를 통해 설정\*_

 _\*autoplay, preload는 동시사용 불가\*_  




## **&lt;video&gt;**

**​**동영상 콘텐츠\(MP4\)를 삽입.

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
      <td style="text-align:left">autoplay</td>
      <td style="text-align:left">&#xC900;&#xBE44;&#xB418;&#xBA74; &#xBC14;&#xB85C; &#xC7AC;&#xC0DD;</td>
      <td
      style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
        <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">controls</td>
      <td style="text-align:left">&#xC81C;&#xC5B4; &#xBA54;&#xB274;&#xB97C; &#xD45C;&#xC2DC;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">loop</td>
      <td style="text-align:left">&#xC7AC;&#xC0DD;&#xC774; &#xB05D;&#xB098;&#xBA74; &#xB2E4;&#xC2DC; &#xCC98;&#xC74C;&#xBD80;&#xD130;
        &#xC7AC;&#xC0DD;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">muted</td>
      <td style="text-align:left">&#xC74C;&#xC18C;&#xAC70; &#xC5EC;&#xBD80;</td>
      <td style="text-align:left">&#xBD88;&#xB9B0;(Boolean)</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">poster</td>
      <td style="text-align:left">&#xB3D9;&#xC601;&#xC0C1; &#xC378;&#xB124;&#xC77C; &#xC774;&#xBBF8;&#xC9C0;
        URL</td>
      <td style="text-align:left">URL</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">preload</td>
      <td style="text-align:left">&#xD398;&#xC774;&#xC9C0;&#xAC00; &#xB85C;&#xB4DC;&#xB420; &#xB54C; &#xD30C;&#xC77C;&#xC744;
        &#xB85C;&#xB4DC;&#xD560;&#xC9C0;&#xC758; &#xC9C0;&#xC815;(&#xD78C;&#xD2B8;
        &#xC81C;&#xACF5;)</td>
      <td style="text-align:left">
        <p><b>none</b>: &#xB85C;&#xB4DC;&#xD558;&#xC9C0; &#xC54A;&#xC74C;,</p>
        <p><b>metadata</b>: &#xBA54;&#xD0C0;&#xB370;&#xC774;&#xD130;&#xB9CC; &#xB85C;&#xB4DC;,</p>
        <p><b>auto</b>: &#xC804;&#xCCB4; &#xD30C;&#xC77C; &#xB85C;&#xB4DC;</p>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">src</td>
      <td style="text-align:left">&#xCF58;&#xD150;&#xCE20; URL</td>
      <td style="text-align:left">URL</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">width</td>
      <td style="text-align:left">&#xB3D9;&#xC601;&#xC0C1; &#xAC00;&#xB85C; &#xB108;&#xBE44;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">height</td>
      <td style="text-align:left">&#xB3D9;&#xC601;&#xC0C1; &#xC138;&#xB85C; &#xB108;&#xBE44;</td>
      <td style="text-align:left"></td>
      <td style="text-align:left"></td>
    </tr>
  </tbody>
</table>

```markup
   <video width="250"

    controls  //컨트롤러

    loop      //반복재생

    muted     //음소거

    poster    //썸네일

     src="https://interactive-examples.mdn.mozilla.net/media/examples/flower.webm">

    </video>
```

_\*몇초부터 재생할지등의 옵션은 자바스크립트를 통해 설정\*_

 _\*autoplay, preload는 동시사용 불가\*_

