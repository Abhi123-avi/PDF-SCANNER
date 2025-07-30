This website seeks to assess the risk of cybersecurity vulnerabilities among average internet users who may be unaware of potential threats. By analyzing online attacks and threats, 
this project aims to identify areas where proactive security measures can mitigate risks and protect users from potential harm. The Malicious File Checker web application, built using 
JavaScript, provides valuable assistance to users who may not be familiar with internet security or lack extensive knowledge of online threats. The global variable function is used in 
the website to store the reference to the drop area where files can be uploaded. A drag-and-drop behavior function used in JavaScript-built antivirus web applications for preventing 
the default drag-and-drop behaviors. Additionally, a CSS class is applied to highlight the drop area when a file is dragged over it by users. The application initializes various elements 
(such as buttons and input fields) using event listeners to enhance user interaction. The 'handle drop' function is implemented for managing dropped files by users, when a PDF file is 
dropped, it displays the file name. This function ensures that only one file is accepted and verifies its validity, thereby improving the user experience during file uploads. The website 
alerts users if multiple files are dropped or if the file is incorrect. These functions collectively enable users to easily upload a single PDF file, receive visual feedback, and proceed 
with further analysis.
several effective approach involves employing a malicious file checker, which follows a well-defined process:
(a) Hash Calculation: Upon user file upload, the checker computes a cryptographic hash (such as SHA-256) for the uploaded file. This hash serves as a unique identifier for the file.

(b) Virus Total API Integration: The checker then initiates an API request to Virus Total, a reputable online service that aggregates threat intelligence from various antivirus engines.
    Using the calculated hash, it queries the virus total's extensive database.

(c) Malware Assessment: The API response provides crucial insights. It indicates whether the given PDF file is malicious or benign. If any malicious detections are found, the checker promptly alerts the users with an appropriate visual indicator (such as a red cross).

(d) Detailed Information Displays: Beyond the binary verdict, the checker enriches the user experience by presenting comprehensive details about the file:
    File Attributes: Name, type, and size.
    Temporal context: First seen date and last seen date.
    Usage Metrics: Submission count and detection count.
