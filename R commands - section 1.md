## R important command:

| Command | Description |
| ------- | ----------- |
| `getwd()` | This command prints the current working directory in R, which is the directory where R is currently looking for and saving files. |
| `setwd("path")` | This command sets the current working directory to the directory specified by `"path"`. For example, `setwd("/Users/username/Documents")` sets the current working directory to the "Documents" folder in the user's home directory. |
| `x = 10` | This command assigns the value `10` to the variable `x`. The type of `x` is dynamically assigned based on the value it is assigned. In this case, `x` is assigned as an integer. |
| `x<-20` | This command is similar to the previous one, but uses the older assignment operator `<-` to assign the value `20` to the variable `x`. |
| `class(x)` | This command returns the class of the variable `x`. For example, if `x` is an integer, `class(x)` returns `"integer"`. |
| `x<-as.character(x)` | This command converts the variable `x` to a character type. If `x` was previously an integer, it will be converted to a character string representation of the integer. |
| `x<-as.integer(x)` | This command converts the variable `x` to an integer type. If `x` was previously a character, it will be converted to an integer representation of the characters. If the conversion fails, `NA` is returned. |
| `v1<-c(1,2,3,4,5)` | This command creates a vector `v1` with the elements `1, 2, 3, 4, 5`. The `c()` function is used to concatenate the elements into a single vector. |
| `v3<-c(v1,v2)` | This command creates a new vector `v3` by concatenating the elements of `v1` and `v2`. `v1` and `v2` must be vectors of the same type for this to work. |
| `1:10` | This command creates a vector with the integers from `1` to `10`. The `:` operator is used to create a sequence of integers. |
| `seq(1,10,by=2)` | This command creates a sequence of numbers from `1` to `10` with a step size of `2`. The `by` parameter specifies the step size. |
| `seq(1,10,length=4)` | This command creates a sequence of numbers from `1` to `10` with a length of `4`. The `length` parameter specifies the number of elements in the sequence. |
| `rep(1,5)` | This command creates a vector of length `5` with all elements equal to `1`. The first argument specifies the element to be repeated, and the second argument specifies the number of times to repeat it. |
| `rep(2:4,3)` | This command creates a vector by repeating the elements of `2:4` (i.e., `2, 3, 4`) three times. The resulting vector is `2, 3, 4, 2, 3, 4, 2, 3, 4`. |
| `v5[3]` | This command returns the third element of the vector `v5`. Vector indexing in R starts from `1`, so `v5[3]` returns the value of the third element in `v5`. |
| `sort(v6, decreasing = FALSE)` | This command sorts the elements of the vector `v6` in ascending order. If `decreasing = TRUE`, the elements will be sorted in descending order. If `decreasing` is not specified, it defaults to `FALSE`. |

| Function | Description |
| -------- | ----------- |
| `abs(z)` | This function returns the absolute value of `z`, which is the distance of `z` from 0 on the number line. For example, if `z` is `-5`, `abs(z)` will return `5`. |
| `sign(w)` | This function returns the sign of `w`. If `w` is positive, it returns `1`. If `w` is negative, it returns `-1`. If `w` is zero, it returns `0`. |
| `sqrt(25)` | This function returns the square root of `25`, which is `5`. |
| `round(w,1)` | This function rounds `w` to 1 decimal place. For example, if `w` is `3.14159`, `round(w,1)` will return `3.1`. |
| `exp(0)` | This function returns the value of `e` raised to the power of `0`, which is `1`. |
| `log(100,10)` | This function returns the logarithm of `100` to the base `10`, which is `2`. In general, `log(x, b)` returns the logarithm of `x` to the base `b`. |
| `sin(2*pi)` | This function returns the sine of `2*pi`, which is `0`. Note that `sin` takes its argument in radians, so `2*pi` corresponds to one complete revolution around the unit circle. The sine of any multiple of `pi` is `0`. |
| `factorial(5)` | This function returns the factorial of `5`, which is `5 * 4 * 3 * 2 * 1`, or `120`. In general, the factorial of a non-negative integer `n` is `n! = n * (n-1) * (n-2) * ... * 1`. |
| `cumsum(1:5)` | This function returns the cumulative sum of the elements in the vector `1:5`. The cumulative sum of a vector is a new vector where each element is the sum of all the previous elements, including itself. For example, `cumsum(1:5)` returns the vector `1 3 6 10 15`, because the cumulative sum of `1:5` is `1 1+2 1+2+3 1+2+3+4 1+2+3+4+5`. |
|v7<-c(8,89,65,8,9,1)|This command creates a new vector `v7` with the values `8, 89, 65, 8, 9, 1`. The `c()` function is used to concatenate the values into a single vector. The resulting vector `v7` has a length of `6`.|


|  Statistics | Description |
| ------- | ----------- |
| `min(v7)` | This command returns the minimum value in the vector `v7`. In this case, the minimum value in `v7` is `1`. |
| `max(v7)` | This command returns the maximum value in the vector `v7`. In this case, the maximum value in `v7` is `89`. |
| `mean(v7)` | This command returns the mean (average) value of the elements in the vector `v7`. In this case, the mean value of `v7` is `(8+89+65+8+9+1)/6 = 26.83333`. |
| `var(v7)` | This command returns the variance of the elements in the vector `v7`. In this case, the variance of `v7` is `955.6`. |
| `sd(v7)` | This command returns the standard deviation of the elements in the vector `v7`. In this case, the standard deviation of `v7` is `30.9446`. |
| `cor(v7,v8)` | This command returns the correlation coefficient between the vectors `v7` and `v8`. The correlation coefficient measures the strength and direction of the linear relationship between two variables. If `v7` and `v8` are of the same length, this command calculates the Pearson correlation coefficient. If `v7` and `v8` have different lengths, R will recycle the shorter vector to match the length of the longer vector. |


|Functions | Details|
|--|--|
|`v7 == 89`|This command returns a logical vector of the same length as `v7`, where each element is `TRUE` if the corresponding element in `v7` is equal to `89`, and `FALSE` otherwise. In this case, the resulting logical vector is `FALSE, TRUE, FALSE, FALSE, FALSE, FALSE`.|
|`which(v7==8)`|This command returns a vector of indices where the elements in `v7` are equal to `8`. The `which()` function returns the indices of a logical vector that are `TRUE`. In this case, the resulting vector is `1 4`, because the first and fourth elements of `v7` are equal to `8`.|
|which(v7<=8)|This command returns a vector of indices where the elements in `v7` are less than or equal to `8`. The resulting vector contains the indices of all the elements in `v7` that are less than or equal to `8`. In this case, the resulting vector is `1 4 6`, because the first, fourth, and sixth elements of `v7` are less than or equal to `8`.|
|`any(v7==2)`|This command returns a logical value `FALSE` because there is no element in the vector `v7` that is equal to `2`. The `any()` function returns `TRUE` if at least one element of a logical vector is `TRUE`, and `FALSE` otherwise. Since there is no element in `v7` equal to `2`, the expression `v7==2` evaluates to a logical vector of `FALSE`s, and so `any(v7==2)` returns `FALSE`.|
|`all(v7>0)`|This command returns a logical value `TRUE` because all the elements of `v7` are greater than `0`. The `all()` function returns `TRUE` if all the elements of a logical vector are `TRUE`, and `FALSE` otherwise. Since all the elements of `v7` are greater than `0`, the expression `v7>0` evaluates to a logical vector of all `TRUE`s, and so `all(v7>0)` returns `TRUE`.|
|`! v7 == 225`|This command returns a logical vector of the same length as `v7`, where each element is `TRUE` if the corresponding element in `v7` is not equal to `225`, and `FALSE` otherwise. The `!` operator is used to negate the logical vector obtained from `v7 == 225`. In this case, the resulting logical vector is `TRUE, TRUE, TRUE, TRUE, TRUE, TRUE`.|
|`any(v7>50) & any(v7<100)`|This command returns a logical value `TRUE` because at least one element of `v7` is greater than `50` and at least one element of `v7` is less than `100`. The `any()` function is used to check if there is at least one element of `v7` that satisfies a condition, and the `&` operator is used to check if both conditions are `TRUE`. In this case, the first condition `any(v7>50)` is `TRUE` because there is at least one element in `v7` that is greater than `50` (`89`). The second condition `any(v7<100)` is also `TRUE` because all the elements in `v7` are less than `100`. Since both conditions are `TRUE`, the entire expression returns `TRUE`.|


|Matrix| Details|
|--|--|
|`m<-matrix(1:6,nrow=3,ncol=2)`|This command creates a new matrix `m` with 3 rows and 2 columns, and fills it with the values `1, 2, 3, 4, 5, 6`. The `matrix()` function is used to create a matrix with the specified number of rows and columns, and the `nrow` and `ncol` parameters are used to specify the number of rows and columns, respectively. The values to be filled in the matrix are provided as the first argument to `matrix()`, in this case, the values `1:6`.|
|`m<-matrix(1:6,nrow=3,byrow= TRUE)`|This command creates a new matrix `m` with 3 rows and 2 columns, and fills it with the values `1, 2, 3, 4, 5, 6`. The `matrix()` function is used to create a matrix with the specified number of rows and columns, and the `nrow` parameter is used to specify the number of rows. The `byrow` parameter is set to `TRUE` to indicate that the values should be filled in row-wise, rather than column-wise.|
|`dim(m)`|This command returns the dimensions of the matrix `m`, which is a vector with two elements representing the number of rows and columns in the matrix, respectively. In this case, since `m` has 3 rows and 2 columns, the resulting vector is `3 2`. The command `dim(m)` is equivalent to `c(nrow(m), ncol(m))`.|
| `m[2,2]` | This command retrieves the value of the element in the second row and second column of the matrix `m`. In this case, the value is `4`. |
| `m[1,]` | This command retrieves all the values in the first row of the matrix `m`. The comma `,` is used to indicate that we want to retrieve all the columns in the first row. In this case, the resulting vector is `1 2`. |
| `m[,2]` | This command retrieves all the values in the second column of the matrix `m`. The comma `,` is used to indicate that we want to retrieve all the rows in the second column. In this case, the resulting vector is `2 4 6`. |
|`m[c(2,3),]`|This command retrieves all the values in the second and third rows of the matrix `m`. The `c(2,3)` argument is used to specify the row indices we want to retrieve. The comma `,` is used to indicate that we want to retrieve all the columns in the specified rows.|
|`m[m>3]`|This command retrieves all the values in the matrix  `m`  that are greater than  `3`. The logical expression  `m > 3`  is evaluated for each element in the matrix, and returns a matrix of the same dimensions as  `m`  with  `TRUE`  values where the corresponding element in  `m`  is greater than  `3`, and  `FALSE`  values otherwise.The resulting matrix contains all the values in  `m`  that are greater than  `3`, arranged in a vector. In this case, the resulting vector is  `4 5 6`, because those are the values in  `m`  that are greater than  `3`. The resulting vector is arranged in column-major order, which means that the values are listed column by column, starting from the first column.|
|`m>3`|This command returns a logical matrix of the same dimensions as `m`, where each element is `TRUE` if the corresponding element in `m` is greater than `3`, and `FALSE` otherwise. The logical expression `m > 3` is evaluated for each element in the matrix, and returns a matrix of the same dimensions as `m` with `TRUE` values where the corresponding element in `m` is greater than `3`, and `FALSE` values otherwise.|
|`m[m%%2==0]`|This command retrieves all the values in the matrix  `m`  that are even. The expression  `m %% 2 == 0`  is evaluated for each element in the matrix, and returns a matrix of the same dimensions as  `m`  with  `TRUE`  values where the corresponding element in  `m`  is even (i.e. divisible by 2), and  `FALSE`  values otherwise. The resulting matrix contains all the values in  `m`  that are even, arranged in a vector. In this case, the resulting vector is  `2 4 6`, because those are the values in  `m`  that are even. The resulting vector is arranged in column-major order, which means that the values are listed column by column, starting from the first column.|
|`t(m)`|This command transposes the matrix `m`, which means it switches its rows and columns. The `t()` function is used to transpose a matrix. In this case, the resulting matrix has 2 rows and 3 columns. The first row contains the values `1, 3, 5`, and the second row contains the values `2, 4, 6`.  You are correct that if we accidentally set the number of columns as `nrow` and the number of rows as `ncol` while creating a matrix, we can use the `t()` function to transpose the matrix and get the correct orientation.|
|`m * tm`|-   `m * tm`  is element-wise multiplication, also known as the  Hadamard  product. It multiplies each element in  `m`  by the corresponding element in  `tm`, and the resulting matrix has the same dimensions as  `m`  and  `tm`. The resulting matrix is not necessarily a valid matrix product, and its interpretation and use depends on the context of the problem being solved.|
|`m %*% tm`|-   `m %*% tm`  is  matrix multiplication, which performs the  dot product  between each row in  `m`  and each column in  `tm`. It results in a new matrix with the same number of rows as  `m`  and the same number of columns as  `tm`. Matrix multiplication is a fundamental operation in  linear algebra  and is used for a variety of applications, such as solving systems of  linear equations  and computing eigenvectors and eigenvalues.|
|tip for `m %*% tm` and `m * tm` |It's important to note that these are different operations and should not be used interchangeably. The resulting matrices are generally different, and their interpretation and use depend on the context of the problem being solved.|

|Command - Con-cat|Details|
|--|--|
|`m3<-cbind(tm,c(11,12))`|This command creates a new matrix `m3` by column-binding the matrix `tm` with a new vector containing the values `11` and `12`. The `cbind()` function is used to column-bind matrices and vectors together. In this case, since `tm` is a 2x3 matrix and the new vector is a 1x2 vector, the resulting matrix `m3` is a 2x5 matrix. The `cbind()` function aligns the dimensions of the matrices and vectors by filling in missing values with `NA`. The first three columns contain the values from `tm`, and the last two columns contain the values `11` and `12`. Since the new vector only has two values, the third row of `m3` contains `NA` values to fill in the missing values.|
|`m4<-rbind(m3,c(8,8,8)`|This command creates a new matrix  `m4`  by row-binding the matrix  `m3`  with a new vector containing the values  `8, 8, 8`. The  `rbind()`  function is used to row-bind matrices and vectors together. In this case, since  `m3`  is a 2x5 matrix and the new vector is a 1x3 vector, the resulting matrix  `m4`  is a 3x5 matrix. The  `rbind()`  function aligns the dimensions of the matrices and vectors by filling in missing values with  `NA`.|
|`colnames(m4)<-c('col1','col2')` `rownames(m4)<-c('col1','col2','col2','col2','col2')`|These commands assign new row and column names to the matrix `m4`. The command `colnames(m4) <- c('col1', 'col2')` assigns the column names `col1` and `col2` to the two columns of `m4`. The `colnames()` function is used to get or set the column names of a matrix or data frame. In this case, the `c()` function is used to create a character vector containing the new column names. The command `rownames(m4) <- c('col1', 'col2', 'col2', 'col2', 'col2')` assigns the row names `col1`, `col2`, `col2`, `col2`, and `col2` to the five rows of `m4`. The `rownames()` function is used to get or set the row names of a matrix or data frame. In this case, the `c()` function is used to create a character vector containing the new row names.|













> Written with [StackEdit](https://stackedit.io/).
