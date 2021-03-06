| Device | Interface > Dest    | IP & Mask                      |
| ------ | ------------------- | ------------------------------ |
| RNM    | G0/0/0 > Izq        | 172.31.230.1 255.255.255.252   |
|        | G0/0/1 > G0/1 S1    | 172.31.230.245 255.255.255.252 |
|        | S0/1/0 > S0/1/0 R10 | 172.31.230.5 255.255.255.252   |
|        |                     |                                |
| R10    | G0/0/0 > F0 DHCP    | 172.31.230.253 255.255.255.252 |
|        | S0/1/0 > S0/1/0 RNM | 172.31.230.6 255.255.255.252   |
|        | S0/1/1 > S0/1/0 R11 | 172.31.230.9 255.255.255.252   |
|        | S0/2/0 > S0/1/0 R12 | 172.31.230.13 255.255.255.252  |
|        |                     |                                |
| R11    | S0/1/0 > S0/1/1 R10 | 172.31.230.10 255.255.255.252  |
|        | G0/0/0 > F0/1 MS1   | 172.31.232.1 255.255.248.0     |
|        | G0/0/1 > F0/1 MS2   | 172.31.232.2 255.255.248.0     |
|        |                     |                                |
| R12    | S0/1/0 > S0/2/0 R10 | 172.31.230.14 255.255.255.252  |
|        | G0/0/0 > F0/2 MS1   | 172.31.232.3 255.255.248.0     |
|        | G0/0/1 > F0/2 MS2   | 172.31.232.4 255.255.248.0     |
|        |                     |                                |
| S1     | G0/1 > G0/0/1 RNM   |                                |
|        | F0/1 > F0 PC4       |                                |
|        |                     |                                |
| S2     | F0/1 > F0/1 MS3     |                                |
|        | F0/2 > F0/1 MS4     |                                |
|        | F0/3 > F0 PC1       |                                |
|        |                     |                                |
| S3     | F0/1 > F0/2 MS3     |                                |
|        | F0/2 > F0/2 MS4     |                                |
|        | F0/3 > F0 PC2       |                                |
|        |                     |                                |
| S4     | F0/1 > F0/3 MS3     |                                |
|        | F0/2 > F0/3 MS4     |                                |
|        | F0/3 > F0 PC3       |                                |
|        |                     |                                |
| MS1    | G0/1 > G0/1 MS3     |                                |
|        | G0/2 > G0/1 MS4     |                                |
|        | F0/1 > G0/0/0 R11   |                                |
|        | F0/2 > G0/0/0 R12   |                                |
|        | F0/3 > F0/3 MS2     |                                |
|        | F0/4 > F0/4 MS2     |                                |
|        |                     |                                |
| MS2    | G0/1 > G0/2 MS3     |                                |
|        | G0/2 > G0/2 MS4     |                                |
|        | F0/1 > G0/0/1 R11   |                                |
|        | F0/2 > G0/0/1 R12   |                                |
|        | F0/3 > F0/3 MS1     |                                |
|        | F0/4 > F0/4 MS1     |                                |
|        |                     |                                |
| MS3    | G0/1 > G0/1 MS1     |                                |
|        | G0/2 > G0/1 MS2     |                                |
|        | F0/1 > F0/1 S2      |                                |
|        | F0/2 > F0/1 S3      |                                |
|        | F0/3 > F0/1 S4      |                                |
|        |                     |                                |
| MS4    | G0/1 > G0/2 MS1     |                                |
|        | G0/2 > G0/2 MS2     |                                |
|        | F0/1 > F0/2 S2      |                                |
|        | F0/2 > F0/2 S3      |                                |
|        | F0/3 > F0/2 S4      |                                |
|        |                     |                                |
| DHCP   | F0 > G0/0/0 R10     | 172.31.230.254 255.255.255.252 |
| PC1    | F0 > F0/3 S2        | DHCP                           |
| PC2    | F0 > F0/3 S3        | DHCP                           |
| PC3    | F0 > F0/3 S4        | DHCP                           |
| PC4    | F0 > F0/1 S1        | 172.31.230.246 255.255.255.252 |
|        |                     |                                |
|---------------------------------------------------------------|
|        |                     |                                |
| RNM2   | G0/0 > Der          | 172.31.230.2 255.255.255.252   |
|        | G0/1 > G0/1 SS      | 172.31.231.1 255.255.255.0     |
|        | S0/1/0 > S0/1/0 RInt| 172.31.230.17 255.255.255.252  |
|        | S0/1/1 > S0/1/0 R20 | 172.31.230.21 255.255.255.252  |
|        |                     |                                |
| R20    | G0/0 > F0 DHCP2     | 172.31.230.249 255.255.255.252 |
|        | S0/1/0 > S0/1/1 RNM2| 172.31.230.22 255.255.255.252  |
|        | S0/1/1 > S0/1/0 R21 | 172.31.230.25 255.255.255.252  |
|        | S0/0/0 > S0/1/0 R22 | 172.31.230.29 255.255.255.252  |
|        |                     |                                |
| R21    | S0/1/0 > S0/1/1 R20 | 172.31.230.26 255.255.255.252  |
|        | G0/0 > G0/1 MS21    | 172.31.240.1 255.255.240.0     |
|        | G0/1 > G0/1 MS22    | 172.31.240.2 255.255.240.0     |
|        |                     |                                |
| R22    | S0/1/0 > S0/0/0 R20 | 172.31.230.30 255.255.255.252  |
|        | G0/0 > G0/2 MS21    | 172.31.240.3 255.255.240.0     |
|        | G0/1 > G0/2 MS22    | 172.31.240.4 255.255.240.0     |
|        |                     |                                |
| MS21   | G0/1 > G0/0 R21     |                                |
|        | G0/2 > G0/0 R22     |                                |
|        | F0/1 > F0/1 S21     |                                |
|        | F0/2 > F0/1 S22     |                                |
|        | F0/3 > F0/1 S23     |                                |
|        |                     |                                |
| MS22   | G0/1 > G0/1 R21     |                                |
|        | G0/2 > G0/1 R22     |                                |
|        | F0/1 > F0/2 S21     |                                |
|        | F0/2 > F0/2 S22     |                                |
|        | F0/3 > F0/2 S23     |                                |
|        |                     |                                |
| S21    | F0/1 > F0/1 MS21    |                                |
|        | F0/2 > F0/1 MS22    |                                |
|        | F0/3 > F0 PC21      |                                |
|        |                     |                                |
| S22    | F0/1 > F0/2 MS21    |                                |
|        | F0/2 > F0/2 MS22    |                                |
|        | F0/3 > F0 PC22      |                                |
|        |                     |                                |
| S23    | F0/1 > F0/3 MS21    |                                |
|        | F0/2 > F0/3 MS22    |                                |
|        | F0/3 > F0 PC23      |                                |
|        |                     |                                |
| DHCP2  | F0 > G0/0 R20       | 172.31.230.250 255.255.255.252 |
| PC21   | F0 > F0/3 S21       | DHCP                           |
| PC22   | F0 > F0/3 S22       | DHCP                           |
| PC33   | F0 > F0/3 S23       | DHCP                           |
|        |                     |                                |
| RInt   | S0/1/0 > S0/1/0 RNM2| 172.31.230.18 255.255.255.252  |
|        | G0/0 > G0/1 SInt    | ----                           |
| SInt   | G0/1 > G0/0 RInt    |                                |
|        | F0/1 > F0 PCInt     |                                |
| PCInt  | F0 > F0/1 SInt      | ----                           |
|        |                     |                                |
| SS     | G0/1 > G0/1 RNM2    |                                |
|        | F0/1 > F0 Srv1      |                                |
|        | F0/2 > F0 Srv2      |                                |
|        | F0/3 > F0 Srv3      |                                |
|        | F0/4 > F0 Srv4      |                                |
|        | F0/5 > F0 Srv5      |                                |
| Srv1   | F0 > F0/1 SS        | 172.31.231.254 255.255.255.0   |
| Srv2   | F0 > F0/2 SS        | 172.31.231.253 255.255.255.0   |
| Srv3   | F0 > F0/3 SS        | 172.31.231.252 255.255.255.0   |
| Srv4   | F0 > F0/4 SS        | 172.31.231.251 255.255.255.0   |
| Srv5   | F0 > F0/5 SS        | 172.31.231.250 255.255.255.0   |
|        |                     |                                |