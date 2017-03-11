## R Workshop
----------------

#### Creating vectors

```r
vector <- c(0,-9,8,0.35,100)
vector <- c(1:10)
```

#### Conversions

```r
vector <- c("1","2","3")
as.integer(vector)
```

#### Samples

```r
data <- sample(-15:15,12)
data <- sample(-15:15,12,replace=T)
```

#### Matrix

```r
m <- matrix(data, 4, 3)
```

#### Frames

```r
users <- data.frame(nickname=c("erich", "martinv", "josdem"),
                    score=c(5,4,5),
                    email=c("erich@emailcom","martinv@email.com","josdem@email.com")
)
table(users$score)
platform <- c("Mac","Windows","Ubuntu")
users$platform <- platform
users[2,2]<-5
```

#### Installing Packages

```bash
install.packages("googlesheets")
library("googlesheets")
workshop <- gs_title("R Workshop")
Workshop_df <- gs_read(Workshop)
```

#### Exercise

1. What is 27 + 1198 / 2 - 63
2. Set a equal to 7, b equal to 17 and c equal to their product. What is c?
3. Set e equal yo c(5,5.1,-12,38,100.5) Find the mean, max, and length of e
4. Change e to character vector, save it as e_char
