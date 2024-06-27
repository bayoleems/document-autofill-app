
# AUTOFILL DOC APP

# Form Generator and Auto-Fill from DOCX

### Project Overview

This project is designed to streamline the process of generating forms from DOCX files and subsequently auto-filling those forms. The system identifies text within double square brackets (e.g., `[[Full Name]]`) in a DOCX file and uses these notifiers to generate corresponding form fields. Users can fill out these forms, and the system will automatically update the original DOCX file with the provided input, replacing the placeholders with the user-entered data. The final DOCX file is then available for download.

### Features

- **DOCX Parsing**: Reads and parses DOCX files to identify placeholders.
- **Form Generation**: Automatically generates a form based on identified placeholders.
- **Auto-Fill Functionality**: Replaces placeholders in the DOCX file with user-provided input.
- **File Download**: Provides the updated DOCX file for download.

### Requirements

- Python 3.x
- `python-docx` library for DOCX file manipulation
- `Flask` for the web interface
- `threading` for scheduling

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/bayoleems/document-autofill-app.git
    cd autofill-doc-app
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

### Usage

1. **Start the application**:
    ```sh
    python main.py
    ```

2. **Upload DOCX File**:
    - Access the web application at `http://localhost:5050`
    - Upload a DOCX file containing placeholders in the format `[[Placeholder Name]]`.

3. **Fill the Form**:
    - The application will generate a form based on the placeholders identified in the uploaded DOCX file.
    - Fill in the form fields with the necessary information.

4. **Download the Updated DOCX**:
    - After submitting the form, the system will replace the placeholders in the DOCX file with the provided input.
    - The updated DOCX file with the placeholders replaced by the user-provided data will be automatically downloaded.

### Example

#### Input DOCX File
```plaintext
Dear [[Full Name]],

We are pleased to inform you that your application for the position of [[Job Title]] has been approved.

Sincerely,
[[Company Name]]
```

#### Generated Form
```
Full Name: _______________
Job Title: _______________
Company Name: _______________
```

#### Output DOCX File
```plaintext
Dear John Doe,

We are pleased to inform you that your application for the position of Software Engineer has been approved.

Sincerely,
Tech Solutions Inc.
```

### Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request


### Contact

If you have any questions or feedback, feel free to reach out:

- **Email**: bayoleems@gmail.com
- **GitHub**: [bayoleems](https://github.com/bayoleems)

---

Thank you for using the AUTOFILL DOC APP project! We hope it makes your job more efficient and effective.