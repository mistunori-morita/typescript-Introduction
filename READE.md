# Typescript導入
- `http://www.typescriptlang.org/#download-links`にて`npm install -g typescript`とnode.jsをインストール

## コンパイルについて
```js
// typescriptにてこういう書き方をしたのち
class Exmaple {

  public houser = null;

  run(){
    alert('hello')
  }


}


//ターミナルから tsc xxxx.ts（xxxはファイル名）をやるとプロジェクトフォルダにxxxx.jsとして書き出される
//下が書き出されたあと
var Exmaple = /** @class */ (function () {
    function Exmaple() {
        this.houser = null;
    }
    Exmaple.prototype.run = function () {
        alert('hello');
    };
    return Exmaple;
}());
```
