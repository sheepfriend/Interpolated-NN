# Interpolated-NN
The code reproduces the results in paper "Benefit of Interpolation in Nearest Neighbor Algorithms" in https://epubs.siam.org/doi/abs/10.1137/21M1437457

Two folders "inter" and "inter_same_k":
Each folder contains one regression model and two classification models.
To run inter.py and cis.py, use
    python inter.py $GAMMA_NUM $LOG_N $D
    python cis.py $GAMMA_NUM $LOG_N $D

    GAMMA_NUM: the index of the gamma in [0.05,0.1,0.15,0.2,0.25,0.3,0.35,0.4]
    LOG_N: log2(n), n is the number of samples
    D: data dimension

To reproduce the figures, use inter_plot_regre.py and inter_plot_tmp.py. The address should be modified in code
"""
model=PATH_TO_MODEL
"""


real_inter:
To run real_inter.py, use
    python real_inter.py $NAME $GAMMA_NUM

    NAME is in ['mnist_small','mnist','HTRU2','Credit','Abalone']


