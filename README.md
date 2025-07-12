# hackathon-2023

Project developed at the computer vision hackathon organized by the Meninas++ project, sponsored by Pix Force, and hosted by UFV. The project achieved 2nd place.

## 1. Introduction

This document describes a Python solution for the automatic correction of multiple-choice tests and quizzes. It uses computer vision and machine learning to read the answer key, analyze students' answer sheets, compare responses, and generate individual reports. Additionally, it includes a data management system to store results in an organized manner.

## 2. Project Objective

The main objective of this project is to automate the multiple-choice test correction process, providing efficiency and accuracy in evaluating student results.

## 3. Features

### 3.1. Answer Key Reading

The web app can read and interpret the test's answer key, identifying correct answers for each question. This is done through image processing and pattern analysis techniques, including optical mark recognition (OMR), Python, and the OpenCV library.

### 3.2. Answer Sheet Reading

The web app can analyze students' filled-out answer sheets, identifying marked options for each question. Using advanced computer vision techniques, particularly optical mark recognition, the system accurately extracts markings.

### 3.3. Comparison and Scoring

Based on the answer key and the answer sheet readings, the solution compares students' responses with correct answers, assigning a score to each question. The score is calculated based on the match between students' choices and correct answers.

### 3.4. Individual Reports

Generates individual reports for each student, highlighting correct and incorrect answers, along with the final score. These reports are presented in a clear and understandable manner to facilitate understanding of individual performance.

## 4. Data Management

Correction results are stored in an organized data management system (SQLite). This allows easy and fast access to past information, enabling historical analysis, pattern identification, and continuous system improvement.

## 5. Technologies Used

- Flask
- Sqlite3
- Tailwindcss
- Flowbite
- JavaScript
- Cv2
- Numpy
- Imutils

## 6. System Architecture

### 6.3. Web Interface Module

- Development of a web interface to facilitate image loading and display of results.
- Integration with image processing and machine learning modules.
- Generation of correction reports for each test or quiz.

## 7. Workflow

### 7.1. Presented Features:

- The user uploads the answer sheet image through the web interface.
- Class registration
- Student registration
- Test registration
- Answer key registration

### 7.2. Image Processing:

- The image is processed to enhance markings.
- Relevant areas are identified using computer vision techniques.

### 7.3. Machine Learning:

- The trained model is applied to classify marked responses.
- Model accuracy is verified using validation techniques.

### 7.4. Report Generation:

- A correction report is generated, showing correct and incorrect answers.
- The web interface displays results in an accessible way for teachers and students.

## 8. System Requirements

- Python 3.11
- Libraries: OpenCV, NumPy, Imutils

## 9. Installation and Configuration

Clone the repository to your local system:

```
git clone https://github.com/luizvilasboas/hackathon-2023.git
```

Navigate to the project directory:

```
cd hackathon-2023
```

Create a virtual environment to isolate project dependencies:

```
python -m venv venv
```

Activate the virtual environment:

On Windows:

```
venv\Scripts\activate
```

On macOS/Linux:

```
source venv/bin/activate
```

Install project dependencies:

```
pip install .
```

Now that the environment is set up, you can start the Flask server. Make sure you are in the project directory with the virtual environment activated.

```
flask --app snapcorrect run
```

## 11. Conclusion

The system provides an efficient and automated solution for correcting multiple-choice tests and quizzes, saving time and minimizing errors. The combination of computer vision and machine learning offers a robust and accurate approach to meet the needs of large-scale correction. The system is flexible and can be adapted to different types of multiple-choice assessments.
