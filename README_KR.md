# things-combo

이는 things-combo.items로 받은 데이터들을 콤보박스로 출력하고 선택한 값을 필드에 표시하는 컴포넌트이다.

Example:

```html
      <things-combo
        items="[{name: 'item1', descrption: 'First Item'},
                {name: 'itme2', description: 'Second Item'}]"
        label-path="description"
        value-path="name">
      </things-combo>
```

## Dependencies

element의 종속성은 [Bower](http://bower.io/)를 통해 관리되며, 아래의 방법을 통해 설치할 수 있다.

    npm install -g bower

다음, element의 종속성을 다운로드한다.

    bower install


## Playing With Your Element

element를 독립적으로 처리하려면 [Polyserve](https://github.com/PolymerLabs/polyserve)를 사용하여 element의 bower 의존성을 유지하도록 하며, 이는 아래의 방법을 통해 설치할 수 있다.

    npm install -g polymer-cli

그리고, 아래의 방법을 통해 실행할 수 있다.

    polymer serve

element를 실행한 경우, `things-combo`가 디렉토리 이름으로 포함되어 있는 `http://localhost:8080/components/things-combo/`를 통해 이를 미리 확인할 수 있다. 


## Testing Your Element

element의 `/test` 디렉토리로 이동하여 테스트를 실행한다. polyserve를 사용할 경우: `http://localhost:8080/components/things-combo/test/`

### web-component-tester

이 테스트는 [web-component-tester](https://github.com/Polymer/web-component-tester)와 호환되며, 아래와 같이 설치한다.

    npm install -g web-component-tester

다음, 아래와 같이 _모든_ 로컬 브라우저에서 테스트를 실행할 수 있다.

    wct

#### WCT Tips

`wct -l chrome`은 크롬에서만 테스트를 실행한다.

`wct -p`는 테스트가 실행된 후 브라우저를 계속 활성화(새로고침을 통해 다시 실행)한다.

`wct test/some-file.html`은 지정한 파일들만 테스트한다.


## Yeoman support

Yeoman을 사용하여 element를 설치하는 방법도 가능하다. 공식적인 [`generator-polymer`](https://github.com/yeoman/generator-polymer) 생성기에 [`seed`](https://github.com/yeoman/generator-polymer#seed)라는 하위 생성기가 있기 때문이다.
