t=linspace(0,2*pi);
t(8:44)=[]; 
x=3*cos(t);
y=10*sin(t);
yh=linspace(min(y)+0.1,-20);
xh=zeros(size(yh));
figure('color','k')
patch(x,y,'w')
hold on
patch(x(y<0),y(y<0),[247 231 206]/255,'EdgeColor','none')
patch([0 -2 2],[-19.5 -20.5 -20.5],'w')
plot(xh,yh,'w','LineW',5)
axis equal off