# Car Evaluation Data Set Analysis

From the experiments we've conducted, several trends can be concluded:

-   For neural network with four layers, normally more than 3000 iterations are
    needed for the neural network to converges. For example, 4 layers NN with
    `(6 8 8 6)` and `(10 10 10 10)` neurons both took roughly 3400 iterations
    to converge (both yield a good test error).

-   Given the size of the data set size (around 1500 instance), it is
    relatively easy for neural network to train. Even if the network did not
    converge, sometimes it could have a relatively good test error.

### Best Parameters

The best parameters so far were:

    python3 NNDriver.py ../data/car.csv 50000 4 6 8 8 6

        Training data set size: 1381
        Testing data set size: 346

        Total training iteration executed: 3403
        Total training error = 0.9413%

        Neural Network model parameter are as follow:
        Layer 0
            Neuron 1 weight: [-7.4495, 3.4099, -0.0256, 0.2039, -11.7304, 0.0667, -0.4135]
            Neuron 2 weight: [-1.3459, 0.5654, -0.3278, 7.4246, 5.4987, -16.548, 1.7411]
            Neuron 3 weight: [-9.5774, 5.6102, -0.9633, 0.0509, -0.083, 0.2789, -13.2914]
            Neuron 4 weight: [-10.0866, 5.8388, -0.5114, -0.0802, 0.2002, -0.1474, 13.3149]
            Neuron 5 weight: [4.4728, -2.0952, -4.0434, 0.223, -0.0699, 0.0131, -0.2912]
            Neuron 6 weight: [-8.0664, 3.86, -6.0655, 0.0349, 0.0627, 0.0569, 0.2338]
        Layer 1
            Neuron 1 weight: [1.7962, 1.7513, 6.6557, -5.7184, 5.0891, -2.959, 2.2231]
            Neuron 2 weight: [-7.4357, -4.4296, 0.8774, 3.7, 2.5725, 4.9805, -5.8043]
            Neuron 3 weight: [-9.061, -4.9209, 2.446, 3.618, 4.5569, 4.3102, -5.1533]
            Neuron 4 weight: [-9.7535, -4.7397, 3.9116, 3.6247, 6.0801, 4.1791, -3.4284]
            Neuron 5 weight: [-5.2063, -2.9887, 1.6484, 2.5329, 2.2577, 2.5409, -2.7006]
            Neuron 6 weight: [-6.6986, -7.1949, 1.069, 6.6203, 5.9993, 6.531, -6.6227]
            Neuron 7 weight: [-6.0742, -3.7759, 1.7956, 3.5573, 2.629, 3.2502, -3.4913]
            Neuron 8 weight: [-4.3256, -2.4988, 1.3507, 2.062, 1.742, 2.0837, -2.2966]
        Layer 2
            Neuron 1 weight: [-3.3491, -3.6796, 2.6636, 3.2787, 3.4829, 1.8846, 4.1216, 2.4721, 1.5827]
            Neuron 2 weight: [-3.3227, -3.5545, 2.6488, 3.2695, 3.3986, 1.8747, 4.0237, 2.3734, 1.4893]
            Neuron 3 weight: [-4.764, -4.4599, 2.4518, 2.6224, 1.9118, 0.9881, 1.3486, 1.4814, 0.7694]
            Neuron 4 weight: [-3.2001, -3.0947, 2.3741, 2.9143, 3.1777, 1.6244, 3.5795, 2.168, 1.3157]
            Neuron 5 weight: [-3.1751, -2.9637, 2.3248, 2.8683, 3.0966, 1.6154, 3.438, 2.0496, 1.2622]
            Neuron 6 weight: [-5.4284, -4.5512, 2.6133, 3.0276, 2.5268, 1.2128, 0.9454, 1.6692, 0.9295]
            Neuron 7 weight: [-4.9765, -4.5137, 2.4607, 2.6537, 2.0182, 1.0187, 1.4628, 1.4863, 0.8098]
            Neuron 8 weight: [-4.86, -3.8599, 2.2375, 2.6718, 2.3304, 1.0421, 0.591, 1.4316, 0.8102]
        Layer 3
            Neuron 1 weight: [3.7841, -3.3815, -3.2848, -2.3381, -3.0111, -2.9757, -2.2433, -2.4828, -1.8178]
            Neuron 2 weight: [3.6239, -3.2994, -3.2137, -2.3033, -2.9531, -2.876, -2.2769, -2.4537, -1.7329]
            Neuron 3 weight: [3.7905, -3.3791, -3.3283, -2.3115, -3.022, -2.9329, -2.3073, -2.4963, -1.7359]
            Neuron 4 weight: [3.224, -0.4285, -0.4868, -1.7978, -0.3126, -0.3557, -1.8481, -1.9114, -1.5181]
            Neuron 5 weight: [3.2512, -3.1242, -3.0055, -2.1638, -2.8028, -2.7125, -2.0741, -2.3858, -1.6408]
            Neuron 6 weight: [6.8334, 0.5777, 0.6429, -3.2487, 0.1145, 0.0146, -3.736, -3.2231, -3.3532]
        Layer 4
            Neuron 1 weight: [-5.2664, -3.719, -3.52, -3.7409, 0.0646, -3.0466, 8.2785]
            Neuron 2 weight: [-0.2783, -2.1669, -2.1709, -2.1854, -3.6548, -2.0863, -0.181]
            Neuron 3 weight: [-2.742, 3.0925, 3.0516, 3.093, 0.2801, 2.9071, -0.543]
            Neuron 4 weight: [2.1963, -2.0925, -1.9776, -2.0184, -2.1596, -1.9149, -15.5732]

        Total test error = 1.4451%


        --- Execution time: 2760.1818130016327 seconds ---

### Appendix: List of Results

    raw
    ├── car_it1000_layer3_10_10_10.txt
    ├── car_it1000_layer3_3_2_3.txt
    ├── car_it1000_layer3_4_4_4.txt
    ├── car_it1000_layer4_4_6_6_4.txt
    ├── car_it2000_layer3_10_10_10.txt
    ├── car_it2000_layer3_3_2_3.txt
    ├── car_it2000_layer3_4_4_4.txt
    ├── car_it2000_layer4_4_6_6_4.txt
    ├── car_it200_layer3_10_10_10.txt
    ├── car_it200_layer3_3_2_3.txt
    ├── car_it200_layer3_4_4_4.txt
    ├── car_it200_layer4_4_6_6_4.txt
    ├── car_it50000_layer3_10_10_10.txt
    ├── car_it50000_layer4_10_10_10_10.txt
    └── car_it50000_layer4_6_8_8_6.txt

    0 directories, 15 files
