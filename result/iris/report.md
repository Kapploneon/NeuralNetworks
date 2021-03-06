# Iris Data Set Analysis

From the experiments we've conducted, several trends can be concluded:

-   For this data set (only 4 inputs and 3 possible label), small number of
    layer with small neuron number would be enough.

-   Given the size of the data set (only less than 150 instance), total
    iteration needed for neural network to converges is at least 600 even for
    relatively small parameters.

    For example, the best parameters example below requires more than 600 or
    800 iterations to converge.

### Best Parameters

The best parameters so far were:

    python3 NNDriver.py ../data/iris.csv 80 2000 3 4 4 4

        Training data set size: 119
        Testing data set size: 30

        Total training iteration executed: 824 error: 0.8403%%
        Total training error = 0.8403%

        Neural Network model parameter are as follow:
        Layer 0
            Neuron 1 weight: [0.3031, 0.3858, 0.1276, -1.4067, -1.0732]
            Neuron 2 weight: [1.4633, 0.6315, -0.5463, -2.3652, -1.8725]
            Neuron 3 weight: [0.0383, -1.0469, 2.1748, -0.9284, -0.6321]
            Neuron 4 weight: [0.0419, -0.2579, 1.1303, -1.1602, -0.8866]
        Layer 1
            Neuron 1 weight: [-2.383, 2.0593, 2.5764, 1.9439, 1.7683]
            Neuron 2 weight: [-3.4129, 1.6341, 1.2904, 1.6836, 1.4868]
            Neuron 3 weight: [-2.7181, 1.7418, 1.878, 1.7543, 1.5622]
            Neuron 4 weight: [-3.3537, 1.6426, 1.333, 1.6521, 1.4992]
        Layer 2
            Neuron 1 weight: [1.7902, -2.4803, -2.3797, -2.2744, -2.3417]
            Neuron 2 weight: [2.1604, -2.9105, -2.7673, -2.7424, -2.7561]
            Neuron 3 weight: [2.3562, -3.1603, -2.9086, -2.8929, -2.9315]
            Neuron 4 weight: [6.5813, -1.4012, -3.1018, -2.1468, -3.0079]
        Layer 3
            Neuron 1 weight: [3.0781, -3.6302, -3.4684, -3.5259, -6.1667]
            Neuron 2 weight: [-2.972, -2.2477, -3.4394, -3.8915, 6.7657]
            Neuron 3 weight: [-6.2196, 3.4064, 3.6468, 3.8175, 1.9171]

        Total test error = 3.3333%


        --- Execution time: 18.540203094482422 seconds ---

    python3 NNDriver.py ../data/iris.csv 80 2000 3 10 10 10

        Training data set size: 119
        Testing data set size: 30

        Total training iteration executed: 623 error: 0.8403%%
        Total training error = 0.8403%

        Neural Network model parameter are as follow:
        Layer 0
            Neuron 1 weight: [0.0275, 0.0632, 0.5351, -1.015, -0.9125]
            Neuron 2 weight: [-1.4237, -0.931, 0.7389, 2.254, 1.8498]
            Neuron 3 weight: [-0.1818, -0.3748, 0.4067, 0.9062, 0.7535]
            Neuron 4 weight: [-0.1052, -0.1717, 0.9667, -0.9912, -0.9477]
            Neuron 5 weight: [-0.0945, -0.2457, 1.1377, -1.0433, -0.9414]
            Neuron 6 weight: [-0.1351, -0.2492, 1.112, -1.0068, -0.9411]
            Neuron 7 weight: [0.0665, -0.038, 0.5838, -0.9492, -0.8808]
            Neuron 8 weight: [-0.1583, -0.3645, 1.2606, -0.9832, -0.9076]
            Neuron 9 weight: [-0.0274, 0.0015, 0.6968, -1.0214, -0.9538]
            Neuron 10 weight: [0.1722, 0.0289, 0.2802, -0.8906, -0.8469]
        Layer 1
            Neuron 1 weight: [-1.26, 0.6871, -1.4164, -0.5938, 0.747, 0.788, 0.7755, 0.563, 0.7749, 0.6852, 0.497]
            Neuron 2 weight: [-1.4155, 0.6604, -1.4465, -0.6081, 0.7447, 0.7729, 0.8178, 0.6251, 0.7848, 0.6878, 0.4502]
            Neuron 3 weight: [-0.9724, 0.7267, -1.4643, -0.5558, 0.8418, 0.8782, 0.8277, 0.7708, 0.8736, 0.7667, 0.6983]
            Neuron 4 weight: [-1.6713, 0.5456, -1.4285, -0.7249, 0.6553, 0.7814, 0.7067, 0.4718, 0.7104, 0.6175, 0.3086]
            Neuron 5 weight: [-0.8456, 0.7617, -1.5106, -0.5363, 0.8595, 0.9498, 0.9269, 0.7675, 0.837, 0.8358, 0.7262]
            Neuron 6 weight: [-1.57, 0.5895, -1.4044, -0.6876, 0.6503, 0.773, 0.75, 0.4776, 0.6964, 0.6479, 0.4031]
            Neuron 7 weight: [-1.6354, 0.537, -1.4019, -0.6768, 0.6317, 0.7862, 0.7184, 0.4496, 0.7375, 0.6206, 0.3054]
            Neuron 8 weight: [-1.4774, 0.5671, -1.4255, -0.5977, 0.7448, 0.7279, 0.765, 0.5799, 0.7708, 0.6647, 0.4311]
            Neuron 9 weight: [-1.034, 0.7365, -1.4704, -0.5715, 0.8133, 0.8232, 0.8579, 0.644, 0.8577, 0.7756, 0.6033]
            Neuron 10 weight: [-1.8894, 0.4918, -1.4186, -0.7821, 0.6797, 0.7884, 0.7418, 0.4129, 0.7502, 0.6032, 0.2478]
        Layer 2
            Neuron 1 weight: [2.4642, -0.4025, -0.5005, -0.2483, -0.6474, -0.1621, -0.5763, -0.6831, -0.5632, -0.2919, -0.7693]
            Neuron 2 weight: [1.6104, -1.182, -1.275, -1.2809, -1.2093, -1.2791, -1.1902, -1.1193, -1.2363, -1.2673, -1.2046]
            Neuron 3 weight: [2.4225, -0.4264, -0.5149, -0.2135, -0.7054, -0.1406, -0.6002, -0.6152, -0.524, -0.2674, -0.7865]
            Neuron 4 weight: [2.9262, -0.4602, -0.5535, -0.2368, -0.7622, -0.1608, -0.6458, -0.7121, -0.5547, -0.3398, -0.9047]
            Neuron 5 weight: [1.7714, -0.3524, -0.4415, -0.292, -0.5096, -0.2771, -0.534, -0.4896, -0.4347, -0.2927, -0.6969]
            Neuron 6 weight: [1.8453, -1.3039, -1.4327, -1.3491, -1.3453, -1.3643, -1.3029, -1.2283, -1.3307, -1.369, -1.3068]
            Neuron 7 weight: [1.3216, -1.0574, -1.1424, -1.1531, -1.0229, -1.158, -1.0921, -1.0303, -1.1142, -1.1008, -1.1111]
            Neuron 8 weight: [1.5365, -1.2115, -1.2482, -1.1885, -1.1701, -1.2248, -1.1475, -1.1918, -1.1569, -1.2433, -1.1624]
            Neuron 9 weight: [2.8754, -0.4273, -0.5757, -0.2497, -0.744, -0.1219, -0.669, -0.6644, -0.5878, -0.316, -0.9089]
            Neuron 10 weight: [1.6639, -1.2095, -1.3565, -1.3094, -1.1802, -1.2773, -1.2462, -1.1517, -1.2597, -1.2624, -1.231]
        Layer 3
            Neuron 1 weight: [4.0638, -2.4349, -1.9087, -2.4099, -2.4996, -2.3437, -1.9969, -2.0528, -2.0818, -2.4501, -2.0024]
            Neuron 2 weight: [-3.4872, 2.0008, -2.8269, 2.0017, 2.5099, 1.1701, -3.2323, -2.1416, -2.5853, 2.5107, -2.8976]
            Neuron 3 weight: [-7.4767, 0.8404, 2.1358, 0.7707, 0.7258, 1.085, 2.2899, 2.0824, 2.1612, 0.6205, 2.1533]

        Total test error = 3.3333%


        --- Execution time: 36.852384090423584 seconds ---

Both of which occasionally reach 0% test error.

### Appendix: List of Results

    raw
    ├── iris.csv_it1000_layer3_10_10_10.txt
    ├── iris.csv_it1000_layer3_3_2_3.txt
    ├── iris.csv_it1000_layer3_4_4_4.txt
    ├── iris.csv_it1000_layer4_10_10_10_10.txt
    ├── iris.csv_it1000_layer4_4_6_6_4.txt
    ├── iris.csv_it1000_layer4_5_5_5_5.txt
    ├── iris.csv_it1000_layer4_6_8_8_6.txt
    ├── iris.csv_it1000_layer8_10_8_8_8_8_8_8_10.txt
    ├── iris.csv_it1000_layer8_15_10_10_10_10_10_10_15.txt
    ├── iris.csv_it1000_layer8_6_6_6_6_6_6_6_6.txt
    ├── iris.csv_it2000_layer3_10_10_10.txt
    ├── iris.csv_it2000_layer3_3_2_3.txt
    ├── iris.csv_it2000_layer3_4_4_4.txt
    ├── iris.csv_it2000_layer4_10_10_10_10.txt
    ├── iris.csv_it2000_layer4_4_6_6_4.txt
    ├── iris.csv_it2000_layer4_5_5_5_5.txt
    ├── iris.csv_it2000_layer4_6_8_8_6.txt
    ├── iris.csv_it2000_layer8_10_8_8_8_8_8_8_10.txt
    ├── iris.csv_it2000_layer8_15_10_10_10_10_10_10_15.txt
    ├── iris.csv_it2000_layer8_6_6_6_6_6_6_6_6.txt
    ├── iris.csv_it200_layer3_10_10_10.txt
    ├── iris.csv_it200_layer3_3_2_3.txt
    ├── iris.csv_it200_layer3_4_4_4.txt
    ├── iris.csv_it200_layer4_10_10_10_10.txt
    ├── iris.csv_it200_layer4_4_6_6_4.txt
    ├── iris.csv_it200_layer4_5_5_5_5.txt
    ├── iris.csv_it200_layer4_6_8_8_6.txt
    ├── iris.csv_it200_layer8_10_8_8_8_8_8_8_10.txt
    ├── iris.csv_it200_layer8_15_10_10_10_10_10_10_15.txt
    ├── iris.csv_it200_layer8_6_6_6_6_6_6_6_6.txt
    ├── iris.csv_it8000_layer3_10_10_10.txt
    ├── iris.csv_it8000_layer3_4_4_4.txt
    ├── iris.csv_it8000_layer4_10_10_10_10.txt
    ├── iris.csv_it8000_layer4_4_6_6_4.txt
    ├── iris.csv_it8000_layer4_5_5_5_5.txt
    ├── iris.csv_it8000_layer4_6_8_8_6.txt
    ├── iris.csv_it8000_layer8_10_8_8_8_8_8_8_10.txt
    ├── iris.csv_it8000_layer8_15_10_10_10_10_10_10_15.txt
    └── iris.csv_it8000_layer8_6_6_6_6_6_6_6_6.txt

    0 directories, 39 files
