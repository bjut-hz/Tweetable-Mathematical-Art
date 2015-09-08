# Tweetable-Mathematical-Art
使用指定长度代码生成一张图片
# 示例
###Martin Büttner 的作品
```
unsigned char RD(int i,int j){
return (char)(_sq(cos(atan2(j-512,i-512)/2))*255);
}
 
unsigned char GR(int i,int j){
return (char)(_sq(cos(atan2(j-512,i-512)/2-2*acos(-1)/3))*255);
}
 
unsigned char BL(int i,int j){
return (char)(_sq(cos(atan2(j-512,i-512)/2+2*acos(-1)/3))*255);
}
```
效果图：

![Tweetable Mathematical Art](http://www.matrix67.com/blogimage_2014/201408121.png "Martin Büttner")

###githubphagocyte 的作品
```
unsigned char RD(int i,int j){
float s=3./(j+99);
float y=(j+sin((i*i+_sq(j-700)*5)/100./DIM)*35)*s;
return (int((i+DIM)*s+y)%2+int((DIM*2-i)*s+y)%2)*127;
}
 
unsigned char GR(int i,int j){
float s=3./(j+99);
float y=(j+sin((i*i+_sq(j-700)*5)/100./DIM)*35)*s;
return (int(5*((i+DIM)*s+y))%2+int(5*((DIM*2-i)*s+y))%2)*127;
}
 
unsigned char BL(int i,int j){
float s=3./(j+99);
float y=(j+sin((i*i+_sq(j-700)*5)/100./DIM)*35)*s;
return (int(29*((i+DIM)*s+y))%2+int(29*((DIM*2-i)*s+y))%2)*127;
}
```
效果图：

![Tweetable Mathematical Art](http://www.matrix67.com/blogimage_2014/201408123.png "githubphagocyte")
