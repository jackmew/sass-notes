@while



@function text-contrast($background) {
    @if lightness($background) < 50% {
        @return white;
    } @else {
        @return black;
    }

}


$j : 1;
$parbg : black;
@while $j < 5 {
    .par-#{$j} { margin-left:20px * $j; background:$parbg;color:text-contrast($parbg);}
    $parbg : lighten($parbg,25%);
    $j : $j + 1;
}

也就說會動態 讓parbg 變色 然後同時call text-contrast 讓字體也變色



sudo gem install sass => 再次安裝 就update了
