library(Matrix) #矩陣次方時要用

#Unit 1.2
# 2-6 2-7
A <- matrix(c(1,2,2,1,3,4), nrow =2 , ncol = 3)
B <- matrix(c(1,2,3,0,1,2), nrow =3 , ncol = 2)
C <- matrix(c(3,4,2,-1,1,1,3,5,3), nrow =3 , ncol = 3)
D <- matrix(c(3,2,-2,4), nrow =2 , ncol = 2)
E <- matrix(c(2,0,3,-4,1,2,5,4,1), nrow =3 , ncol = 3)
F <- matrix(c(-4,5,2,3), nrow =2 , ncol = 2)
O <- matrix(c(0,0,0,0,0,0,0,0,0), nrow =3 , ncol = 3)

#2-6
t(A);t(t(A))
t(C+E);t(C)+t(E)
t(2*D+3*F)
D-t(D)
2*t(A)+B
t(3*D-2*F)

#2-7
t(2*A)
t(A-B) #無法執行
t(3*t(B)-2*A)
t(3*t(A)-5*t(B)) #無法執行
t(-1*A);-1*t(A)
t(C+E+t(F)) #無法執行


#2-8 2-9
A <- matrix(c(3,0,0,2), nrow =2 , ncol = 2)
a <- matrix(c(1,0,0,1), nrow =2 , ncol = 2)
b <- matrix(c(1,0,0,0), nrow =2 , ncol = 2)

#2-11 位元矩陣 只由0和1組成 將矩陣餘2的結果就是位元矩陣
A <- matrix(c(1,1,0,0,1,1,1,0,1), nrow =3 , ncol = 3)
B <- matrix(c(0,1,1,1,0,1,1,1,0), nrow =3 , ncol = 3)
C <- matrix(c(1,0,1,1,1,0,0,1,1), nrow =3 , ncol = 3)
(B+C)%%2
(A+B+C)%%2
(A+t(C))%%2
(B-C)%%2

#2-12 位元矩陣
A <- matrix(c(1,1,0,0), nrow =2 , ncol = 2)
B <- matrix(c(1,0,0,1), nrow =2 , ncol = 2)
C <- matrix(c(1,0,1,0), nrow =2 , ncol = 2)
D <- matrix(c(0,1,0,0), nrow =2 , ncol = 2)
(A+B)%%2
(C+D)%%2
(A+B+t(C+D))%%2
(C-B)%%2
(A-B+C-D)%%2



#Unit 1.3
#3-1 內積 a．b
a <- c(1,2);b <- c(4,-1);sum(a*b)
a <- c(-3,-2);b <- c(1,-2);sum(a*b)
a <- c(4,2,-1);b <- c(1,3,6);sum(a*b)
a <- c(1,1,0);b <- c(1,0,1);sum(a*b)

#3-4 內積 w．w 以隨機變數表示x是未知數
x <- sample(0.0:6.28,1,replace = TRUE)
w <- c(sin(x),cos(x));sum(w*w)

#3-8 矩陣乘法 及 規則
A <- matrix(c(1,4,2,0,-3,-2), nrow =2 , ncol = 3)
B <- matrix(c(3,2,-1,1,4,5), nrow =3 , ncol = 2)
C <- matrix(c(2,3,1,3,-4,-1,1,5,-2), nrow =3 , ncol = 3)
D <- matrix(c(2,-1,3,-2), nrow =2 , ncol = 2)
E <- matrix(c(1,-2,3,0,1,4,-3,5,2), nrow =3 , ncol = 3)
F <- matrix(c(2,4,-3,1), nrow =2 , ncol = 2)
A%*%(B%*%D);(A%*%B)%*%D
A%*%(C+E);A%*%C+A%*%E
(D+F)%*%A

#3-10 單位矩陣乘法規則
I <- diag(1, 2) #單位矩陣
D <- matrix(c(2,-1,3,-2), nrow =2 , ncol = 2)
D%*%I;I%*%D

#3-13
A <- matrix(c(1,3,4,2,-1,2,-2,1,2,4,3,5), nrow =4 , ncol = 3)
B <- matrix(c(1,3,4,0,3,2,-1,-3,5,2,4,1), nrow =3 , ncol = 4)
A%*%B[,1] #AB the first column
A%*%B[,3] #AB the third column

#3-17 證明AB 等同於 row1(A)B,row2(A)B
A <- matrix(c(2,1,-3,2,1,4), nrow =2 , ncol = 3)
B <- matrix(c(3,5,2), nrow =3 , ncol = 1)
A%*%B == rbind((A[1,]%*%B),A[2,]%*%B)

#3-T4 T5 T7 證明對角矩陣 AB=BA
x <- sample(0:10,1,replace = TRUE)
y <- sample(0:10,1,replace = TRUE)
I <- sample(0:5,1,replace = TRUE)
A <- diag(x,I);B <- diag(y,I)
A;B;A%*%B;A%*%B==B%*%A



#Unit 1.4 
#4-9 矩陣乘法
A <- matrix(c(2,3,1,2,-2,5), nrow =2 , ncol = 3)
B <- matrix(c(2,3,1,-1,4,-2), nrow =3 , ncol = 2)
C <- matrix(c(2,-1,3,1,2,1,3,4,0), nrow =3 , ncol = 3)
D <- matrix(c(2,-3,-1,2), nrow =2 , ncol = 2)
E <- matrix(c(1,2,-3,1,-1,2,2,3,-1), nrow =3 , ncol = 3)
F <- matrix(c(1,2,0,-3), nrow =2 , ncol = 2)
t(3*C-2*E)%*%B
t(A)%*%(D+F)
t(B)%*%C+A
(2*E)%*%t(A)
(t(B)+A)%*%C

#4-13 矩陣次方
A <- matrix(c(4,1,2,3), nrow =2 , ncol = 2)
I <- diag(1, 2) #單位矩陣
A%*%A+3*A #A^2+3A
2*(A%*%A%*%A)+3*(A%*%A)+4*A+5*I #2A^3+3A^2+4A+5I

#4-14 矩陣次方
A <- matrix(c(1,2,-1,3), nrow =2 , ncol = 2)
I <- diag(1, 2) #單位矩陣
A%*%A-2*A #A^2-2A
3*(A%*%A%*%A)-2*(A%*%A)+5*A-4*I #3A^3-2A^2+5A-4I

#4-22 證明位元矩陣A^2=0
A <- matrix(c(1,1,1,1), nrow =2 , ncol = 2)
(A%*%A)%%2;(A%*%A)%%2==0

#4-23 證明位元矩陣A^2=I
A <- matrix(c(1,0,1,1), nrow =2 , ncol = 2)
I <- diag(1, 2) #單位矩陣
(A%*%A)%%2;(A%*%A)%%2==I

#4-24 位元矩陣計算
A <- matrix(c(0,0,1,1), nrow =2 , ncol = 2)
(A%*%A-A)%%2
(A%*%A%*%A+A%*%A+A)%%2

#4-25 位元矩陣計算
A <- matrix(c(0,1,0,1), nrow =2 , ncol = 2)
(A%*%A-A)%%2
(A%*%A%*%A%*%A+A%*%A%*%A+A%*%A)%%2



#Unit 1.5
#5-1 矩陣轉換 f(u)=Au 對X軸反射
A <- matrix(c(1,0,0,-1), nrow =2 , ncol = 2)
u <- matrix(c(2,3), nrow =2 , ncol = 1)
A%*%u

#5-2 矩陣轉換 f(u)=Au 對Y軸反射
A <- matrix(c(-1,0,0,1), nrow =2 , ncol = 2)
u <- matrix(c(1,-2), nrow =2 , ncol = 1)
A%*%u

#5-3 矩陣轉換 f(u)=Au 逆時針旋轉30度(pi/6)
A <- matrix(c(cos(pi/6),sin(pi/6),-1*sin(pi/6),cos(pi/6)), nrow =2 , ncol = 2)
u <- matrix(c(-1,3), nrow =2 , ncol = 1)
A%*%u

#5-4 矩陣轉換 f(u)=Au 逆時針旋轉120度(2*pi/3)
A <- matrix(c(cos(2*pi/3),sin(2*pi/3),-1*sin(2*pi/3),cos(2*pi/3)), nrow =2 , ncol = 2)
u <- matrix(c(-2,-3), nrow =2 , ncol = 1)
A%*%u

#5-5 矩陣轉換 f(u)=Au 對原點反射
A <- matrix(c(-1,0,0,-1), nrow =2 , ncol = 2)
u <- matrix(c(3,2), nrow =2 , ncol = 1)
A%*%u

#5-6 矩陣轉換 f(u)=Au 伸縮
A <- matrix(c(2,0,0,2), nrow =2 , ncol = 2)
u <- matrix(c(-3,3), nrow =2 , ncol = 1)
A%*%u

#5-7 矩陣轉換 f(u)=Au 投射
A <- matrix(c(1,1,0,0,-1,0,0,0,0), nrow =3 , ncol = 3)
u <- matrix(c(2,-1,3), nrow =3 , ncol = 1)
A%*%u

#5-8 矩陣轉換 f(u)=Au 投射
A <- matrix(c(1,-1,0,0,1,0,1,0,1), nrow =3 , ncol = 3)
u <- matrix(c(0,-2,4), nrow =3 , ncol = 1)
A%*%u

#5-9 矩陣轉換 f(x)=Ax=w 問w是否在f的值域中(x=a^-1w)
A <- matrix(c(1,-1,3,2), nrow =2 , ncol = 2)
w <- matrix(c(7,3), nrow =2 , ncol = 1)
solve(A)%*%w

#5-15-17 描述給定A之下，對應f的幾何意義 (假設f(u)=Au)
u <- matrix(c(1,2), nrow =2 , ncol = 1)
#5-15.a 對Y軸反射
A <- matrix(c(-1,0,0,1), nrow =2 , ncol = 2)
A%*%u
#5-15.b 逆時針旋轉90度(pi/2)
A <- matrix(c(0,1,-1,0), nrow =2 , ncol = 2)
A%*%u
#5-16.a 對x=y軸反射
A <- matrix(c(0,1,1,0), nrow =2 , ncol = 2)
A%*%u
#5-16.b 對x=-y軸反射
A <- matrix(c(0,-1,-1,0), nrow =2 , ncol = 2)
A%*%u
#5-17.a 投射到x軸
A <- matrix(c(1,0,0,0), nrow =2 , ncol = 2)
A%*%u
#5-17.b 投射到y軸
A <- matrix(c(0,0,0,1), nrow =2 , ncol = 2)
A%*%u

#5-19 f(u)=Au 逆時針旋轉30度(pi/6) 描述g(u)的幾何意義
A <- matrix(c(cos(pi/6),sin(pi/6),-1*sin(pi/6),cos(pi/6)), nrow =2 , ncol = 2)
u <- matrix(c(1,2), nrow =2 , ncol = 1) #假設u
#g(u)=(A^2)u 逆時針旋轉60度
(A%*%A)%*%u
#g(u)=(A^3)u 逆時針旋轉90度
(A%^%A%*%A)%*%u
#g(u)=(A^k)u 逆時針旋轉360度 k=12



#Unit 1.6
library(cmna) #梯形矩陣要用
library(pracma) #化約梯形矩陣要用
#6-9 行列間轉換
C <- matrix(c(1,-3,4,5,0,1,2,-1,3,4,2,5), nrow =4 , ncol = 3)
#r2 <=> r4
A<-C;B<-A[2,];A[2,]<-A[4,];A[4,]<-B;A
#r3*3
A<-C;A[3,]<-A[3,]*3;A
#r4 <= r1*-3
A<-C;A[4,]<-A[1,]*-3;A

#6-13 階梯形矩陣
A <- matrix(c(0,2,1,3,-1,3,3,2,2,4,-1,4,3,5,2,1), nrow =4 , ncol = 4)
refmatrix(A)

#6-15 階梯形矩陣
A <- matrix(c(1,-1,0,2,2,0,1,3,-3,3,2,0,1,4,-1,3), nrow =4 , ncol = 4)
refmatrix(A)

#6-17 6-13的化約列梯形矩陣
A <- matrix(c(0,2,1,3,-1,3,3,2,2,4,-1,4,3,5,2,1), nrow =4 , ncol = 4)
rref(A)

#6-17 6-15的化約列梯形矩陣
A <- matrix(c(1,-1,0,2,2,0,1,3,-3,3,2,0,1,4,-1,3), nrow =4 , ncol = 4)
rref(A)

#6-27 用高斯消去法解線性方程組 Ax = b [A b]=>[I x]
Ab <- matrix(c(1,1,0,1,1,1,1,0,1,0,3,1), nrow =3 , ncol = 4)
x<-rref(Ab)[,4];x
Ab <- matrix(c(1,1,1,1,2,1,1,3,3,1,2,3,0,0,0,0), nrow =4 , ncol = 4)
x<-rref(Ab)[,4];x

#6-27 用高斯消去法解線性方程組 Ax = b [A b]=>[I x]
Ab <- matrix(c(1,1,1,2,3,0,3,0,2,1,1,1,8,7,3), nrow =3 , ncol = 5)
x<-rref(Ab)[,4:5];x #無限多組解
Ab <- matrix(c(1,2,3,3,-2,-1,0,-3,3,-3,1,0,4,5,2,7), nrow =4 , ncol = 4)
x<-rref(Ab);x #無解

#6-31