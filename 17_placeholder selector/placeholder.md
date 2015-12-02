placeholder


#main %blue {
    color:white;
    background-color:blue;
    font-size:14px;
}

.sign {
    @extend %blue;
}
.box {
    @extend %blue;
}




====> 其實看不出來有沒有比較好..


#main .sign, #main .box {
  color: white;
  background-color: blue;
  font-size: 14px; }
