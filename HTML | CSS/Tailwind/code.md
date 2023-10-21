#################
# grid
#################
grid
親要素に指定。flex と同じような使い方。

grid-cols-{n}
n 個のカラム(横の要素数)をもつグリッドかを指定。gridと一緒に、親要素に指定。

col-span-{n}
要素自体の幅。子要素に指定。

```:SampleComponent.tsx
<div className="grid grid-cols-3">{/* 3カラムのグリッドであることを指定 */}
  <div className="col-span-1">1</div1>
  <div className="col-span-2">2</div1>{/* この要素で2カラム分使っている */}
  <div className="col-span-1">3</div1>{/* ここから下の段に改行される */}
  <div className="col-span-1">4</div1>
</div>
```

gap-{n}
n スペース分の余白を要素と要素の間にもたせるか。親要素に指定。
普通に要素感の余白の大きさです。
gap-\[10px]みたいな使い方もできるはず(JIT モードなら)

[参照](https://zenn.dev/mayo_dev/articles/learn-grid-layout-with-tailwind)
