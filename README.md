# SgLang-vs-vLLM Comparison
## on RTX 4090

# Sglang

## Model : NousResearch/Hermes-3-Llama-3.2-3B

Prompt                        Tokens     Time (s)   Memory (MB) GPU Mem (MB) Tokens/s 

                               123        1.30       0.10       30.00        94.55  
                               121        1.03       0.02       0.00         117.60 
                               124        1.02       0.01       0.00         121.13
                               125        1.03       0.02       0.00         121.70
                               127        1.03       0.01       0.00         123.86 
                               127        1.03       0.01       0.00         123.63 
                               127        1.03       0.00       0.00         123.79
                               126        1.03       0.02       0.00         122.11
                               128        1.04       0.00       0.00         123.60
                               128        1.03       0.00       0.00         124.62
                               118        1.03       0.00       0.00         114.88
                               128        50.80      0.00       0.00         2.52
                               126        48.74      0.00       0.00         0.00
=== Overall Metrics ===
Total Tokens: 1628
Total Time: 13.76 seconds
Average Tokens/s: 118.34
CPU Usage: 0.00%
Memory Usage: 953.74 MB
GPU Utilization: 96.00%

## Model : Qwen/Qwen2.5-Coder-1.5B-Instruct

Prompt                        Tokens     Time (s)   Memory (MB) GPU Mem (MB) Tokens/s 

                               127        0.74       0.11       30.00        170.57
                               126        0.58       0.03       0.00         217.89
                               128        0.59       0.01       0.00         218.64
                               124        0.59       0.02       0.00         210.5
                               128        50.21      0.00       0.00         2.55
                               128        49.07      0.01       0.00         0.00
                               128        0.58       0.00       0.00         222.15
                               126        0.58       0.02       0.00         215.93
                               127        0.58       0.00       0.00         220.46
                               127        0.58       0.01       0.00         218.96
                               127        0.58       0.00       0.00         220.63
                               125        0.58       0.00       0.00         216.54
                               127        0.59       0.00       0.00         214.48
=== Overall Metrics ===
Total Tokens: 1648
Total Time: 7.83 seconds
Average Tokens/s: 210.48
CPU Usage: 10.00%
Memory Usage: 932.45 MB
GPU Utilization: 55.00%

# Vllm

## Model : NousResearch/Hermes-3-Llama-3.2-3B

Prompt                        Tokens     Time (s)   Memory (MB) GPU Mem (MB) Tokens/s 

                               12         0.39       0.20       4.00         30.97
                               15         0.20       0.04       0.00         76.53
                               15         0.20       0.03       0.00         74.40
                               15         0.20       0.03       0.00         74.51
                               11         0.20       0.03       0.00         55.33
                               13         0.20       0.08       0.00         64.12
                               15         0.21       0.03       0.00         72.34
                               15         0.37       0.08       0.00         40.45
                               12         0.21       0.03       0.00         56.44
                               14         0.21       0.03       0.00         66.36
                               15         0.21       0.03       0.00         72.12
                               16         0.21       0.02       0.00         76.43
                               15         0.21       0.03       0.00         72.52
=== Overall Metrics ===
Total Tokens: 183
Total Time: 3.02 seconds
Average Tokens/s: 60.69
CPU Usage: 0.00%
Memory Usage: 5701.59 MB
GPU Utilization: 31.00%


## Model : Qwen/Qwen2.5-Coder-1.5B-Instruct

Prompt                        Tokens     Time (s)   Memory (MB) GPU Mem (MB) Tokens/s 

                               13         0.23       0.21       4.00         55.5
                               15         0.13       0.04       0.00         112.34
                               14         0.13       0.04       0.00         110.14
                               14         0.13       0.03       0.00         105.37
                               14         0.12       0.03       0.00         113.78
                               14         0.13       0.06       0.00         106.96
                               15         0.13       0.03       0.00         116.17
                               9          0.13       0.02       0.00         69.8
                               14         0.14       0.03       0.00         99.51
                               15         0.14       0.03       0.00         108.44
                               15         0.13       0.03       0.00         113.77
                               12         0.13       0.02       0.00         90.96
                               14         0.13       0.03       0.00         109.19
=== Overall Metrics ===
Total Tokens: 178
Total Time: 1.81 seconds
Average Tokens/s: 98.27
CPU Usage: 0.00%
Memory Usage: 5759.47 MB
GPU Utilization: 50.00%
