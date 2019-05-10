# Build Bigger, Better:

### Modularize  

- キャッシュ、並列実行によるビルドの高速化  
- モジュール単位のテスト  
- Lint をモジュール単位で実行  

### dependencies の DRY  

- ライブラリの管理 パターン1  
<img src="img/1.png" />  
<img src="img/2.png" />  

- ライブラリの管理 パターン2  
<img src="img/3.png" />  
<img src="img/4.png" />  


- Config の管理 DSL  
<img src="img/5.png" />  
<img src="img/6.png" />  

### Build Scans  

- `./gradlew task --scan` で　Gradle のサーバにビルドの情報を送る  

### Gradle Memory Limits  

- 計測してどのくらい必要か確認する(ex. -Xms2g)   
<img src="img/7.png" />  

- Gradle build scan で Execution と garbage collection の時間を比較  

- `org.gradle.workers.max` で worker の設定ができる  
