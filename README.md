# Open-Source-Medical-Website

## Overview  
Open Source Medical Software is a web application created as a semester project by Sagnik Dey and Rahul Kumar. It aims to simplify medical data analysis and enhance healthcare accessibility.  
This Flask-based web application allows users to upload previous and latest prescriptions in PDF format to compare medications, their strengths, and dosage forms. The app also features user authentication with signup and login functionality.

## Repository  
The project repository is maintained by Sagnik Dey and can be found [here](https://github.com/sagnik-create/Medbud).  

## Features

- **User Authentication**: Users can sign up and sign in to access their personalized dashboard.
- **PDF Prescription Analysis**: The application extracts text from prescription PDFs and compares the medications, checking their strengths against a dataset of medicines.
- **Comparison with Dataset**: The app checks medication strength and form (tablet, syrup, etc.) from a provided dataset of medicines.

## Prerequisites

Before running the application, make sure you have the following installed:

- Python 3.7+
- Flask
- Pandas
- PyPDF2

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/sagnik-create/Wellnest.git
   cd medbud-app
   ```

2. Create a virtual environment and activate it:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required packages:

   ```bash
   pip install Flask pandas PyPDF2
   ```

4. Place your `medicine_dataset.csv` file in the `/mnt/data/` directory.

5. Make sure the directory structure for user pages is in place:

   ```bash
   mkdir users
   ```

## Running the Application

1. Run the Flask application:

   ```bash
   python app.py
   ```

2. Open your browser and navigate to:

   ```
   http://127.0.0.1:5000/
   ```

## Usage

### Sign Up

1. Navigate to the sign-up page.
2. Enter your username, email, and password to create an account.

### Log In

1. Enter your username and password on the login page to access your personalized dashboard.

### Analyze Prescription

1. Upload both the previous and latest prescription PDFs.
2. The app will extract text from both prescriptions, compare the medications, and present the differences (e.g., increased dosage).
3. The analysis results will be compared to the `medicine_dataset.csv` file to check for standard strengths and dosage forms.

## File Structure

```
├── app.py
├── templates
│   ├── first.html
│   ├── index.html
│   ├── signin.html
│   ├── signup.html
│   ├── user.html
│   └── prescription_analysis.html
├── users
│   └── (auto-generated HTML files for users)
├── mnt
│   └── data
│       └── medicine_dataset.csv
└── README.md
```

## Dataset

The app uses a dataset (`medicine_dataset.csv`) that contains medicine information such as:

- **Name**: The name of the medicine.
- **Strength**: The strength (e.g., 500 mg).
- **Dosage Form**: The form in which the medicine is administered (e.g., tablet, syrup).

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

## Contact
kadvasararahul@gmail.com
