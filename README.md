practice1
clear;clc;
A=input('请输入分数（用中括号括起来）：')
n=length(A);
s=0;
a=0;b=0;
for i=1:n
    s=s+A(i);
    if A(i)>=90
        a=a+1;
    elseif A(i)<60
        b=b+1;
    end
end
average=s/n;
fprintf('全班人数=%.0f,总得分=%.0f,平均分=%.0f,90分及以上人数%.0f,不及格人数%.0f',n,s,average,a,b)
