# Dense_Pakcing

This is the code running the simulations described in "Dense packing of the surface code: code deformation procedures and hook-error-avoiding gate scheduling".

## Environment

-Python 3.11.6

-stim 1.15.0

-sinter 1.15.0

-pymatching 2.3.0

-numpy 1.26.4

-matplotlib 3.10.6

-scipy 1.16.1

The simulations were executed in the above environment.
Although the code may work with other versions of Pythons or these libraries, compatibility has not been tested.

## How to run

This repository provides code to evaluate the logical error rates of individual logical qubits in a densely packed surface code composed of five logical qubits.

Each logical qubit is specified by its position within the dense packing. The available options are:

- leftmost
- second_from_the_left
- center
- second_from_the_right
- rightmost

To evaluate the logical error rate of a specific logical qubit, specify its position using the `--mode` argument. For example, to evaluate the leftmost logical Z error rate, run:

```bash
python3 dense_packing_simulation_z_error.py --mode leftmost
```
To evaluate center logica X error rate, run:
```bash
python3 dense_packing_simulation_x_error.py --mode center
```



