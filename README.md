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


### 余談visual stdio code
- ターミナル開くにはalt＋コントロール＋T（表示→統合ターミナル） 


## コンパイルの自動化について
- `tsc --init`でtsconfig.jsonを作成
- watch機能を使って自動コンパイル
- `tsc -watch xxx.ts`にすると自動コンパイルができる