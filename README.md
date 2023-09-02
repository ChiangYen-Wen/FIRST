# START
#HW_WeeK3-1.py

#轉帳金額確認

A = int(input())
B = int(input())
M = int(input())

if ( M < A ) :
    print(A-M , B+M)
else:
    print(0, B+A)
