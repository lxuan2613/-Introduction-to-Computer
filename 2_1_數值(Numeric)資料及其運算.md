

-3%2
a = 7//2
b = 7.0//2
c = 7//2.0

a,b,c
5 ** 2
Logical Operators::
x = 5

print(x > 3 and x < 10)
x = 5

print(x > 3 or x < 4)
x = 5

print(not(x > 3 and x < 10))
Bitwise Operators
#!/usr/bin/python3
 
a = 60            # 60 = 0011 1100 
b = 13            # 13 = 0000 1101 
c = 0

print ("0 - a =  60 = 0011 1100(二進位) ")
print ("0 - b =  13 = 0000 1101(二進位) ")
c = a & b;        # 12 = 0000 1100
print ("1 - c = a & b的值為：", c)
 
c = a | b;        # 61 = 0011 1101 
print ("2 - c = a | b的值為：", c)
 
c = a ^ b;        # 49 = 0011 0001
print ("3 - c= a ^ b 的值為：", c)
 
c = ~a;           # -61 = 1100 0011
print ("4 - c = ~a的值為：", c)
 
c = a << 2;       # 240 = 1111 0000
print ("5 - c = a << 2的值為：", c)
 
c = a >> 2;       # 15 = 0000 1111
print ("6 - c = a >> 2的值為：", c)

各種數學函數
https://www.w3schools.com/python/python_ref_functions.asp
作業:完成十種函數的自我測試報告
x = abs(-36)
x
進位轉換
x = bin(36)
x

x = oct(36)
x

x = hex(255)
x

int()函數的測試
https://www.w3schools.com/python/ref_func_int.asp
x=int('10',2)
x

x=int('10',16)
x

x=int('10',8)
x
round()函數的測試
#Round a number to only two decimals:

x = round(5.76543, 2)
print(x)

# Round to the nearest integer:

x = round(5.76543)
print(x)

Python 類型轉換
有時候，我們需要對資料內置的類型進行轉換，
資料類型的轉換只需要將資料類型作為函數名即可。


int(x) 將x轉換為一個整數。
float(x) 將x轉換到一個浮點數。
complex(x) 將x轉換到一個複數，實數部分為 x，虛數部分為 0。
complex(x, y) 將 x 和 y 轉換到一個複數，實數部分為 x，虛數部分為 y。x 和 y 是數字運算式。
a = 1.0004
int(a)

b = 0.9999
int(a)
運算子優先順序
picoCTF 2017 : compute-rsa-50
RSA encryption/decryption is based on a formula that anyone can find and use, 
as long as they know the values to plug in. 
Given the encrypted number 150815, d = 1941, and N = 435979, what is the decrypted number?

HINTS

decrypted = (encrypted) ^ d mod N
