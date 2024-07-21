# Simple-image-converter
Simple image converteris a user-friendly tool that converts image files between DDS and PNG formats. With a simple GUI, users can select a source folder and an output folder, specify the conversion direction, and start the process. The program displays real-time progress and completes the conversion with a single click.
The Image Converter is a versatile and user-friendly application designed to convert image files between various formats. It supports both single file and batch conversions, providing an intuitive graphical user interface (GUI) that dynamically resizes and remembers the user's last-used directories.

Technologies Used
Programming Language: Python
GUI Framework: Tkinter (enhanced with ttkthemes for improved styling)
Image Processing Library: Python Imaging Library (PIL) via the Pillow library
Threading: Used for asynchronous operations to ensure the GUI remains responsive during conversions
Configuration Management: JSON for storing and loading persistent user settings

Core Features
Multi-Format Support:
Convert images between various formats including PNG, DDS, JPEG, BMP, TIFF, and GIF.
Single File Mode:
Easily convert individual image files.
Folder Mode:
Batch convert all image files in a selected folder.
Persistent Directories:
The application remembers the last used input and output directories, enhancing user convenience.
Dynamic GUI Resizing:
The layout adapts to different window sizes, ensuring a consistent and user-friendly experience.
Loading Spinner:
Provides visual feedback during long conversion processes.
Scrollable Log Output:
Displays conversion progress and status updates clearly.

Application Structure
Main Application:
Built with ThemedTk from the ttkthemes package for a modern look and feel. Uses Tkinter widgets for the GUI.
Configuration Management:
Loads and saves user settings using JSON files, ensuring persistent working directories.
Image Conversion:
Implemented using the Pillow library, which extends the capabilities of PIL to handle multiple image formats.
Threading:
Utilizes threading to perform image conversions asynchronously, keeping the GUI responsive.
Loading Spinner:
A custom loading spinner implemented with Tkinter's Canvas widget to provide visual feedback during conversions.

Usage Instructions
Running the Application:
Double-click on ImageConverter.exe to launch the application.
Selecting Input Mode:
Use the slider at the top to switch between Folder Mode and Single File Mode.
Selecting Input and Output:
In Folder Mode, click on the "Select Input Folder" button to choose the folder containing images. Click on the "Select Output Folder" button to choose the folder where converted images will be saved.
In Single File Mode, click on the "Select Input File" button to choose the image file to convert. Click on the "Select Output Folder" button to choose the folder where the converted image will be saved.
Choosing Image Formats:
Use the "Input Format" dropdown to select the format of the input images.
Use the "Output Format" dropdown to select the format you want to convert the images to.
Starting the Conversion:
Click on the "Start Conversion" button to begin the conversion process. A loading spinner will indicate that the conversion is in progress, and the log output section will display the progress and status.

Known Issues
GUI Scaling:
Minor visual inconsistencies may occur when using extreme window sizes.
Conversion Speed:
Converting large batches of high-resolution images can be time-consuming. Further optimizations are planned for future releases.





Changelog: 

After listening to feedback
-regarding wishes to implement singular file conversions and that the program should be able to remember the different directorys 

UPDATE 1.2

CHANGELOG
·        Added support for converting between multiple image formats, including PNG, DDS,
JPEG, BMP, TIFF, and GIF.
·        Replacedradio buttons with dropdown comboboxes for selecting input and output image
formats.
·        Improvedusability by providing a clear selection method for desired formats.

BUG FIXES
FixedButton Overlap Issues:
Resolvedissues where buttons overlapped with other elements, ensuring all buttons are
clickable and properly positioned.
AddressedGUI Layout Problems:
Fixedlayout problems that caused elements to shift unexpectedly, especially when
switching between single file and folder modes.


UPDATE 1.1 

Single File and Folder Mode:
Implemented a slider to switch between "Single File Mode" and "Folder Mode."
Updated GUI elements to support both modes.
 PersistentWorking Directory:
Configurations are saved to config.json and reloaded upon application start.
User Feedback:
Notifications for successful and failed conversions.
Improved error handling and logging.
## License

This project is licensed under a custom license. Please refer to the `LICENSE` file for details.
