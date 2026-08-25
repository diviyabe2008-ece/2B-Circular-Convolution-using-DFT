# EXPT 2B:CIRCULAR-CONVOLUTION-USING-DFT
## AIM
To perform and verify circular convolution operation of two given sequences using SCILAB.

## APPARATUS REQUIRED
PC installed with SCILAB

## PROGRAM:
## CIRCULAR CONVOLUTION
```
clc; clear;
x=[1 1 1 1];
n1=0:1:length(x)-1;
subplot(3,1,1);
plot2d3(n1,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
h=[1 2 3];
n2=0:1:length(h)-1;
subplot(3,1,2);
plot2d3(n2,h);
xlabel('time');
ylabel('amplitude');
title('impulse sequence');
N1=length(x);
N2=length(h);
N=max(N1,N2);
N3=N1-N2;
if(N3>0)
h=[h,zeros(1,N3)];
else
x=[x,zeros(1,abs(N3))];
end
disp(x)
disp(h)
for n=1:N
y(n)=0;
for i=1:N
j=n-i+1;
if(j<=0)
j=N+j;
end
y(n)=y(n)+x(i)*h(j);
end
end
disp(y)
n=0:N-1;
subplot(3,1,3);
plot2d3(n,y);
xlabel('time');
ylabel('amplitude');
title('circular convolution');
```

### CALCULATIONS:
<img width="994" height="1601" alt="image" src="https://github.com/user-attachments/assets/56e32f1e-90b6-4237-8109-d60b071b0991" />

### SAMPLE OUTPUT:
<img width="745" height="670" alt="image" src="https://github.com/user-attachments/assets/8d4065da-0103-43e4-b871-468fd98d7e1a" />



## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.


## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.

## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.

## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.
## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.
## RESULT:
Thus, the circular convolution of the two given sequences were performed and its result was verified.

