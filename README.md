# XpertMeterReader

**Goal**

The goal of the Automated Meter Reading Solution is to streamline the process of reading digital electronic meters by automating the extraction of meter readings from mobile camera images. By leveraging machine learning models such as Faster R-CNN and YOLO, the solution aims to accurately detect and record meter readings from images, eliminating the need for manual data entry. This automation reduces the potential for human error and saves time and resources traditionally spent on manual meter reading processes.

**Functionality**

  **1. Image Tagging and Preparation**
  
  Tagging Images: Users can tag images captured by a mobile camera to indicate the presence of meter readings, facilitating organization and preparation for processing.
  
  **2. Machine Learning Models**
  
  Faster R-CNN and YOLO Models: The solution utilizes advanced machine learning models, including Faster R-CNN and YOLO, to detect and extract numbers from meter images.
  
  **3. Automated Data Extraction**
  
  Record Numbers into Excel Sheet: Detected meter readings are automatically saved into an Excel sheet or a structured database, eliminating the need for manual data entry.
  
  **4. Error Reduction and Efficiency**
  
  Reduced Human Error: Automation of the meter reading process reduces the potential for human error associated with manual data entry.
  
  Time and Resource Savings: By automating meter reading, the solution saves time and resources, leading to increased efficiency in meter management.

**How it Operates**
  
  1. Capture Meter Image:
  Users initiate the process by entering their consumer number and capturing the meter image using the DISCOM app. The image is then transmitted to the XAMR Application.
  2. Image Validation:
  On the XAMR application, the captured image undergoes validation to ensure its authenticity. If the image passes the validity check, the process moves forward. In cases of invalid images, users are prompted to retake the image for accuracy.
  3. Readability Check & Data Input:
  The XAMR application verifies the readability of the image. If the image is deemed unreadable, users are prompted to retake it for clarity. Upon confirming readability, users input the manual reading.
  4. Data Forwarding and Offline Storage Protocol:
  The consumer number, manual reading, and readable image data are then forwarded to both the DISCOM server and AMR server. In situations where internet connectivity is unavailable, the data is securely stored within the XAMR app's local database until connectivity is restored.
  5. Processing on AMR Server:
  Upon arrival at the AMR server, an algorithm conducts an analysis to identify any anomalies in the meter reading. If anomalies are detected, the meter reading undergoes correction. Additionally, if fraudulent activity is detected, both the corrected meter reading and evidence of the fraud are forwarded to the DISCOM server for appropriate actions.

[![XpertMeterReader](http://img.youtube.com/vi/qNIhTDREQjw/0.jpg)](http://www.youtube.com/watch?v=qNIhTDREQjw"XpertMeterReader”)
