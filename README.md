# homework1
R version 3.5.1 (2018-07-02) -- "Feather Spray"
Copyright (C) 2018 The R Foundation for Statistical Computing
Platform: x86_64-w64-mingw32/x64 (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY.
You are welcome to redistribute it under certain conditions.
Type 'license()' or 'licence()' for distribution details.

R is a collaborative project with many contributors.
Type 'contributors()' for more information and
'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or
'help.start()' for an HTML browser interface to help.
Type 'q()' to quit R.

> my_num1<-2.33
> my_num1
[1] 2.33
> 
> my_num2<-2.0
> my_num2
[1] 2
> 
> my_num3<-2
> my_num3
[1] 2
> 
> my_int1<-2L
> my_int1
[1] 2
> 
> my_int2 <- 2.0L
Warning message:
integer literal 2.0L contains unnecessary decimal point 
> my_int2
[1] 2
> 
> my_int3 <- 2.33L
Warning message:
integer literal 2.33L contains decimal; using numeric value 
> my_int3
[1] 2.33
> TRUE
[1] TRUE
> FALSE
[1] FALSE
> 
> T
[1] TRUE
> F
[1] FALSE
> 
> True
Error: object 'True' not found
> true
Error: object 'true' not found
> 8 > 7 # 判斷 8 是否?於 7
[1] TRUE
> 8 < 7 # 判斷 8 是否?於 7
[1] FALSE
> 8 >= 7 # 判斷 8 是否?於等於 7
[1] TRUE
> 8 <= 7 # 判斷 8 是否?於等於 7
[1] FALSE
> 8 == 7 # 判斷 8 是否等於 7
[1] FALSE
> 8 != 7 # 判斷 8 是否不等於 7
[1] TRUE
> 7 %in% c(8, 7) # 判斷 7 是否包含於?個 c(8, 7) 之中
[1] TRUE
> first_name <- "Cindy"
> first_name
[1] "Cindy"
> my_weight
Error: object 'my_weight' not found
> my_height <- 163
> my_weight <- 50
> my_weight
[1] 50
> my_height
[1] 163
> class(2)
[1] "numeric"
> class(2L)
[1] "integer"
> class(TRUE)
[1] "logical"
> class("Learning R the easy way")
[1] "character"
> is.numeric(8.7)
[1] TRUE
> is.numeric("8.7")
[1] FALSE
> is.integer(7L)
[1] TRUE
> is.integer(7)
[1] FALSE
> is.logical(FALSE)
[1] TRUE
> is.logical("FALSE")
[1] FALSE
> is.character("TRUE")
[1] TRUE
> is.character(TRUE)
[1] FALSE
> inherits(Sys.Date(), what = "Date") # Sys.Date() 是?期類型
[1] TRUE
> inherits("1970-01-01", what = "Date") # "1970-01-01" 是?字類型
[1] FALSE
> 
> inherits(Sys.time(), what = "POSIXct") # Sys.time() 是時間類型
[1] TRUE
> inherits("1970-01-01 00:00:00", what = "POSIXct") # "1970-01-01 00:00:00" 是?字類型
[1] FALSE
> 
> as.numeric(7L)
[1] 7
> as.numeric(TRUE)
[1] 1
> as.numeric(FALSE)
[1] 0
> as.numeric(Sys.Date())
[1] 17802
> as.numeric(Sys.time())
[1] 1538121918
> 
> as.integer(7)
[1] 7
> as.integer(TRUE)
[1] 1
> as.integer(FALSE)
[1] 0
> as.integer(Sys.Date())
[1] 17802
> as.integer(Sys.time())
[1] 1538121918
> 
> as.logical(0)
[1] FALSE
> as.logical(0L)
[1] FALSE
> as.logical(1L)
[1] TRUE
> as.logical(-1.3)
[1] TRUE
> as.logical(87)
[1] TRUE
> as.logical("TRUE")
[1] TRUE
> as.logical("True")
[1] TRUE
> as.logical("true")
[1] TRUE
> as.logical("FALSE")
[1] FALSE
> as.logical("False")
[1] FALSE
> as.logical("false")
[1] FALSE
> 
> as.character(8.7)
[1] "8.7"
> as.character(87L)
[1] "87"
> as.character(TRUE)
[1] "TRUE"
> as.character(Sys.Date())
[1] "2018-09-28"
> as.character(Sys.time())
[1] "2018-09-28 16:05:18"
> 
> as.Date("1970-01-01")
[1] "1970-01-01"
> as.Date("1970/01/01")
[1] "1970-01-01"
> as.Date("01-01-1970") # 轉換錯誤
[1] "0001-01-19"
> as.Date("01-01-1970", format = "%m-%d-%Y") # 轉換正確
[1] "1970-01-01"
> as.Date("01/01/70") # 不是預設格式，轉換失敗
Error in charToDate(x) : 
  character string is not in a standard unambiguous format
> as.Date("01/01/70", format = "%m/%d/%y") # 轉換正確
[1] "1970-01-01"
> 
> as.POSIXct("1970-01-01 00:00:00")
[1] "1970-01-01 CST"
> as.POSIXct("1970-01-01 00:00:00", tz = "GMT")
[1] "1970-01-01 GMT"
