All implemented (readable) vendor-specific registers. Dumped on an icestorm core, while running m1n1 (after chicken bits):

```
s3_0_c15_c0_1 (3, 0, 15, 0, 1) = 0x7180080006000000
s3_0_c15_c1_1 (3, 0, 15, 1, 1) = 0x129802000000
s3_0_c15_c1_2 (3, 0, 15, 1, 2) = 0x618100
s3_0_c15_c1_4 (3, 0, 15, 1, 4) = 0xce8e19f3b0a04081
s3_0_c15_c1_5 (3, 0, 15, 1, 5) = 0x19d1c3862c081
s3_0_c15_c2_1 (3, 0, 15, 2, 1) = 0x0
s3_0_c15_c3_1 (3, 0, 15, 3, 1) = 0x2030001fe0
s3_0_c15_c4_1 (3, 0, 15, 4, 1) = 0x100000000800
s3_0_c15_c5_0 (3, 0, 15, 5, 0) = 0x2082df50e700df14
s3_0_c15_c6_0 (3, 0, 15, 6, 0) = 0x7dc8031f007f0e
s3_0_c15_c7_1 (3, 0, 15, 7, 1) = 0x0
s3_0_c15_c8_0 (3, 0, 15, 8, 0) = 0x381c109438000135
s3_0_c15_c9_1 (3, 0, 15, 9, 1) = 0x600000811
s3_0_c15_c10_1 (3, 0, 15, 10, 1) = 0x3000528002788
s3_0_c15_c10_2 (3, 0, 15, 10, 2) = 0x40032014
s3_0_c15_c11_1 (3, 0, 15, 11, 1) = 0x30000000010
s3_0_c15_c11_3 (3, 0, 15, 11, 3) = 0x0
s3_0_c15_c12_0 (3, 0, 15, 12, 0) = 0xe10000000e020
s3_0_c15_c12_1 (3, 0, 15, 12, 1) = 0x1800
s3_0_c15_c12_2 (3, 0, 15, 12, 2) = 0x40201008040201
s3_0_c15_c13_0 (3, 0, 15, 13, 0) = 0x0
s3_0_c15_c15_3 (3, 0, 15, 15, 3) = 0x20402000000
s3_0_c15_c15_5 (3, 0, 15, 15, 5) = 0x54090afcfa9
s3_1_c15_c0_0 (3, 1, 15, 0, 0) = 0x0
s3_1_c15_c0_1 (3, 1, 15, 0, 1) = 0x0
s3_1_c15_c0_2 (3, 1, 15, 0, 2) = 0x6
s3_1_c15_c0_3 (3, 1, 15, 0, 3) = 0x0
s3_1_c15_c0_4 (3, 1, 15, 0, 4) = 0x0
s3_1_c15_c1_0 (3, 1, 15, 1, 0) = 0x0
s3_1_c15_c1_2 (3, 1, 15, 1, 2) = 0x0
s3_1_c15_c1_3 (3, 1, 15, 1, 3) = 0x0
s3_1_c15_c1_4 (3, 1, 15, 1, 4) = 0x0
s3_1_c15_c2_0 (3, 1, 15, 2, 0) = 0x0
s3_1_c15_c2_2 (3, 1, 15, 2, 2) = 0x0
s3_1_c15_c2_3 (3, 1, 15, 2, 3) = 0x0
s3_1_c15_c3_0 (3, 1, 15, 3, 0) = 0x0
s3_1_c15_c3_2 (3, 1, 15, 3, 2) = 0x0
s3_1_c15_c3_3 (3, 1, 15, 3, 3) = 0x0
s3_1_c15_c4_0 (3, 1, 15, 4, 0) = 0x0
s3_1_c15_c4_2 (3, 1, 15, 4, 2) = 0x6
s3_1_c15_c4_3 (3, 1, 15, 4, 3) = 0x0
s3_1_c15_c5_0 (3, 1, 15, 5, 0) = 0x0
s3_1_c15_c5_2 (3, 1, 15, 5, 2) = 0x0
s3_1_c15_c5_3 (3, 1, 15, 5, 3) = 0x0
s3_1_c15_c6_0 (3, 1, 15, 6, 0) = 0x0
s3_1_c15_c6_2 (3, 1, 15, 6, 2) = 0x0
s3_1_c15_c6_3 (3, 1, 15, 6, 3) = 0x0
s3_1_c15_c7_0 (3, 1, 15, 7, 0) = 0x0
s3_1_c15_c7_2 (3, 1, 15, 7, 2) = 0x0
s3_1_c15_c7_3 (3, 1, 15, 7, 3) = 0x0
s3_1_c15_c8_0 (3, 1, 15, 8, 0) = 0x0
s3_1_c15_c8_3 (3, 1, 15, 8, 3) = 0x0
s3_1_c15_c9_0 (3, 1, 15, 9, 0) = 0x0
s3_1_c15_c9_2 (3, 1, 15, 9, 2) = 0x6
s3_1_c15_c9_3 (3, 1, 15, 9, 3) = 0x0
s3_1_c15_c10_0 (3, 1, 15, 10, 0) = 0x0
s3_1_c15_c10_2 (3, 1, 15, 10, 2) = 0x0
s3_1_c15_c10_3 (3, 1, 15, 10, 3) = 0x0
s3_1_c15_c11_0 (3, 1, 15, 11, 0) = 0xfffff
s3_1_c15_c11_3 (3, 1, 15, 11, 3) = 0x0
s3_1_c15_c12_0 (3, 1, 15, 12, 0) = 0x0
s3_1_c15_c12_3 (3, 1, 15, 12, 3) = 0x0
s3_1_c15_c13_0 (3, 1, 15, 13, 0) = 0x0
s3_1_c15_c13_3 (3, 1, 15, 13, 3) = 0x0
s3_1_c15_c14_0 (3, 1, 15, 14, 0) = 0x0
s3_1_c15_c14_1 (3, 1, 15, 14, 1) = 0x0
s3_1_c15_c14_3 (3, 1, 15, 14, 3) = 0x0
s3_1_c15_c15_0 (3, 1, 15, 15, 0) = 0x0
s3_1_c15_c15_3 (3, 1, 15, 15, 3) = 0x0
s3_2_c15_c0_0 (3, 2, 15, 0, 0) = 0x0
s3_2_c15_c0_1 (3, 2, 15, 0, 1) = 0x0
s3_2_c15_c0_2 (3, 2, 15, 0, 2) = 0x0
s3_2_c15_c0_3 (3, 2, 15, 0, 3) = 0x0
s3_2_c15_c0_4 (3, 2, 15, 0, 4) = 0x0
s3_2_c15_c0_5 (3, 2, 15, 0, 5) = 0x0
s3_2_c15_c0_6 (3, 2, 15, 0, 6) = 0x0
s3_2_c15_c0_7 (3, 2, 15, 0, 7) = 0x0
s3_2_c15_c1_0 (3, 2, 15, 1, 0) = 0x0
s3_2_c15_c1_1 (3, 2, 15, 1, 1) = 0x0
s3_2_c15_c2_0 (3, 2, 15, 2, 0) = 0x0
s3_2_c15_c3_0 (3, 2, 15, 3, 0) = 0x0
s3_2_c15_c4_0 (3, 2, 15, 4, 0) = 0x0
s3_2_c15_c5_0 (3, 2, 15, 5, 0) = 0x0
s3_2_c15_c6_0 (3, 2, 15, 6, 0) = 0x0
s3_2_c15_c7_0 (3, 2, 15, 7, 0) = 0x0
s3_2_c15_c9_0 (3, 2, 15, 9, 0) = 0x0
s3_2_c15_c10_0 (3, 2, 15, 10, 0) = 0x0
s3_2_c15_c12_0 (3, 2, 15, 12, 0) = 0x0
s3_2_c15_c13_0 (3, 2, 15, 13, 0) = 0x0
s3_2_c15_c14_0 (3, 2, 15, 14, 0) = 0x0
s3_2_c15_c15_0 (3, 2, 15, 15, 0) = 0x0
s3_3_c15_c0_4 (3, 3, 15, 0, 4) = 0x0
s3_3_c15_c0_5 (3, 3, 15, 0, 5) = 0x0
s3_3_c15_c0_6 (3, 3, 15, 0, 6) = 0x0
s3_3_c15_c1_4 (3, 3, 15, 1, 4) = 0x0
s3_3_c15_c1_5 (3, 3, 15, 1, 5) = 0x0
s3_3_c15_c1_6 (3, 3, 15, 1, 6) = 0x0
s3_3_c15_c2_0 (3, 3, 15, 2, 0) = 0x0
s3_3_c15_c2_4 (3, 3, 15, 2, 4) = 0x0
s3_3_c15_c2_5 (3, 3, 15, 2, 5) = 0x0
s3_3_c15_c3_0 (3, 3, 15, 3, 0) = 0x60
s3_3_c15_c3_4 (3, 3, 15, 3, 4) = 0x0
s3_3_c15_c3_5 (3, 3, 15, 3, 5) = 0x0
s3_3_c15_c4_0 (3, 3, 15, 4, 0) = 0x0
s3_3_c15_c4_4 (3, 3, 15, 4, 4) = 0x0
s3_3_c15_c4_5 (3, 3, 15, 4, 5) = 0x0
s3_3_c15_c4_6 (3, 3, 15, 4, 6) = 0x3ffffffffff
s3_3_c15_c5_0 (3, 3, 15, 5, 0) = 0x0
s3_3_c15_c5_5 (3, 3, 15, 5, 5) = 0x0
s3_3_c15_c6_5 (3, 3, 15, 6, 5) = 0x0
s3_3_c15_c7_0 (3, 3, 15, 7, 0) = 0xf1200
s3_3_c15_c7_5 (3, 3, 15, 7, 5) = 0x0
s3_3_c15_c8_0 (3, 3, 15, 8, 0) = 0x11000ffc00000000
s3_3_c15_c8_1 (3, 3, 15, 8, 1) = 0x1
s3_3_c15_c8_2 (3, 3, 15, 8, 2) = 0x1
s3_3_c15_c8_3 (3, 3, 15, 8, 3) = 0x4
s3_3_c15_c9_0 (3, 3, 15, 9, 0) = 0x0
s3_3_c15_c10_0 (3, 3, 15, 10, 0) = 0x0
s3_3_c15_c11_0 (3, 3, 15, 11, 0) = 0x0
s3_3_c15_c12_0 (3, 3, 15, 12, 0) = 0xfffffffff
s3_3_c15_c13_0 (3, 3, 15, 13, 0) = 0x238018600bc0024
s3_3_c15_c13_1 (3, 3, 15, 13, 1) = 0x84005a002c0008
s3_3_c15_c13_2 (3, 3, 15, 13, 2) = 0x1c8014e00a60024
s3_3_c15_c13_3 (3, 3, 15, 13, 3) = 0x6a004e00260008
s3_3_c15_c13_4 (3, 3, 15, 13, 4) = 0x20000
s3_3_c15_c13_5 (3, 3, 15, 13, 5) = 0x40000
s3_3_c15_c13_6 (3, 3, 15, 13, 6) = 0x80000
s3_3_c15_c13_7 (3, 3, 15, 13, 7) = 0x100000
s3_3_c15_c14_0 (3, 3, 15, 14, 0) = 0xf0000
s3_3_c15_c15_0 (3, 3, 15, 15, 0) = 0x4ad4b4c00
s3_3_c15_c15_1 (3, 3, 15, 15, 1) = 0x352b4b200
s3_3_c15_c15_2 (3, 3, 15, 15, 2) = 0x10000
s3_3_c15_c15_3 (3, 3, 15, 15, 3) = 0x20000
s3_3_c15_c15_4 (3, 3, 15, 15, 4) = 0x8d48e9f929042518
s3_4_c15_c0_2 (3, 4, 15, 0, 2) = 0x0
s3_4_c15_c0_3 (3, 4, 15, 0, 3) = 0x7f
s3_4_c15_c0_4 (3, 4, 15, 0, 4) = 0xc
s3_4_c15_c0_5 (3, 4, 15, 0, 5) = 0x0
s3_4_c15_c0_7 (3, 4, 15, 0, 7) = 0x0
s3_4_c15_c1_0 (3, 4, 15, 1, 0) = 0x0
s3_4_c15_c1_1 (3, 4, 15, 1, 1) = 0x0
s3_4_c15_c1_2 (3, 4, 15, 1, 2) = 0x0
s3_4_c15_c1_3 (3, 4, 15, 1, 3) = 0x0
s3_4_c15_c1_4 (3, 4, 15, 1, 4) = 0x100
s3_4_c15_c1_5 (3, 4, 15, 1, 5) = 0x0
s3_4_c15_c1_6 (3, 4, 15, 1, 6) = 0x0
s3_4_c15_c1_7 (3, 4, 15, 1, 7) = 0x0
s3_4_c15_c2_2 (3, 4, 15, 2, 2) = 0x0
s3_4_c15_c2_3 (3, 4, 15, 2, 3) = 0x80485c000
s3_4_c15_c2_4 (3, 4, 15, 2, 4) = 0x804924000
s3_4_c15_c2_5 (3, 4, 15, 2, 5) = 0x0
s3_4_c15_c2_6 (3, 4, 15, 2, 6) = 0x0
s3_4_c15_c2_7 (3, 4, 15, 2, 7) = 0x0
s3_4_c15_c3_0 (3, 4, 15, 3, 0) = 0x0
s3_4_c15_c3_1 (3, 4, 15, 3, 1) = 0x0
s3_4_c15_c3_2 (3, 4, 15, 3, 2) = 0x0
s3_4_c15_c3_3 (3, 4, 15, 3, 3) = 0x0
s3_4_c15_c3_4 (3, 4, 15, 3, 4) = 0x0
s3_4_c15_c3_5 (3, 4, 15, 3, 5) = 0x0
s3_4_c15_c3_6 (3, 4, 15, 3, 6) = 0x0
s3_4_c15_c3_7 (3, 4, 15, 3, 7) = 0x0
s3_4_c15_c4_0 (3, 4, 15, 4, 0) = 0x4
s3_4_c15_c4_6 (3, 4, 15, 4, 6) = 0x0
s3_4_c15_c4_7 (3, 4, 15, 4, 7) = 0x100
s3_4_c15_c5_0 (3, 4, 15, 5, 0) = 0x0
s3_4_c15_c5_6 (3, 4, 15, 5, 6) = 0x0
s3_4_c15_c5_7 (3, 4, 15, 5, 7) = 0x0
s3_4_c15_c6_0 (3, 4, 15, 6, 0) = 0x0
s3_4_c15_c6_1 (3, 4, 15, 6, 1) = 0x0
s3_4_c15_c6_2 (3, 4, 15, 6, 2) = 0x0
s3_4_c15_c6_3 (3, 4, 15, 6, 3) = 0x0
s3_4_c15_c6_4 (3, 4, 15, 6, 4) = 0x80485c000
s3_4_c15_c6_5 (3, 4, 15, 6, 5) = 0x804924000
s3_4_c15_c6_6 (3, 4, 15, 6, 6) = 0x0
s3_4_c15_c6_7 (3, 4, 15, 6, 7) = 0x0
s3_4_c15_c9_0 (3, 4, 15, 9, 0) = 0x0
s3_4_c15_c9_1 (3, 4, 15, 9, 1) = 0x0
s3_4_c15_c9_2 (3, 4, 15, 9, 2) = 0x0
s3_4_c15_c9_3 (3, 4, 15, 9, 3) = 0x0
s3_4_c15_c9_4 (3, 4, 15, 9, 4) = 0x0
s3_4_c15_c9_5 (3, 4, 15, 9, 5) = 0x0
s3_4_c15_c10_4 (3, 4, 15, 10, 4) = 0x3
s3_4_c15_c10_5 (3, 4, 15, 10, 5) = 0xfb8de8634
s3_4_c15_c10_6 (3, 4, 15, 10, 6) = 0xfb8de8634
s3_4_c15_c11_0 (3, 4, 15, 11, 0) = 0x0
s3_4_c15_c11_1 (3, 4, 15, 11, 1) = 0x0
s3_4_c15_c11_2 (3, 4, 15, 11, 2) = 0x0
s3_4_c15_c11_3 (3, 4, 15, 11, 3) = 0x0
s3_4_c15_c11_4 (3, 4, 15, 11, 4) = 0x0
s3_4_c15_c11_5 (3, 4, 15, 11, 5) = 0x0
s3_4_c15_c12_5 (3, 4, 15, 12, 5) = 0x0
s3_4_c15_c12_7 (3, 4, 15, 12, 7) = 0x0
s3_5_c15_c0_2 (3, 5, 15, 0, 2) = 0xf
s3_5_c15_c0_3 (3, 5, 15, 0, 3) = 0xf
s3_5_c15_c0_4 (3, 5, 15, 0, 4) = 0x0
s3_5_c15_c0_5 (3, 5, 15, 0, 5) = 0x0
s3_5_c15_c0_6 (3, 5, 15, 0, 6) = 0x21f
s3_5_c15_c1_0 (3, 5, 15, 1, 0) = 0x0
s3_5_c15_c1_1 (3, 5, 15, 1, 1) = 0x0
s3_5_c15_c1_2 (3, 5, 15, 1, 2) = 0x1b0000001b
s3_5_c15_c1_3 (3, 5, 15, 1, 3) = 0x3
s3_5_c15_c2_0 (3, 5, 15, 2, 0) = 0x0
s3_5_c15_c3_0 (3, 5, 15, 3, 0) = 0x0
s3_5_c15_c3_1 (3, 5, 15, 3, 1) = 0x1800
s3_5_c15_c3_2 (3, 5, 15, 3, 2) = 0x0
s3_5_c15_c3_4 (3, 5, 15, 3, 4) = 0x0
s3_5_c15_c3_5 (3, 5, 15, 3, 5) = 0x0
s3_5_c15_c4_0 (3, 5, 15, 4, 0) = 0xd
s3_5_c15_c4_1 (3, 5, 15, 4, 1) = 0x100003e485001f
s3_5_c15_c5_0 (3, 5, 15, 5, 0) = 0x2000000
s3_5_c15_c5_2 (3, 5, 15, 5, 2) = 0x0
s3_5_c15_c5_4 (3, 5, 15, 5, 4) = 0x0
s3_5_c15_c6_0 (3, 5, 15, 6, 0) = 0x180010102001c207
s3_5_c15_c7_0 (3, 5, 15, 7, 0) = 0x100
s3_5_c15_c8_0 (3, 5, 15, 8, 0) = 0x4
s3_5_c15_c8_1 (3, 5, 15, 8, 1) = 0xffffffff
s3_5_c15_c9_0 (3, 5, 15, 9, 0) = 0x20001d1500f20014
s3_5_c15_c10_0 (3, 5, 15, 10, 0) = 0x2005f200102
s3_5_c15_c10_1 (3, 5, 15, 10, 1) = 0x0
s3_5_c15_c13_4 (3, 5, 15, 13, 4) = 0x0
s3_5_c15_c13_5 (3, 5, 15, 13, 5) = 0x0
s3_5_c15_c14_2 (3, 5, 15, 14, 2) = 0x0
s3_5_c15_c14_3 (3, 5, 15, 14, 3) = 0x0
s3_5_c15_c14_4 (3, 5, 15, 14, 4) = 0x0
s3_5_c15_c14_5 (3, 5, 15, 14, 5) = 0x0
s3_5_c15_c14_6 (3, 5, 15, 14, 6) = 0x0
s3_5_c15_c14_7 (3, 5, 15, 14, 7) = 0x0
s3_6_c15_c1_0 (3, 6, 15, 1, 0) = 0x0
s3_6_c15_c1_2 (3, 6, 15, 1, 2) = 0x0
s3_6_c15_c1_4 (3, 6, 15, 1, 4) = 0x0
s3_6_c15_c2_0 (3, 6, 15, 2, 0) = 0x0
s3_6_c15_c2_1 (3, 6, 15, 2, 1) = 0x12fa1db611a4c14
s3_6_c15_c2_2 (3, 6, 15, 2, 2) = 0x7bea3a52c6e474ab
s3_6_c15_c2_3 (3, 6, 15, 2, 3) = 0x0
s3_6_c15_c2_4 (3, 6, 15, 2, 4) = 0x0
s3_6_c15_c2_5 (3, 6, 15, 2, 5) = 0x0
s3_6_c15_c2_7 (3, 6, 15, 2, 7) = 0x10003
s3_6_c15_c7_0 (3, 6, 15, 7, 0) = 0x3e094b905367a138
s3_6_c15_c7_1 (3, 6, 15, 7, 1) = 0x729c61cc911db3d0
s3_6_c15_c7_2 (3, 6, 15, 7, 2) = 0xdd3223b5c9807c14
s3_6_c15_c7_3 (3, 6, 15, 7, 3) = 0x191277470b2e1017
s3_6_c15_c7_4 (3, 6, 15, 7, 4) = 0xe5ac8d636d111ab8
s3_6_c15_c7_5 (3, 6, 15, 7, 5) = 0x4c0a977780a1bf2e
s3_6_c15_c7_6 (3, 6, 15, 7, 6) = 0xd186cdb61af898a6
s3_6_c15_c7_7 (3, 6, 15, 7, 7) = 0xfc9946bc0688369f
s3_6_c15_c8_0 (3, 6, 15, 8, 0) = 0x0
s3_6_c15_c8_3 (3, 6, 15, 8, 3) = 0x2
s3_6_c15_c8_6 (3, 6, 15, 8, 6) = 0x2
s3_6_c15_c12_2 (3, 6, 15, 12, 2) = 0xc
s3_6_c15_c12_3 (3, 6, 15, 12, 3) = 0x1
s3_6_c15_c12_4 (3, 6, 15, 12, 4) = 0x1
s3_6_c15_c12_5 (3, 6, 15, 12, 5) = 0x0
s3_6_c15_c12_6 (3, 6, 15, 12, 6) = 0x0
s3_6_c15_c12_7 (3, 6, 15, 12, 7) = 0x0
s3_6_c15_c13_0 (3, 6, 15, 13, 0) = 0x7e1eb75eca93408c
s3_6_c15_c13_1 (3, 6, 15, 13, 1) = 0x69a4334ee673171b
s3_6_c15_c13_2 (3, 6, 15, 13, 2) = 0x7b0537a4c9237fd6
s3_6_c15_c13_3 (3, 6, 15, 13, 3) = 0x356ec5ffdbda584e
s3_6_c15_c13_4 (3, 6, 15, 13, 4) = 0xc9dfbcc5b08d03b8
s3_6_c15_c13_5 (3, 6, 15, 13, 5) = 0x5ecf1a29c0973432
s3_6_c15_c13_6 (3, 6, 15, 13, 6) = 0x7684c29566e14dc9
s3_6_c15_c13_7 (3, 6, 15, 13, 7) = 0x4bb4f32b76f2e6a9
s3_6_c15_c14_0 (3, 6, 15, 14, 0) = 0x7fc148694e0bcc6d
s3_6_c15_c14_1 (3, 6, 15, 14, 1) = 0x2936a8c66238f8f4
s3_6_c15_c14_2 (3, 6, 15, 14, 2) = 0x0
s3_6_c15_c14_4 (3, 6, 15, 14, 4) = 0x0
s3_6_c15_c14_5 (3, 6, 15, 14, 5) = 0x0
s3_6_c15_c14_6 (3, 6, 15, 14, 6) = 0xc00
s3_6_c15_c14_7 (3, 6, 15, 14, 7) = 0x0
s3_6_c15_c15_0 (3, 6, 15, 15, 0) = 0xc
s3_6_c15_c15_1 (3, 6, 15, 15, 1) = 0x0
s3_6_c15_c15_4 (3, 6, 15, 15, 4) = 0x0
s3_7_c15_c0_0 (3, 7, 15, 0, 0) = 0x0
s3_7_c15_c0_1 (3, 7, 15, 0, 1) = 0x0
s3_7_c15_c0_2 (3, 7, 15, 0, 2) = 0x0
s3_7_c15_c0_3 (3, 7, 15, 0, 3) = 0x0
s3_7_c15_c0_4 (3, 7, 15, 0, 4) = 0x0
s3_7_c15_c0_5 (3, 7, 15, 0, 5) = 0x0
s3_7_c15_c1_0 (3, 7, 15, 1, 0) = 0x0
s3_7_c15_c1_1 (3, 7, 15, 1, 1) = 0x0
s3_7_c15_c1_2 (3, 7, 15, 1, 2) = 0x0
s3_7_c15_c1_3 (3, 7, 15, 1, 3) = 0x0
s3_7_c15_c1_4 (3, 7, 15, 1, 4) = 0x0
s3_7_c15_c1_5 (3, 7, 15, 1, 5) = 0x0
s3_7_c15_c2_0 (3, 7, 15, 2, 0) = 0x0
s3_7_c15_c2_1 (3, 7, 15, 2, 1) = 0x3db15f4dfc5d5724
s3_7_c15_c2_2 (3, 7, 15, 2, 2) = 0x0
s3_7_c15_c2_3 (3, 7, 15, 2, 3) = 0x0
s3_7_c15_c2_4 (3, 7, 15, 2, 4) = 0x0
s3_7_c15_c2_5 (3, 7, 15, 2, 5) = 0x0
s3_7_c15_c3_2 (3, 7, 15, 3, 2) = 0x0
s3_7_c15_c3_3 (3, 7, 15, 3, 3) = 0x0
s3_7_c15_c3_4 (3, 7, 15, 3, 4) = 0x0
s3_7_c15_c3_5 (3, 7, 15, 3, 5) = 0x0
s3_7_c15_c4_0 (3, 7, 15, 4, 0) = 0x0
s3_7_c15_c4_2 (3, 7, 15, 4, 2) = 0x0
s3_7_c15_c4_3 (3, 7, 15, 4, 3) = 0x0
s3_7_c15_c4_4 (3, 7, 15, 4, 4) = 0x0
s3_7_c15_c4_5 (3, 7, 15, 4, 5) = 0x0
s3_7_c15_c5_0 (3, 7, 15, 5, 0) = 0x0
s3_7_c15_c5_2 (3, 7, 15, 5, 2) = 0x0
s3_7_c15_c5_3 (3, 7, 15, 5, 3) = 0x0
s3_7_c15_c5_4 (3, 7, 15, 5, 4) = 0x0
s3_7_c15_c5_5 (3, 7, 15, 5, 5) = 0x0
s3_7_c15_c6_2 (3, 7, 15, 6, 2) = 0x0
s3_7_c15_c6_3 (3, 7, 15, 6, 3) = 0x0
s3_7_c15_c6_4 (3, 7, 15, 6, 4) = 0x0
s3_7_c15_c6_5 (3, 7, 15, 6, 5) = 0x0
s3_7_c15_c7_2 (3, 7, 15, 7, 2) = 0x0
s3_7_c15_c7_3 (3, 7, 15, 7, 3) = 0x0
s3_7_c15_c7_4 (3, 7, 15, 7, 4) = 0x0
s3_7_c15_c7_5 (3, 7, 15, 7, 5) = 0x0
s3_7_c15_c8_2 (3, 7, 15, 8, 2) = 0x0
s3_7_c15_c8_3 (3, 7, 15, 8, 3) = 0x0
s3_7_c15_c8_4 (3, 7, 15, 8, 4) = 0x0
s3_7_c15_c8_5 (3, 7, 15, 8, 5) = 0x0
s3_7_c15_c9_2 (3, 7, 15, 9, 2) = 0x0
s3_7_c15_c9_3 (3, 7, 15, 9, 3) = 0x0
s3_7_c15_c9_4 (3, 7, 15, 9, 4) = 0x0
s3_7_c15_c9_5 (3, 7, 15, 9, 5) = 0x0
s3_7_c15_c10_2 (3, 7, 15, 10, 2) = 0x0
s3_7_c15_c10_3 (3, 7, 15, 10, 3) = 0x0
s3_7_c15_c10_4 (3, 7, 15, 10, 4) = 0x0
s3_7_c15_c10_5 (3, 7, 15, 10, 5) = 0x0
s3_7_c15_c11_2 (3, 7, 15, 11, 2) = 0x0
s3_7_c15_c11_3 (3, 7, 15, 11, 3) = 0x0
s3_7_c15_c11_4 (3, 7, 15, 11, 4) = 0x0
s3_7_c15_c11_5 (3, 7, 15, 11, 5) = 0x0
s3_7_c15_c12_2 (3, 7, 15, 12, 2) = 0x0
s3_7_c15_c12_3 (3, 7, 15, 12, 3) = 0x0
s3_7_c15_c12_4 (3, 7, 15, 12, 4) = 0x0
s3_7_c15_c13_2 (3, 7, 15, 13, 2) = 0x0
s3_7_c15_c13_3 (3, 7, 15, 13, 3) = 0x0
s3_7_c15_c13_4 (3, 7, 15, 13, 4) = 0x0
s3_7_c15_c14_2 (3, 7, 15, 14, 2) = 0x0
s3_7_c15_c14_3 (3, 7, 15, 14, 3) = 0x0
s3_7_c15_c14_4 (3, 7, 15, 14, 4) = 0x0
s3_7_c15_c15_2 (3, 7, 15, 15, 2) = 0x0
s3_7_c15_c15_3 (3, 7, 15, 15, 3) = 0x0
```