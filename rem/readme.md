1. 1em=font-size大小，1rem等于根元素字体大小；
2. 浏览器默认字体大小是16px （所以根元素的默认字体大小是16px）
3. chrome默认最小字体为6px（可设置）
4. rem一般只用在移动端做自适应布局，pc端一般还是固定宽度，两边留白（margin：0 auto）
5. 在移动端使用rem布局时，字体大小不必设置成rem；
6. **rem不能太小比如1px，因为页面字体大小（html根元素字体大小）最小为6px**
7. rem计算过程 ： 我们的目的是让1rem=100px；屏幕375px=100vw，所以375px/100vw= 100px/1rem，1rem=100vm/3.75
8. less/sass都可以将px直接转化为rem，使用function。以sass为例：

```
@function px2rem( $px ){
	@return $px*320/$designWidth/20 + rem;
}

$designWidth : 750;

```