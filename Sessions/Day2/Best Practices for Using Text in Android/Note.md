# Best Practices for Using Text in Android  

### Precomputed Text  

- Text のスタイルは Precomputed の後に変更したらエラーになる  
<img src="img/1.png" />

### Styling Text  

- Android Q より TextAppearance パラメータが追加される  
<img src="img/2.png" />  

### Custom Fonts  

<img src="img/3.png" />  
効率的ではない  

- Android Q より `Typeface.CustomFallbackBuilder` が追加    
<img src="img/4.png" />  
<img src="img/5.png" />  

- 複数の Style も可能  
<img src="img/6.png" />  

- `CustomFallbackBuilder` では最大 64 のフォントまで使える  

- サポートしているフォントから使われ、最終的にはシステムフォントになる  
<img src="img/7.png" />  

- その場合のシステムフォントのスタイルも定義可能  
<img src="img/8.png" />  

- フォントの Weight もセットできる  
<img src="img/9.png" />  

### Editable Text  

- EditText + Image  
<img src="img/10.png" />  

- TextInputLayout の Helper Text の下にキーボードになるのは Rect 周りをいじっているため  

- キーボードにパスワードを覚えさせないようにできる  
```
android:imeOptions="flagNoPersonalizedLearning"
```
