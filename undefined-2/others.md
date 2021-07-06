---
description: >-
  <button>,<textarea>,<fieldset>, <legend>,<select>, <datalist>, <optgroup>,
  <option>,<progress>
---

# others

### **button** **{** **display: inline-block; }**

선택 가능한 버튼을 지정한다.



| **속성** | **의미** | **값** | **특징** |
| :--- | :--- | :--- | :--- |
| autofocus | 페이지가 로드될 때 자동으로 포커스 | 불린\(Boolean\) | 문서 내 고유해야 함 |
| disabled | 버튼을 비활성화 | 불린\(Boolean\) |  |
| form | **&lt;form&gt;**의 **id** 속성 값 |  | 해당 **&lt;form&gt;**의 후손이 아닐 경우만 |
| name | 폼 데이터와 함께 전송되는 버튼의 이름 |  |  |
| type | 버튼의 타입 | **button**, **reset**, **submit** |  |

```markup
<body>
    <input type="submit" value="제출">
    <button type="submit">제출</button>    //2개는 같은 역할을 한다
   
    <button onclick="doit">클릭하세요!</button>
                                         //일반 버튼은 보통JS와 연계
    <script>
    function doit(){
        alert('클릭했습니다')
    }
    </script>

</body>
```



###  **textarea** **{** **display: inline-block; }**

여러 줄의 일반 텍스트 양식



| **속성** | **의미** | **값** | **기본값** | **특징** |
| :---: | :---: | :---: | :---: | :---: |
| autocomplete | 사용자가 이전에 입력한 값으로 자동 완성 기능을 사용할 것인지 여부 | **on**, **off** | **on** |  |
| autofocus | 페이지가 로드될 때 자동으로 포커스 | 불린\(Boolean\) |  | 문서 내 고유해야 함 |
| disabled | 양식을 비활성화 | 불린\(Boolean\) |  |  |
| form | **&lt;form&gt;**의 **id** 속성 값 |  |  | 해당 **&lt;form&gt;**의 후손이 아닐 경우만 |
| maxlength | 입력 가능한 최대 문자 수 | 숫자\(Number\) | 무한 |  |
| name | 양식의 이름 |  |  |  |
| placeholder | 사용자가 입력할 값의 힌트 |  |  |  |
| readonly | 수정 불가한 읽기 전용 | 불린\(Boolean\) |  |  |
| rows | 양식의 줄 수 | 숫자\(Number\) | **2** |  |





###  **fieldset,** **legend** **{** **display: block; }**

같은 목적의 양식을 그룹화\(**&lt;fieldset&gt;**\).

그룹의 제목\(**&lt;legend&gt;**\)을 지정.

```markup
<form>
        <fieldset>
          <legend>Coffee Size</legend>
          <label>
              <input type="radio" name="size" value="tall" />
              Tall
          </label>
          <label>
              <input type="radio" name="size" value="grande" />
              Grande
          </label>
          <label>
              <input type="radio" name="size" value="venti" />
              Venti
          </label>
        </fieldset>
</form>

```

![](../.gitbook/assets/image%20%286%29.png)

#### \*\*\*\*

#### **&lt;fieldset&gt;태그의 속성들**

| **속성** | **의미** | **값** |  |
| :--- | :--- | :--- | :--- |
| disabled | 그룹 내 모든 양식 요소를 비활성화 | 불린\(Boolean\) |  |
| form | 그룹이 속할 하나 이상의 **&lt;form&gt;**의 **id** 속성 값 |  |  |
| name | 그룹의 이름 |  |  |



##  **&lt;select&gt;, &lt;datalist&gt;, &lt;optgroup&gt;, &lt;option&gt;**

 ****옵션\(**&lt;option&gt;**, **&lt;optgroup&gt;**\)의

 선택 메뉴\(**&lt;select&gt;**\)나

 자동완성\(**&lt;datalist&gt;**\)을 제공.

### \*\*\*\*

### **&lt;select&gt;**

옵션을 선택하는 메뉴.

| **속성** | **의미** | **값** | **기본값** |  |
| :--- | :--- | :--- | :--- | :--- |
| autocomplete | 사용자가 이전에 입력한 값으로 자동 완성 기능을 사용할 것인지 여부 | **on**, **off** | **on** |  |
| disabled | 선택 메뉴를 비활성화 | 불린\(Boolean\) |  |  |
| form | 선택 메뉴가 속할 하나 이상의 **&lt;form&gt;**의 **id** 속성 값 |  |  |  |
| multiple | 다중 선택 여부 | 불린\(Boolean\) |  |  |
| name | 선택 메뉴의 이름 |  |  |  |
| size | 한 번에 볼 수 있는 행의 개수 |  |  |  |

```markup
<body>
    <select name="pets" size="3" multiple disabled>       /1.한번에 3개씩 보여준다.
        <option value="">Please choose an option</option>  2.중복선택 가능
        <option value="dog">Dog</option>                   3.선택 비활성화
        <option value="cat">Cat</option>
        <option value="hamster">Hamster</option>
        <option value="parrot">Parrot</option>
        <option value="spider">Spider</option>
        <option value="goldfish">Goldfish</option>
    </select>
</body>
```



### **&lt;option&gt;**

선택 메뉴\(**&lt;select&gt;**\)나 자동완성\(**&lt;datalist&gt;**\)에서 사용될 옵션.

\*선택적 빈태그로 사용가능\*

| **속성** | **의미** | **값** | **특성** |
| :--- | :--- | :--- | :--- |
| disabled | 옵션을 비활성화 | 불린\(Boolean\) |  |
| label | 표시될 옵션의 제목 |  | 생략되면 포함된 텍스트를 표시 |
| selected | 옵션이 선택되었음을 표시 | 불린\(Boolean\) |  |
| value | 양식으로 제출될 값 |  | 생략되면 포함된 텍스트를 값으로 사용 |

```markup
<select name="pets">    
    <optgroup label="좋아하는 pet">
        <option value="dog">Dog</option>               
        <option value="cat">Cat</option>
        <option value="hamster">Hamster</option>
    </optgroup>
    <optgroup label="싫어하는 pet">
        <option value="parrot">Parrot</option>
        <option value="spider">Spider</option>
        <option value="goldfish">Goldfish</option>
    </optgroup>
</select>

```

![](../.gitbook/assets/image%20%287%29.png)





### **&lt;datalist&gt;**

**&lt;input&gt;**에 미리 정의된 옵션을 지정하여 자동완성\(Autocomplete\) 기능을 제공하는 데 사용.

**\*&lt;input&gt;**의 **list** 속성 바인딩.\*

**\*&lt;option&gt;**을 포함하여 정의된 옵션을 지정.\*

```markup
<body>
    <input type="text" list="fruits">
     <datalist id="fruits"> //input의 리스트값과 연결
        <option>Apple</option>
        <option>Orange</option>
        <option>Banana</option>
        <option>Mango</option>
        <option>Fineapple</option>
     </datalist>
</body>
```





### **&lt;progress&gt;**

작업의 완료 진행률을 표시.

| **속성** | **의미** | **값** | **특징** |
| :--- | :--- | :--- | :--- |
| max | 작업의 총량 | 숫자\(Number\) |  |
| value | 작업의 진행량 | 숫자\(Number\) | **max** 속성을 생략할 경우 **0**~**1** 사이의 숫자여야 함 |

```markup
<body>
    <progress value="70" max="100">70 %</progress>
    <script>
        const progress = document.querySelector('progress');
        const interval = setInterval(function () {
            progress.value += 10;
            if (progress.value >= 100) clearInterval(interval);
        }, 1000)
    </script>
</body>
```

