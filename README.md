# rrrr
#!/usr/bin/env python
# -*- coding: utf-8 -*-

from subkeys import *

PI =      [58, 50, 42, 34, 26, 18, 10, 2]
PI = PI + [60, 52, 44, 36, 28, 20, 12, 4]
PI = PI + [62, 54, 46, 38, 30, 22, 14, 6]
PI = PI + [64, 56, 48, 40, 32, 24, 16, 8]
PI = PI + [57, 49, 41, 33, 25, 17,  9, 1]
PI = PI + [59, 51, 43, 35, 27, 19, 11, 3]
PI = PI + [61, 53, 45, 37, 29, 21, 13, 5]
PI = PI + [63, 55, 47, 39, 31, 23, 15, 7]

Y =     [32,  1,  2,  3,  4,  5]
Y = Y + [ 4,  5,  6,  7,  8,  9]
Y = Y + [ 8,  9, 10, 11, 12, 13]
Y = Y + [12, 13, 14, 15, 16, 17]
Y = Y + [16, 17, 18, 19, 20, 21]
Y = Y + [20, 21, 22, 23, 24, 25]
Y = Y + [24, 25, 26, 27, 28, 29]
Y = Y + [28, 29, 30, 31, 32,  1]

S1    = [ [], [],  [],  [] ]
S1[0] = [14,  4, 13,  1,  2, 15, 11,  8,  3, 10,  6, 12,  5,  9,  0,  7]
S1[1] = [ 0, 15,  7,  4, 14,  2, 13,  1, 10,  6, 12, 11,  9,  5,  3,  8]
S1[2] = [ 4,  1, 14,  8, 13,  6,  2, 11, 15, 12,  9,  7,  3, 10,  5,  0]
S1[3] = [15, 12,  8,  2,  4,  9,  1,  7,  5, 11,  3, 14, 10,  0,  6, 13]

S2    = [ [], [],  [],  [] ]
S2[0] = [15,  1,  8, 14,  6, 11,  3,  4,  9,  7,  2, 13, 12,  0,  5, 10]
S2[1] = [ 3, 13,  4,  7, 15,  2,  8, 14, 12,  0,  1, 10,  6,  9, 11,  5]
S2[2] = [ 0, 14,  7, 11, 10,  4, 13,  1,  5,  8, 12,  6,  9,  3,  2, 15]
S2[3] = [13,  8, 10,  1,  3, 15,  4,  2, 11,  6,  7, 12,  0,  5, 14,  9]

S3    = [ [], [],  [],  [] ]
S3[0] = [10,  0,  9, 14,  6,  3, 15,  5,  1, 13, 12,  7, 11,  4,  2,  8]
S3[1] = [13,  7,  0,  9,  3,  4,  6, 10,  2,  8,  5, 14, 12, 11, 15,  1]
S3[2] = [13,  6,  4,  9,  8, 15,  3,  0, 11,  1,  2, 12,  5, 10, 14,  7]
S3[3] = [ 1, 10, 13,  0,  6,  9,  8,  7,  4, 15, 14,  3, 11,  5,  2, 12]

S4    = [ [], [],  [],  [] ]
S4[0] = [ 7, 13, 14,  3,  0,  6,  9, 10,  1,  2,  8,  5, 11, 12,  4, 15]
S4[1] = [13,  8, 11,  5,  6, 15,  0,  3,  4,  7,  2, 12,  1, 10, 14,  9]
S4[2] = [10,  6,  9,  0, 12, 11,  7, 13, 15,  1,  3, 14,  5,  2,  8,  4]
S4[3] = [ 3, 15,  0,  6, 10,  1, 13,  8,  9,  4,  5, 11, 12,  7,  2, 14]

S5    = [ [], [],  [],  [] ]
S5[0] = [ 2, 12,  4,  1,  7, 10, 11,  6,  8,  5,  3, 15, 13,  0, 14,  9]
S5[1] = [14, 11,  2, 12,  4,  7, 13,  1,  5,  0, 15, 10,  3,  9,  8,  6]
S5[2] = [ 4,  2,  1, 11, 10, 13,  7,  8, 15,  9, 12,  5,  6,  3,  0, 14]
S5[3] = [11,  8, 12,  7,  1, 14,  2, 13,  6, 15,  0,  9, 10,  4,  5,  3]

S6    = [ [], [],  [],  [] ]
S6[0] = [12,  1, 10, 15,  9,  2,  6,  8,  0, 13,  3,  4, 14,  7,  5, 11]
S6[1] = [10, 15,  4,  2,  7, 12,  9,  5,  6,  1, 13, 14,  0, 11,  3,  8]
S6[2] = [ 9, 14, 15,  5,  2,  8, 12,  3,  7,  0,  4, 10,  1, 13, 11,  6]
S6[3] = [ 4,  3,  2, 12,  9,  5, 15, 10, 11, 14,  1,  7,  6,  0,  8, 13]

S7    = [ [], [],  [],  [] ]
S7[0] = [ 4, 11,  2, 14, 15,  0,  8, 13,  3, 12,  9,  7,  5, 10,  6,  1]
S7[1] = [13,  0, 11,  7,  4,  9,  1, 10, 14,  3,  5, 12,  2, 15,  8,  6]
S7[2] = [ 1,  4, 11, 13, 12,  3,  7, 14, 10, 15,  6,  8,  0,  5,  9,  2]
S7[3] = [ 6, 11, 13,  8,  1,  4, 10,  7,  9,  5,  0, 15, 14,  2,  3, 12]

S8    = [ [], [],  [],  [] ]
S8[0] = [13,  2,  8,  4,  6, 15, 11,  1, 10,  9,  3, 14,  5,  0, 12,  7]
S8[1] = [ 1, 15, 13,  8, 10,  3,  7,  4, 12,  5,  6, 11,  0, 14,  9,  2]
S8[2] = [ 7, 11,  4,  1,  9, 12, 14,  2,  0,  6, 10, 13, 15,  3,  5,  8]
S8[3] = [ 2,  1, 14,  7,  4, 10,  8, 13, 15, 12,  9,  0,  3,  5,  6, 11]

PF =      [16,  7, 20, 21]
PF = PF + [29, 12, 28, 17]
PF = PF + [ 1, 15, 23, 26]
PF = PF + [ 5, 18, 31, 10]
PF = PF + [ 2,  8, 24, 14]
PF = PF + [32, 27,  3,  9]
PF = PF + [19, 13, 30,  6]
PF = PF + [22, 11,  4, 25]

PZ =      [40,  8, 48, 16, 56, 24, 64, 32]
PZ = PZ + [39,  7, 47, 15, 55, 23, 63, 31]
PZ = PZ + [38,  6, 46, 14, 54, 22, 62, 30]
PZ = PZ + [37,  5, 45, 13, 53, 21, 61, 29]
PZ = PZ + [36,  4, 44, 12, 52, 20, 60, 28]
PZ = PZ + [35,  3, 43, 11, 51, 19, 59, 27]
PZ = PZ + [34,  2, 42, 10, 50, 18, 58, 26]
PZ = PZ + [33,  1, 41,  9, 49, 17, 57, 25]

    
def F(R, K):
    
    RY = permuta(Y, R)
    R = XOR(K, RY)
    
    B1 = R[ 0: 6]
    B2 = R[ 6:12]
    B3 = R[12:18]
    B4 = R[18:24]
    B5 = R[24:30]
    B6 = R[30:36]
    B7 = R[36:42]
    B8 = R[42:48]
    
    B1 = intToBin( unBox( S1, binToInt(B1[0]+B1[5]), binToInt(B1[1:5]) ) )[4:]
    B2 = intToBin( unBox( S2, binToInt(B2[0]+B2[5]), binToInt(B2[1:5]) ) )[4:]
    B3 = intToBin( unBox( S3, binToInt(B3[0]+B3[5]), binToInt(B3[1:5]) ) )[4:]
    B4 = intToBin( unBox( S4, binToInt(B4[0]+B4[5]), binToInt(B4[1:5]) ) )[4:]
    B5 = intToBin( unBox( S5, binToInt(B5[0]+B5[5]), binToInt(B5[1:5]) ) )[4:]
    B6 = intToBin( unBox( S6, binToInt(B6[0]+B6[5]), binToInt(B6[1:5]) ) )[4:]
    B7 = intToBin( unBox( S7, binToInt(B7[0]+B7[5]), binToInt(B7[1:5]) ) )[4:]
    B8 = intToBin( unBox( S8, binToInt(B8[0]+B8[5]), binToInt(B8[1:5]) ) )[4:]
    
    R = B1+B2+B3+B4+B5+B6+B7+B8
    
    R = permuta(PF, R)
    
    return R

def DES(M, KN):
    
    BI = permuta(PI, M)
    L0 = BI[0:32]
    R0 = BI[32:64]

    LN = [L0]
    RN = [R0]

    for i in range(1, 17):
        
        LN.append( RN[i-1] )
        
        TR = F(RN[i-1], KN[i])
        TR = XOR(LN[i-1], TR)
        RN.append( TR )

    BF = RN[16]+LN[16]
    return permuta(PZ, BF)

def cifrar(M, K):
    
    KN = getSubKeys(K)
    return DES(M, KN) 

def descifrar(M, K):
    
    KN = getSubKeys(K)
    KN.reverse()
    KN = [KN[-1]]+KN[0:16]
    return DES(M, KN)
