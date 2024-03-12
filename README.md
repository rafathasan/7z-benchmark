# 7z Benchmark Comparison: Colab vs Kaggle vs i9-9900K

## Colab Results

**Processor Name:** Intel(R) Xeon(R) CPU @ 2.20GHz (406F0)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 2992                    | 128                    | 2273                 | 2911                    | 38202                    | 171                      | 1909                   | 3262                      |
| 23   | 4135                    | 178                    | 2372                 | 4214                    | 35911                    | 164                      | 1892                   | 3109                      |
| 24   | 3693                    | 167                    | 2380                 | 3971                    | 37896                    | 175                      | 1903                   | 3327                      |
| 25   | 2865                    | 144                    | 2271                 | 3272                    | 32120                    | 152                      | 1885                   | 2859                      |
| Avr  | 154                     | 2324                   | 3592                 |                         | 165                      | 1897                     | 3139                 |                           |
| Tot  | 160                     | 2111                   | 3365                 |                         |                          |                          |                        |                           |


## Kaggle Results

**Processor Name:** AMD EPYC 7B12 (830F10)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 9824                    | 331                    | 2888                 | 9557                    | 125236                   | 362                      | 2952                   | 10685                     |
| 23   | 11088                   | 374                    | 3019                 | 11297                   | 134001                   | 392                      | 2958                   | 11594                     |
| 24   | 11060                   | 374                    | 3184                 | 11892                   | 130798                   | 390                      | 2943                   | 11482                     |
| 25   | 10859                   | 380                    | 3266                 | 12399                   | 119010                   | 365                      | 2900                   | 10592                     |
| Avr  | 365                     | 3089                   | 11286                |                         | 377                      | 2938                     | 11088                |                           |
| Tot  | 371                     | 3014                   | 11187                |                         |                          |                          |                        |                           |


## i9-9900K Results

**Processor Name:** Intel(R) Core(TM) i9-9900K CPU @ 3.60GHz (906ED)

| Dict | Compress Speed (KiB/s) | Compression Usage (%) | Compression R/U MIPS | Compression Rating MIPS | Decompress Speed (KiB/s) | Decompression Usage (%) | Decompression R/U MIPS | Decompression Rating MIPS |
|------|-------------------------|------------------------|----------------------|-------------------------|--------------------------|--------------------------|------------------------|---------------------------|
| 22   | 52649                   | 1385                   | 3698                 | 51217                   | 637986                   | 1577                     | 3450                   | 54414                     |
| 23   | 50906                   | 1452                   | 3572                 | 51867                   | 635144                   | 1590                     | 3457                   | 54953                     |
| 24   | 48628                   | 1470                   | 3556                 | 52285                   | 625044                   | 1587                     | 3458                   | 54863                     |
| 25   | 45579                   | 1483                   | 3508                 | 52040                   | 615586                   | 1589                     | 3447                   | 54785                     |
| Avr  | 1448                    | 3583                   | 51852                |                         | 1586                     | 3453                     | 54754                |                           |
| Tot  | 1517                    | 3518                   | 53303                |                         |                          |                          |                        |                           |


## Comparison

| Processor (Freq)   | Average Compression Speed (KiB/s) | Average Compression Usage (%) | Average Compression Rating MIPS | Average Decompression Speed (KiB/s) | Average Decompression Usage (%) | Average Decompression Rating MIPS |
|---------------------|------------------------------------|-------------------------------|----------------------------------|--------------------------------------|----------------------------------|---------------------------------|
| Colab               | Intel Xeon @ 2.20GHz               | 154                           | 2324                          | 3592                             | 165                              | 1897                            | 3139                           |
| Kaggle              | AMD EPYC 7B12 @ 2.20GHz             | 365                           | 3089                          | 11286                            | 377                              | 2938                            | 11088                          |
| i9-9900K            | Intel i9-9900K @ 3.60GHz            | 1448                          | 3583                          | 51852                            | 1586                             | 3453                            | 54754                          |

Please note that the benchmark results may vary based on the specific configurations and resources available on each platform.
