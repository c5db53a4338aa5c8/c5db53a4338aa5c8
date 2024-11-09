## 5.15.0

VM running on
Intel(R) Xeon(R) Silver 4214R

```
---------------------------------------------------------------------------------------------------------
| Container instance      |      W/o struct-agnostic      |      W struct-agnostic        |  Reduction  |
|                         |     1 to 0    |    3 to 0     |     1 to 0    |    3 to 0     |             |
|                         |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |             |
---------------------------------------------------------------------------------------------------------
| posix timers hash table |   3.9 |  15.1 |   0.0 |  13.9 |   3.4 |  16.6 |   0.0 |   9.4 |  100 |   38 |
| futex hash table        |   0.0 |  34.1 |  14.8 |  32.4 |   0.2 |  24.0 |   0.1 |  23.9 |  100 |   30 |
```

IPC stuff errored out.

## 6.11.6

Laptop with
AMD Ryzen 7 PRO 4750U

```
---------------------------------------------------------------------------------------------------------
| Container instance      |      W/o struct-agnostic      |      W struct-agnostic        |  Reduction  |
|                         |     1 to 0    |    3 to 0     |     1 to 0    |    3 to 0     |             |
|                         |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |             |
---------------------------------------------------------------------------------------------------------
| posix timers hash table |   0.0 |   0.0 |   0.0 |   0.0 |   0.8 |   0.0 |   0.3 |   0.0 |  100 |  100 |
| futex hash table        |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |  100 |  100 |
| ipc hash table          |  41.5 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |  100 |  100 |
| ipc radix tree          |   0.0 |   0.2 |       |       |   0.0 |   0.0 |       |       |  100 |  100 |
---------------------------------------------------------------------------------------------------------
```
hrtimer stuff errored out.

## 6.2.0

Workstation with
AMD EPYC 75F3

```
---------------------------------------------------------------------------------------------------------
| Container instance      |      W/o struct-agnostic      |      W struct-agnostic        |  Reduction  |
|                         |     1 to 0    |    3 to 0     |     1 to 0    |    3 to 0     |             |
|                         |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |  FPR  |  FNR  |             |
---------------------------------------------------------------------------------------------------------
| posix timers hash table |   0.0 |   6.4 |   0.0 |   6.4 |   0.0 |   0.3 |   1.3 |   0.3 |  100 |   95 |
| futex hash table        |   0.0 |   0.0 |   0.0 |   0.0 |   0.0 |   0.1 |   0.0 |   0.1 |  100 | -194 |
| ipc hash table          |   0.4 |   0.0 |   0.0 |   0.0 |   0.0 |   3.5 |   0.0 |   0.0 |  100 |  100 |
| ipc radix tree          |   0.0 |   0.0 |       |       |   0.0 |   0.0 |       |       |  100 |  100 |
---------------------------------------------------------------------------------------------------------
```

