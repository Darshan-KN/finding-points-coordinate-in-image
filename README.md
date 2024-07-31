# finding-points-coordinate-in-image

Certainly! Here's the content for your `README.md` file:

---

# Finding Points Coordinates in Images

## Introduction

This project aims to detect specific points in images and extract their coordinates. By providing an image link, the program identifies and returns the coordinates of the points of interest. The project is designed to work with images where the points are clearly distinguishable, such as images with marked fiducial points or specific patterns.

## Table of Contents

1. [Features](#features)
2. [Usage](#usage)
   - [Detecting Points](#detecting-points)
   - [Specifying Coordinates](#specifying-coordinates)
3. [Examples](#examples)
4. [Acknowledgments](#acknowledgments)

## Features

- **Automatic Point Detection**: Detects points in images and extracts their coordinates.
- **Custom Coordinate Specification**: Allows users to specify points' coordinates if known.
- **Image Visualization**: Displays the image with detected points marked for verification.
- **Flexible Input**: Supports both image links and local image files.



## Usage

### Detecting Points

To detect points in an image, provide the image URL or path to the image file:

```python
from point_detection import detect_points

image_url = "https://example.com/path/to/your/image.jpg"
coordinates = detect_points(image_url)
print("Detected coordinates:", coordinates)
```

### Specifying Coordinates

If you already know the coordinates of certain points, you can specify them directly:

```python
from point_detection import plot_points

known_coordinates = [(50, 100), (150, 200), (250, 300)]
plot_points(image_url, known_coordinates)
```

## Examples

### Example 1: Automatic Detection

**Input Image:**

![BMJHSET2AP_points_plot](https://github.com/user-attachments/assets/a9183eb4-b7d8-4c80-a011-fe3c97327f65)

**Detected Points:**

```
X	Y	Point Number
106	228	1
91	222	2
173	214	3
186	209	4
36	184	5
29	171	6
223	152	7
229	139	8
230	111	9
16	105	10
22	91	11
216	71	12
210	59	13
60	35	14
72	28	15
152	20	16
141	15	17


```

**Output Image:**

![BMJHSET2AP_points_plot_annotated](https://github.com/user-attachments/assets/0f762134-819f-4010-b246-096b637f32a6)



## Acknowledgments

Special thanks to the open-source community for providing the libraries and tools used in this project.

---

Replace placeholders such as `https://github.com/your-username/your-repo-name.git` and `path/to/input_image.jpg` with your actual GitHub repository link and image paths or URLs, respectively.
