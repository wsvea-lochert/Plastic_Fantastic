# Plastic-Fantastic
 Quick image augmentation library for myself.

## Requirements
* Keras/TensorFlow
* PIL
* Numpy
* tqdm
* SciPy

## Code snippets

### horizontal_img_shift()
Shifts the images horizontally withing the shift_range.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.horizontal_img_shift(shift_amount=[-250, 250])
```

### vertical_img_shift()
Shifts the images vertically withing the set shift_amount.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.vertical_img_shift(shift_amount=0.5)
```

### horizontal_img_flip()
Flips the images horizontally.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.horizontal_img_flip()
```

### img_dir.vertical_img_flip()
Flips the images vertically.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.vertical_img_flip()
```

### img_dir.random_img_rotation()
Randomly rotates the images in the set rot_range.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.random_img_rotation(rot_range=90)
```

### random_img_brightness()
Randomly adjust the brightness of the images within the set b_range.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.random_img_brightness(b_range=[0.2, 1.0])
```

### random_img_zoom()
Randomly zoomes the images according to the set z_range.
```python
img_dir = ImageAugment(data_dir='path_to_directory', output_path='path_to_output_dir')
img_dir.random_img_zoom(z_range=[0.5, 1.0])
```