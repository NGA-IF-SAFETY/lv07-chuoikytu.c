#**CHUỖI KÍ TỰ**  
##I.*khái niệm*  
- Chuỗi ký tự là một dãy gồm các ký tự hoặc một mảng các ký tự được kết thúc bằng ký tự '\0'   
- Các hằng chuỗi ký tự được đặt trong cặp dấu nháy kép ""   
- Mỗi ký tự của chuỗi được chứa trong một phần tử của mảng   
- *Cách khai báo chuỗi*:   

       +char ten_chuoi[];  
       +char *ten_chuoi;  
##II.*các thao tác trên chuỗi*   
-Ðể thực hiện các thao tác trên chuỗi ta sử dụng một thư viện các hàm chuẩn là <string.h>.   
**NHẬP XUẤT CHUỖI KÍ TỰ**   

1.*nhập chuỗi từ bàn phím*
- Để nhập một chuỗi ký tự từ bàn phím, ta sử dụng hàm gets()  

- Cú pháp: gets(<Biến chuỗi>)   

Ví dụ:   

char Ten[20];   
gets(Ten);   
- Ta cũng có thể sử dụng hàm scanf() để nhập dữ liệu cho biến chuỗi, tuy nhiên lúc này ta chỉ có thể nhập được một chuỗi không có dấu khoảng trắng.   

- Ngoài ra, hàm cgets() (trong conio.h) cũng được sử dụng để nhập chuỗi.    

2.*xuất chuỗi từ bàn phím*   

- Để xuất một chuỗi (biểu thức chuỗi) lên màn hình, ta sử dụng hàm puts().
- Cú pháp: puts(`<Biểu thức chuỗi>`)
Ví dụ: Nhập vào một chuỗi và hiển thị trên màn hình chuỗi vừa nhập.   

`#include<conio.h>`   
 
`#include<stdio.h>`    
 
`#include<string.h>`   
 
int main()    

{   
  
    char Ten[12];   
 
    char queQuan[15];   
 
    printf("Nhap Ten: "); fflush(stdin); gets(Ten);

    printf("Nhap Que Quan: "); fflush(stdin); gets(queQuan);
 
    printf("Chuoi vua nhap: "); puts(Ten); puts(queQuan);

    getch();
 
    return 0;   
 
}    

###CÁC HÀM XỬ LÝ TRONG CHUỖI :   

1.Hàm strcpy:  

- Công dụng: sao chép chuỗi nguồn vào chuỗi đích.
- Cấu trúc:

char*strcpy(char *dich, char *nguon);   

- Có nghĩa là khi ta nhập vào một dãy các kí tự ở chuỗi nguồn thì nó sẽ sao chép tất cả các kí tự vừa nhập vào cái chuỗi đích.   

2.Hàm strncpy:  

- Công dụng: sao chép n kí tự đầu tiên của chuỗi nguồn vào chuỗi đích.  

- Cấu trúc:

 char *strncpy(char *dich, char *nguon,int n);   
 
 3.Hàm strlen:   
 
- Công dụng :cho biết độ dài của chuỗi s   

- Cấu trúc:   

int strlen(char *s);  

4.Hàm strcat:  
 
Công dụng: ghép chuỗi nguồn vào sau chuỗi đích.  

Cấu trúc:

char *strcat(char *dich,char *nguon);  

5.Hàm strncat:   

Công dụng: ghép n kí tự đầu tiên của chuỗi vào sau chuỗi đích  

Cấu trúc:

char *strncat(char *dich,char *nguon,int n);  

6.Hàm strcmp:   

- Công dụng: so sánh 2 chuỗi s1 và s2   

- Cấu trúc:
int strcmp(char *s1,char *s2);  

- Hàm sẽ trả về 1 trong các giá trị sau:
-Giá trị âm: nếu chuỗi s1 nhỏ hơn chuỗi s2   
-Giá trị 0 : nếu hai chuỗi bằng nhau   
-Giá trị dương : nếu chuỗi s1 lớn hơn chuỗi s2    

7.Hàm strstr:   

- Công dụng: trả về địa chỉ vị trí xuất hiện đầu tiên của chuỗi s1 trong chuỗi s và sẽ trả về giá trị NULL trong trường hợp không tìm thấy.  

- Cấu trúc:  
char *strstr(char *s, char *s1);     

8.Hàm strrchr:   
- Công dụng: trả về địachỉ vị trí xuất hiện cuối cùng của kí tự ch trong chuỗi s. Nếu không tìm thấy hàm sẽ trả về giá trị NULL   

- Cấu trúc:   
char *strrchr(char *s,char ch);   

##III.*MẢNG VÀ CHUỖI KÍ TỰ*    

- Một dạng sử dụng con trỏ đặc biệt là việc sử dụng một mảng các biến con trỏ    

-cú pháp: type *pointer_array[size];     
 
 ví dụ:char*temp[5];


 
 
 




