i=imread("C:\Users\BME\Documents\MATLAB\IP_2024 - Copy\DIP3E_Original_Images_CH03\Fig0304(a)(breast_digital_Xray).tif");
subplot(1,2,1),imshow(i);
[r,c]=size(i);
for x=1:r
    for y=1:c
        r=i(x,y);
        s(x,y)=255-r;
    end
end
subplot(1,2,2),imshow(s)
