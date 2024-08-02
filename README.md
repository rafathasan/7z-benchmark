# 7z Benchmark Comparison: Colab vs Kaggle vs i9-9900K

## Colab Results

**Processor Name:** Intel(R) Xeon(R) CPU @ 2.20GHz (406F0)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 2992                    | 128                    | 2273                 | 2911                    | 38202                    | 171                      | 1909                   | 3262                      |
| 23   | 4135                    | 178                    | 2372                 | 4214                    | 35911                    | 164                      | 1892                   | 3109                      |
| 24   | 3693                    | 167                    | 2380                 | 3971                    | 37896                    | 175                      | 1903                   | 3327                      |
| 25   | 2865                    | 144                    | 2271                 | 3272                    | 32120                    | 152                      | 1885                   | 2859                      |
| Avr  |                         | 154                    | 2324                 | 3592                    |                          | 165                      | 1897                   | 3139                      |
| Tot  |                         | 160                    | 2111                 | 3365                    |                          |                          |                        |                           |

## Kaggle Results

**Processor Name:** AMD EPYC 7B12 (830F10)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 9824                    | 331                    | 2888                 | 9557                    | 125236                   | 362                      | 2952                   | 10685                     |
| 23   | 11088                   | 374                    | 3019                 | 11297                   | 134001                   | 392                      | 2958                   | 11594                     |
| 24   | 11060                   | 374                    | 3184                 | 11892                   | 130798                   | 390                      | 2943                   | 11482                     |
| 25   | 10859                   | 380                    | 3266                 | 12399                   | 119010                   | 365                      | 2900                   | 10592                     |
| Avr  |                         | 365                    | 3089                 | 11286                   |                          | 377                      | 2938                   | 11088                     |
| Tot  |                         | 371                    | 3014                 | 11187                   |                          |                          |                        |                           |

## i9-9900K Results

**Processor Name:** Intel(R) Core(TM) i9-9900K CPU @ 3.60GHz (906ED)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 52649                   | 1385                   | 3698                 | 51217                   | 637986                   | 1577                     | 3450                   | 54414                     |
| 23   | 50906                   | 1452                   | 3572                 | 51867                   | 635144                   | 1590                     | 3457                   | 54953                     |
| 24   | 48628                   | 1470                   | 3556                 | 52285                   | 625044                   | 1587                     | 3458                   | 54863                     |
| 25   | 45579                   | 1483                   | 3508                 | 52040                   | 615586                   | 1589                     | 3447                   | 54785                     |
| Avr  |                         |1448                    | 3583                 | 51852                   |                          | 1586                     | 3453                   | 54754                     |
| Tot  |                         |1517                    | 3518                 | 53303                   |                          |                          |                        |                           |


## Azure Standard B1s (1 vcpu, 1 GiB memory)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 3766                    | 100                    | 3679                 | 3664                    | 30351                    | 100                      | 2595                   | 2591                      |
| 23   | 3458                    | 96                     | 3657                 | 3524                    | 30255                    | 100                      | 2627                   | 2619                      |
| 24   | 3246                    | 99                     | 3523                 | 3490                    | 29599                    | 100                      | 2604                   | 2599                      |
| 25   | 2968                    | 99                     | 3427                 | 3389                    | 29229                    | 99                       | 2619                   | 2602                      |
| Avr  | 3359                    | 98                     | 3571                 | 3517                    | 29859                    | 100                      | 2611                   | 2603                      |
| Tot  |                         | 99                     | 3091                 | 3060                    |                          |                          |                        |                           |



## Compression Comparison (Average Values)

| Processor        | Average Compress Speed (KiB/s) | Average Compression R/U MIPS | Average Compression Rating MIPS | Average Decompress Speed (KiB/s) | Average Decompression R/U MIPS | Average Decompression Rating MIPS |
|------------------|-------------------------------|------------------------------|--------------------------------|----------------------------------|------------------------------|----------------------------------|
| Colab            | 3421                          | 2324                         | 3592                           | 3592                             | 1897                         | 3139                             |
| Kaggle           | 8278                          | 3089                         | 11286                          | 11286                            | 2938                         | 11088                            |
| i9-9900K         | 49365                         | 3583                         | 51852                          | 51852                            | 3453                         | 54754                            |
| Azure Std B1s    | 3359                          | 3571                         | 3517                           | 29859                            | 2611                         | 2603                             |
Please note that the benchmark results may vary based on the specific configurations and resources available on each platform.
