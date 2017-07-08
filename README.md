# Caffe-ShuffleNet
This is Re-implementation of ShuffleNet, For details, please read the original paper:  
["ShuffleNet: An Extremely Efficient Convolutional
Neural Network for Mobile Devices" by Xiangyu Zhang et. al. 2017](https://arxiv.org/pdf/1707.01083.pdf). If you find any bug, please drop me an email. Thanks.

# Notes  
    | 水果        | 价格    |  数量  |
    | --------   | -----:   | :----: |
    | 香蕉        | $1      |   5    |
    | 苹果        | $1      |   6    |
    | 草莓        | $1      |   7    |  
    
    
    
    | group 1    | group 2    |  group 3  |
    | ：-：   | ：-：      | ：-： |  
    | 1    2     | 3     4    | 5   6     |  
    Every nubmer represents a channel of the feature map
## step 1: Reshape  
1  2  
3  4   
5  6 
## step 2: transpose  
1 3 5  
2 4 6　　
## step 3: flatten  
    | group 1    | group 2    |  group 3  |
    | --------   | -----      | --------- |
    | 1    3    | 5     2   | 4   6    |

# Acknowledge  
[HolmesShuan](https://github.com/HolmesShuan)
