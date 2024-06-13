# Image Browser Application

This image browser application is built with PyQt5 and is used to browse image files in a specified directory. It can also calculate the Dice coefficient and IoU for images. The application supports taking screenshots, which are saved to the clipboard and the current directory.

## Features

- **Open Directory**: Choose a directory to browse the image files within it.
- **Image Display**: Display the original image, mask image, and predicted image of the selected file from the directory.
- **Calculate Dice and IoU**: Calculate the Dice coefficient and IoU between the mask image and predicted image of the selected file.
- **Screenshot**: Use the shortcut Ctrl+A to take a screenshot of the current application window and save it to the clipboard and the current directory.

## Installation

Make sure the following dependencies are installed:

- Python 3.x
- PyQt5
- Pillow (PIL)
- NumPy

You can install these dependencies using the following command:

```
pip install PyQt5 pillow numpy
```

## How to Use

1. **Run the Application**:
   ```
   python image_browser.py
   ```

2. **Open Directory**:
   Click the **Open Directory** button in the interface and select a directory containing image files.

3. **Browse Images**:
   In the file list on the right, select a file. The application will display the original image, mask image, and predicted image (if available) for that file.

4. **Calculate Dice and IoU**:
   If the **Calculate Dice and IoU** checkbox is selected and matching mask and predicted images are available in the directory, the application will automatically calculate the Dice coefficient and IoU between them.

5. **Screenshot**:
   Use the shortcut **Ctrl+A** to take a screenshot of the current application window and save it to the clipboard and the current directory.

## Notes

- Ensure that the directory contains the correct image files: original image (ending with `image.png`), corresponding mask image (ending with `mask.png`), and predicted image (ending with `predict.png`).
- The screenshot functionality will capture the current application window and save it as a `screenshot.png` file.
