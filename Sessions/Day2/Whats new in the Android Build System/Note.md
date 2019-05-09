# What's new in the Android Build System  


### Worker API  

- AS 3.5 で `enableWorker` は true 、 `use.worker.api` は false
<img src="img/1.png" />

### Artifact Transforms  
- Gradle をはやくできる API?
- Dexing のタイミングを変更してモジュール単位でキャッシュするように  

### Apply changes  
- Instant Run に代わるもの   

### Build Output
- エラーが見やすくなるように  

### Build Speed
- AS 3.5 と Gradle 5.4 の組み合わせで早くなった(35% ぐらい)  
- しかし、全体としては Kotlin やプラグインとかが増えて 25% ぐらい遅くなってる  

### Speed attribution  
- Gradle Plugin のタスクや遅くなっているのを可視化できるようになる?(Comming soon)  

### Chrome Trace  

- Chrome でビルドの Trace が見れる!?  
```
-Pandroid.enableProfileJson=true

// json file in build/android-profile
```
