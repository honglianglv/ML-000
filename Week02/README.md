本周学习了python效果调优，发现使用不通写法的python代码效率居然可以查几个数量级，第一次学习了cython和jax，收获很大，谢谢老师

# 代码说明:
1. 其中target_mean_v3 使用cython里面的c++，主要数据结构用了map，100万的数据平均耗时83.7 ms
2. 其中target_mean_v4 使用cython里面的c++，主要数据结构用了unordered_map，100万的数据平均耗时93.3 ms
3. 其中target_mean_v5 使用cython里面的c，主要数据结构用了静态数组，100万的数据平均耗时10.8 ms

