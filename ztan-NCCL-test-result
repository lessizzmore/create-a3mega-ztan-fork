## NCCL TEST RESULT

> mpirun -v --mca btl self,tcp --mca btl_tcp_if_include enp0s12 --hostfile ~/hostfile \
>    -np 16 \
>    -npernode 8 \
>    -x ${HOST_VARS} \
>    /opt/src/nccl-tests/build/all_reduce_perf -b 8 -e 8G -f 2 -g 1

# nThread 1 nGpus 1 minBytes 8 maxBytes 8589934592 step: 2(factor) warmup iters: 5 iters: 20 agg iters: 1 validation: 1 graph: 0
#
# Using devices
#  Rank  0 Group  0 Pid   6899 on ztan-mig-235z device  0 [0000:04:00] NVIDIA H100 80GB HBM3
#  Rank  1 Group  0 Pid   6900 on ztan-mig-235z device  1 [0000:05:00] NVIDIA H100 80GB HBM3
#  Rank  2 Group  0 Pid   6901 on ztan-mig-235z device  2 [0000:0b:00] NVIDIA H100 80GB HBM3
#  Rank  3 Group  0 Pid   6902 on ztan-mig-235z device  3 [0000:0c:00] NVIDIA H100 80GB HBM3
#  Rank  4 Group  0 Pid   6903 on ztan-mig-235z device  4 [0000:84:00] NVIDIA H100 80GB HBM3
#  Rank  5 Group  0 Pid   6904 on ztan-mig-235z device  5 [0000:85:00] NVIDIA H100 80GB HBM3
#  Rank  6 Group  0 Pid   6905 on ztan-mig-235z device  6 [0000:8b:00] NVIDIA H100 80GB HBM3
#  Rank  7 Group  0 Pid   6906 on ztan-mig-235z device  7 [0000:8c:00] NVIDIA H100 80GB HBM3
#  Rank  8 Group  0 Pid   6733 on ztan-mig-gq73 device  0 [0000:04:00] NVIDIA H100 80GB HBM3
#  Rank  9 Group  0 Pid   6734 on ztan-mig-gq73 device  1 [0000:05:00] NVIDIA H100 80GB HBM3
#  Rank 10 Group  0 Pid   6735 on ztan-mig-gq73 device  2 [0000:0b:00] NVIDIA H100 80GB HBM3
#  Rank 11 Group  0 Pid   6736 on ztan-mig-gq73 device  3 [0000:0c:00] NVIDIA H100 80GB HBM3
#  Rank 12 Group  0 Pid   6737 on ztan-mig-gq73 device  4 [0000:84:00] NVIDIA H100 80GB HBM3
#  Rank 13 Group  0 Pid   6738 on ztan-mig-gq73 device  5 [0000:85:00] NVIDIA H100 80GB HBM3
#  Rank 14 Group  0 Pid   6739 on ztan-mig-gq73 device  6 [0000:8b:00] NVIDIA H100 80GB HBM3
#  Rank 15 Group  0 Pid   6740 on ztan-mig-gq73 device  7 [0000:8c:00] NVIDIA H100 80GB HBM3
#
#                                                              out-of-place                       in-place          
#       size         count      type   redop    root     time   algbw   busbw #wrong     time   algbw   busbw #wrong
#        (B)    (elements)                               (us)  (GB/s)  (GB/s)            (us)  (GB/s)  (GB/s)       
           8             2     float     sum      -1    135.8    0.00    0.00      0    123.5    0.00    0.00      0
          16             4     float     sum      -1    123.2    0.00    0.00      0    122.3    0.00    0.00      0
          32             8     float     sum      -1    123.3    0.00    0.00      0    122.7    0.00    0.00      0
          64            16     float     sum      -1    123.4    0.00    0.00      0    122.9    0.00    0.00      0
         128            32     float     sum      -1    123.0    0.00    0.00      0    122.7    0.00    0.00      0
         256            64     float     sum      -1    123.6    0.00    0.00      0    122.7    0.00    0.00      0
         512           128     float     sum      -1    126.6    0.00    0.01      0    123.4    0.00    0.01      0
        1024           256     float     sum      -1    147.1    0.01    0.01      0    123.1    0.01    0.02      0
        2048           512     float     sum      -1    125.8    0.02    0.03      0    124.6    0.02    0.03      0
        4096          1024     float     sum      -1    126.9    0.03    0.06      0    125.6    0.03    0.06      0
        8192          2048     float     sum      -1    131.6    0.06    0.12      0    130.6    0.06    0.12      0
       16384          4096     float     sum      -1    138.6    0.12    0.22      0    137.6    0.12    0.22      0
       32768          8192     float     sum      -1    155.2    0.21    0.40      0    153.1    0.21    0.40      0
       65536         16384     float     sum      -1    159.4    0.41    0.77      0    157.6    0.42    0.78      0
      131072         32768     float     sum      -1    159.3    0.82    1.54      0    169.0    0.78    1.45      0
      262144         65536     float     sum      -1    167.1    1.57    2.94      0    163.9    1.60    3.00      0
      524288        131072     float     sum      -1    174.2    3.01    5.64      0    171.0    3.07    5.75      0
     1048576        262144     float     sum      -1    203.2    5.16    9.68      0    207.2    5.06    9.49      0
     2097152        524288     float     sum      -1    254.0    8.26   15.48      0    252.9    8.29   15.55      0
     4194304       1048576     float     sum      -1    364.6   11.50   21.57      0    356.6   11.76   22.05      0
     8388608       2097152     float     sum      -1    571.9   14.67   27.50      0    563.5   14.89   27.91      0
    16777216       4194304     float     sum      -1    977.6   17.16   32.18      0    951.6   17.63   33.06      0
    33554432       8388608     float     sum      -1   1059.9   31.66   59.36      0   1054.0   31.84   59.69      0
    67108864      16777216     float     sum      -1   1261.6   53.20   99.74      0   1270.2   52.83   99.06      0
   134217728      33554432     float     sum      -1   1652.2   81.24  152.32      0   1636.7   82.01  153.76      0
   268435456      67108864     float     sum      -1   2360.9  113.70  213.19      0   2359.9  113.75  213.28      0
   536870912     134217728     float     sum      -1   3817.5  140.63  263.69      0   3828.0  140.25  262.97      0
  1073741824     268435456     float     sum      -1   6759.0  158.86  297.86      0   6737.4  159.37  298.82      0
  2147483648     536870912     float     sum      -1    12646  169.81  318.40      0    12641  169.88  318.52      0
  4294967296    1073741824     float     sum      -1    24361  176.31  330.58      0    24365  176.27  330.51      0
  8589934592    2147483648     float     sum      -1    47535  180.71  338.82      0    47743  179.92  337.35      0
# Out of bounds values : 0 OK
# Avg bus bandwidth    : 70.742 
