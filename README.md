linbpq / FBB PG server for display of Keps from exported mail.

Export the keps file to a text file using mail forwarding, e.g. FILE /home/user/linbpq-node/keps.txt

Compile and move to the PG directory (note case on Linux)

Create/add the configuration for this to the <basedir>/PG/PGList.txt file

```
### BPQ PG Server configuration file
#
#
# Format:
#
# Each PG Server on a seperate line
#
# PG_NAME,PG_EXE,PG_DESCRIPTION
KEPS,kepsrv,Kepler display
```


Run the server at the BBS prompt:


```
[BPQ-6.0.25.26-B12FWIHJM$]
Hello Steve. Latest Message is 4517, Last listed is 264
de GB7BWR>
pg
KEPS   ->   Kepler display
de GB7BWR>
pg keps
Satellite tracker
-----------------

 1: AO-07
 2: UO-11
 3: AO-27
 4: FO-29
 5: GO-32
 6: ISS
 7: NO-44
 8: SO-50
 9: CO-55
10: RS-22
11: CO-65
12: CO-66
13: RS-30
14: SRMSAT
15: ZACUBE-1
16: Delfi-N3xt
17: GOMX-1
18: LO-74
19: AO-73
20: DTUSAT-2
21: LILACSAT-2
22: Horyu-4
23: Lapan A3
24: CAS-2T
25: TechnoSat
26: AO-91
27: S-Net D
28: S-Net B
29: S-Net A
30: S-Net C
31: Ten-Koh
32: PO-101
33: QO-100
34: MinXSS-2
35: AO-95
36: SNUSat 2
37: SnugLite
38: ITASat 1
39: EAGLET 1
40: ESEO
41: JO-97
42: Suomi 100
43: ISAT
44: UWE-4
45: Sparrow
46: Prox-1
47: Taurus 1
48: TO-108
49: RS-44
50: SALSAT
51: CSS (TIANHE-1)
52: CUTE
53: TeikyoSat 4
54: Z-Sat
55: KOSEN 1
56: HO-113
57: SNUGLITE 2
58: UmKA 1 (RS40S)
59: CubeBel-2 (EU11S)
60: RS-38S
61: SONATE-2
62: GRBBeta
63: Curium One
64: ROBUSTA-3A
65: CatSat
66: HYPERVIEW-1G (RS66S)
67: AO-123
68: JINJUSat 1B
69: NUSHSAT 1
70: TEVEL2-4
71: TEVEL2-5
72: TEVEL2-6
73: TEVEL2-1
74: TEVEL2-3
75: TEVEL2-2
76: TEVEL2-9
77: TEVEL2-7
78: TEVEL2-8
79: HYDRA-W
80: HADES-ICM (SO-125)
81: SPIRONE
82: K-HERO
83: SNUGLITE-III DURI
84: SilverSat
85: SAKHACUBE-CHOLBON
86: RS95S (QMR-KWT-2)
87: Ten-Koh2
88: JACK-002
89: DISCO 2
90: HADES-SA (SpinnyONE)
91: PARUS-6U1
92: SAL-E
93: FSI-SAT 2
94: OrigamiSat 2
95: ARICA 2
96: WASEDA-SAT-ZERO-II
97: MANGARO-II-Piscus
98: IO-86
99: LILIUM-4                
100: LILIUM-4

Enter sat number or name (0=Exit):
33

QO-100 GOOD
AZ 256 (W)
EL 2 deg
RNG 41423 km

Aim antenna: W low.

                N
                                 
                                 
                                 
W ---*----------+-------------- E
                                 
                                 
                                 
                S

1.00 orbits/day

Enter sat number or name (0=Exit):
0
Bye!
de GB7BWR>
```




The keps.txt file can have the headers left in but needs to be in the following format

```
AO-07
1 07530U 74089B   26131.02828537 -.00000034  00000-0  74901-4 0  9994
2 07530 101.9918 143.8856 0012125 200.3561 181.7211 12.53697443355861
UO-11
1 14781U 84021B   26131.16982026  .00000814  00000-0  88631-4 0  9996
2 14781  97.8036  97.1668 0006433 315.7966  44.2738 14.90694568251611
AO-27
1 22825U 93061C   26131.14983863  .00000053  00000-0  37296-4 0  9992
2 22825  98.6892 198.5733 0007951 201.7057 158.3790 14.30931926701709
```

