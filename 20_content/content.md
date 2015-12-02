@content

@mixin phone {
    @media only screen and (max-width:480px) {
        @content;
    }
}

在media query 時特別好用

一樣可以傳變數進去！
