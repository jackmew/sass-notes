13 useful function

http://sass-lang.com/documentation/Sass/Script/Functions.html




@function text-contrast($background) {
    @if lightness($background) < 50% {
        @return lighten($background,90%);
    } @else {
        @return darken($background,90%);
    }

}

@each $p in (
one black ,
two black + 20,
three white,
four white - 40
) {
    .#{nth($p,1)} { background:nth($p,2); color:text-contrast(nth($p,2));}
}
通過each後的每一個tag p 都會去判斷背景顏色是啥 而且文字可能變亮或變暗

也就是說我們可以想像 切換一個backgound 顏色 就可以改變整個頁面主題的感覺！
