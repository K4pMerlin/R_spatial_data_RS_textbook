### 判断体
```R
x <- 30L
if(is.integer(x)) {
  print("X is an Integer")
}

x <- c("what","is","truth")

if("Truth" %in% x) {
  print("Truth is found")
} else {
  print("Truth is not found")
}

if("Truth" %in% x) {
  print("Truth is found the first time")
} else if ("truth" %in% x) {
  print("truth is found the second time")
} else {
  print("No truth found")
}

x <- switch(
  3,
  "first",
  "second",
  "third",
  "fourth"
)
print(x)
```


### 循环体
```R
v <- c("Hello","loop")
cnt <- 2

repeat {
  print(v)
  cnt <- cnt+1
  
  if(cnt > 5) {
    break
  }
}

v <- c("Hello","while loop")
cnt <- 2

while (cnt < 7) {
  print(v)
  cnt = cnt + 1
}

v <- LETTERS[1:4]
for ( i in v) {
  print(i)
}
```
### 函数
```R
new.function1 <- function() {
  for(i in 1:5) {
    print(i^2)
  }
}	
new.function1()

new.function2 <- function(a,b,c) {
  result <- a * b + c
  print(result)
}
new.function1(5,3,11)
new.function1(a = 11, b = 5, c = 3)

new.function2 <- function(a = 3, b = 6) {
  result <- a * b
  print(result)
}
new.function2()
new.function2(5)
new.function2(b=5)
```

