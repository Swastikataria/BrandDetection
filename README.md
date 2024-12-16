# Brand Detection Model

## Overview
The **Brand Detection Model** is an innovative solution designed to automatically identify and categorize brands into pre-defined categories. This model uses Optical Character Recognition (OCR) technology combined with fuzzy string matching to accurately detect brand names from live camera feeds or uploaded images.

By categorizing products efficiently, this system enhances stock management, inventory tracking, and provides actionable insights for businesses. Deployed locally using **Flask**, it offers a seamless, real-time solution for brand recognition.
![image](https://github.com/user-attachments/assets/9d7d0b90-209c-48c3-bb6b-5ad0056a4e12)


## Key Features
- **Brand Detection & Categorization**: Detects brands from product packaging and assigns them to appropriate categories (e.g., Food & Beverages, Personal Care).
- **Optical Character Recognition (OCR)**: Extracts textual information from live video frames using OCR technology.
- **Fuzzy Matching**: Ensures reliable brand recognition by matching detected text against a predefined list of brand names.
- **Live Camera Integration**: Captures real-time video feed from connected camera hardware for on-the-fly detection.
- **Dynamic Updates**: Stores detection results, such as brand names and their categories, for efficient tracking and monitoring.
- **Inventory Insights**: Can be integrated with stock management systems to alert when specific products are running low.
- **Local Deployment**: Runs locally using **Flask** for easy accessibility and minimal dependencies.


## Applications
- **Inventory Management**: Helps businesses track stock levels and identify missing products.
- **Retail Solutions**: Automates product identification in stores, warehouses, or supermarkets.
- **Quality Control**: Ensures all products are properly categorized for streamlined operations.
- **Smart Vision Technology**: Offers a quick, hardware-assisted method to solve inventory and categorization challenges.
- **Dynamic Notification System**: Alerts when specific brands or product types are not detected, aiding restocking decisions.


## Technology Stack
- **Python**: Core programming language.
- **Flask**: Backend framework for local deployment and server management.
- **OpenCV**: For live video capture and image processing.
- **EasyOCR**: OCR library for text detection and extraction from images.
- **FuzzyWuzzy**: Implements fuzzy string matching to identify brands accurately.
- **HTML/CSS**: Simple frontend for visualization of results.
- **CSV Storage**: Results are stored dynamically in a CSV file for easy analysis.


## Workflow
1. **Video Feed Capture**: The application accesses the live camera feed using OpenCV.
2. **Text Detection**: EasyOCR processes each video frame and extracts textual data.
3. **Brand Matching**: Extracted text is matched against a predefined list of brands using fuzzy matching.
4. **Categorization**: The detected brand is assigned to one of the following categories:
   - Food & Beverages
   - Personal Care
   - Household Items
   - Baby Care
   - Electronics & Accessories
5. **Result Storage**: Detection results (Frame number, Brand name, and Category) are saved in a CSV file.
6. **Live Display**: The recognized brand and category are displayed in real-time on the video feed.


## Deployment
The Brand Detection Model is deployed locally using **Flask**. Follow these steps to set it up:

1. Clone the project repository.
   ```bash
   git clone <repository-link>
   cd brand-detection-model
   ```
2. Install the required dependencies.
   ```bash
   pip install flask easyocr opencv-python fuzzywuzzy python-Levenshtein
   ```
3. Run the application.
   ```bash
   python app.py
   ```
4. Open a web browser and visit `http://127.0.0.1:5000` to view the live brand detection feed.


## Output
- **Real-Time Detection**: Display of detected brand names and categories on live video feeds.
- **CSV File**: Results are stored in `live_camera_results.csv` with details of frame numbers, detected brands, and their categories.


## Benefits
- **Improved Stock Management**: Accurately categorizes and tracks brands for better inventory control.
- **Quick & Reliable**: Leverages OCR and fuzzy matching for fast and accurate text recognition.
- **Real-Time Processing**: Processes live camera feeds to detect brands on-the-go.
- **Innovative Solution**: Combines advanced vision technology with practical business applications.
- **Scalable**: Can be integrated with IoT devices and hardware for large-scale deployments.


*Table shown even on UI*
![image](https://github.com/user-attachments/assets/3f32abb0-b2fe-41bc-a641-e48241241b45)

