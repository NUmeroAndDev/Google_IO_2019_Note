# Understanding ART for Faster App  

### Android Q でアプリの起動時間の改善  

- Cloud Profile  
- アプリのプロセス管理の調整  
- アプリ起動の計測に `reportFullyDrawn()`  


### GC  

- Android O では Concurrent copying GC  
- Android Q では Minor and major collection   

### Heap compaction  

- 参照が途切れていないものを別の Space に移動させて残ったもの(参照されていないもの)をクリアする  


### Region space compaction  

- Space を細かく分割し、区切った Space 内で全て参照されているかチェックする  
- 全て参照されていない Space のものを別の Space に移動させ、クリアする  

### Improved heap compaction    

- 使えるスペースが 3 つを下回ったら参照しているものをまとめて移動させて、空きスペースを確保する  
- 全体的に使えるメモリの空き容量を確保できる  
