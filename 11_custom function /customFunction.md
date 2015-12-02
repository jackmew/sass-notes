12 useful function

http://sass-lang.com/documentation/Sass/Script/Functions.html




判斷傳入的參數 $background  的lightness(亮度) 是某有超過50%
若沒有 就讓文字亮一點
若有 就讓文字暗一點


@function text-contrast($background) {
    @if lightness($background) < 50% {
        @return lighten($background,70%);
    } @else {
        @return darken($background,90%);
    }

}
.three {
    color:text-contrast(white);
}
