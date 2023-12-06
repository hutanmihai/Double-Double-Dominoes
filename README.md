# Computer Vision - Project 1 - Double Double Dominoes

## Author

- Hutan Mihai Alexandru
- Github: [hutanmihai](https://github.com/hutanmihai)
- LinkedIn: [Mihai-Alexandru Hutan](https://www.linkedin.com/in/hutanmihai/)

## The problem statement can be found here: [Problem.pdf](./Problem.pdf)

## For a detailed explanation of the solution please read the [report](./documentation.pdf).

## Required Libraries

python=3.11.5
opencv-python==4.8.1.78
numpy==1.26.0

### Install required libraries using conda

This is the recommended way of installing the required libraries.

```bash
conda create --name computer-vision-project-1 python=3.11.5
conda activate computer-vision-project-1
pip install opencv-python==4.8.1.78
pip install numpy==1.26.0
```

### Install required libraries using pip

Make sure you have python 3.11.5 installed on your system and you are using it.

```bash
pip install opencv-python==4.8.1.78
pip install numpy==1.26.0
```

## How to run the project

Setup the constants in the `src/constants.py` file.
Please only change the values of the constants and do not change their names.

Optional constants that can be set to `True` or `False` depending on what you want to visualize.
If none of them are set to `True` then the program will not display any images.
If all of them are set to `True` then the program will display all the images but it will take a while to go through
them all.

```python
SHOW_BOARD_EXTRACTION_POINTS = False
SHOW_BOARD_LINES = False
SHOW_PATCHES = False
SHOW_TEMPLATES_ON_GENERATION = False
SHOW_PATCHES_PREPROCESSING = False
SHOW_DETECTED_PIECES = False
SHOW_BOARD_EXTRACTION_STEPS = False
SHOW_AUGMENTATION_STEPS = False
```

Make sure you are in the root directory of the project.

```bash
export PYTHONPATH=.
python src/main.py
```

For evaluation if the mode you used was train run the following command:

```bash
python src/eval_train.py
```

To change from train to test mode change the following line in `src/constants.py`:

```python
MODE = "train"  # "train" or "test"
```

To run the train data and augment it change the following line in `src/constants.py`:

```python
AUGMENT_DATA = True  # True or False
MODE = "train"
```

For evaluation if the mode you used was test run the following command:

```bash
python src/eval_test.py
```
