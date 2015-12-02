10. build in function


thesassway.com

也就是說 有內建一些css function

fade-out() 就是內建function => rgba()

percentage() 用來計算畫面比例用的

sass-lang.com/docs/yardoc/Sass/Script/Functions.html

11. custom made function


@function text-contrast($background,$val) {
    @return ( $background + $val )
}
.three {
    color:text-contrast(black + 40 ,100);
}

你可以自定義function 並回傳你要的參數
