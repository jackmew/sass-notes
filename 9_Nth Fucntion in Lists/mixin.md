nth

//nth(10px,20px,30px,1) ==> 10px
//nth((Helvetica,Arial,sans-serii),3) ==> sans-serif

@each $p in (
 one black ,
 two black + 20,
 three black + 40,
 four black + 60
) {
    .#{nth($p,1)} { background:#{nth($p,2)};}
}

ㄎ
