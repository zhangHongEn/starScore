## starScore 星星评分

```javascript
$('selector').starScore({
  length : 5,  //星星个数
  size : '20px',  //每个星星大小
  sumScore : 5,  //总分数
  step : .1,  //步长
  emptyImgUrl : 'images/star-empty.png',  //没有分数的星星图片
  fullImgUrl : 'images/star-full.png',  //有分数的星星图片 
  prompts : ['很差!','差!','一般!','还可以!','非常好!'],  //每颗星星悬停提示文字 
  readonly : false,  //只读 
  showScoreElement : 'selector'  //显示分数的元素
}).bind('changeScore',function(e){  //分数更改(点击星星打分时)
  alert(e.score);  //更改后的分数
});
```

```html
<input 
 data-star="true" 
 data-score="1" 
 data-length="5" 
 data-size="30" 
 data-step=".1" 
 data-sum-score="10" 
 data-prompts="a,b,c" 
 data-show-score-element="#show-score"
/>
<span id="show-score"></span>
```
