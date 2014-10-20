SDialog
=======
기존 브라우저가 제공하는 다이얼로그(Alert, Confirm)창을 브라우저 요소가 아닌 자바스크립트 요소로 사용할 수 있습니다.

#중요함

## 노트

## 시작하기

SDialog는 매우 쉽게 사용할 수 있습니다.

먼저 SDialog를 다운로드 합니다. [Download it](https://github.com/siluniv/SDialog/archive/master.zip)

다운로드를 완료하였으면 헤드 영역에 다음과 같이 HTML 태그를 추가합니다.
```html
<link rel="stylesheet" href="path/to/your/sdialog.css">
```

다음으로 script를 연결해주어야 합니다. 헤드 영역이나 `</body>`태그 이전에 추가 해주어야 합니다.
```html
<script src="path/to/your/sdialog.js"></script>
```

스타일과 스크립트를 연결하였으면 모든 준비가 끝났습니다.

원하는 곳에서 `sdialog()` 메서드를 이용하여 간단하게 다이얼로그 창을 만들어 낼 수 있습니다.

## 사용자정의

SDialog는 몇가지의 사용자 정의를 지원합니다.

```html
<script>
var options = {
  type:'message',
  bgClick:true
}

sdialog('사용자 정의 문자열', options, function(){ ... });
</script>
```

#### type

`Default: 'message'`

사용하는 다이얼로그의 형식을 정의할 수 있습니다.
