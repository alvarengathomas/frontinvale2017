### 2010's

```html
  <html>
    <head>
      <title>Greetings</title>
    </head>
    <body>
      <div ng-app="testing">
        <p>Name: <input type="text" ng-model="name"></p>
        <li ng-repeat="item in items">
          {{$index}} {{item}}
        </li>
      </div>
    </body>
  </html>
```
