# Medical-Data-Extraction-using-OCR 🏥💻

### This project focuses on automating the extraction of useful data from patient details and prescription images for health insurance companies. Currently, many insurance companies rely on manual data extraction, which is time-consuming and prone to errors. To overcome these challenges, this project proposes a Test-driven development solution using Python. 📚🔬

### The solution approach involves using the Pytesseract library for **optical character recognition (OCR)** to extract text from images. The extracted data is then processed using regular expressions to obtain the desired output. The workflow of the project can be summarized as follows: 📝➡️🔍

## **PDF to Image Conversion** 📄🖼️:
The pdf2image library is used to convert PDF documents into images for further processing.

## **Extraction without Preprocessing** 🚫🔄:
Initially, attempts are made to extract data directly from the source files without any preprocessing. However, the results are not satisfactory due to the unstructured format of the data.

## **Image Processing** 🌄🔧:
To improve data extraction, the OpenCV library is employed for image preprocessing. Initially, normal thresholding is applied, but it may result in the loss of data in areas with shadows or noise. As a better alternative, adaptive thresholding is used, which divides the image into sub-regions and applies different thresholding values to each region, resulting in improved accuracy.

## **Data Extraction after Preprocessing** 💾🔍:
With the preprocessed image, OCR is performed using pytesseract to extract the text data. The extracted data is then processed using regular expressions to match patterns and extract the required information from medical documents.

## **Test-driven Development** 🧪🔧:
Throughout the development process, pytest is used for test-driven development. Test cases are designed to validate methods' functionality and ensure the extracted data's accuracy.

## **FastAPI and Postman** 🚀📬:
FastAPI hosts the project's server, providing fast performance, built-in data validation, and documentation. Postman is used to send HTTP requests and test the server's responses.

## Results 📊📈:
The resulting backend functionality can be integrated into Mr. X Analytics' existing software, allowing for automatic data extraction. While the extracted data may still require manual verification and correction, this solution significantly reduces the time and effort required for data entry. The benefits of this project include time savings for Mr. X Analytics, the ability to process more documents within deadlines, reduced hiring needs, and lower error rates due to a combination of automation and manual verification.

## Benefits 🌟📈:
- **Time Savings**: The automation of data extraction reduces the time required for processing each document. By saving at least 30 seconds per document, cumulatively, it leads to significant time savings. This enables Mr. X Analytics to complete more documents within the given time frame and increase overall efficiency.
- **Cost Savings**: With automated data extraction, the need to hire additional workforce during peak seasons or for handling a large volume of documents is reduced. This translates to cost savings for Mr. X Analytics as they can manage the workload with existing resources.
- **Reduced Errors**: While automation is employed for data extraction, human verification and correction are still involved. This combination of automation and manual review significantly reduces the occurrence of errors compared to manual data entry alone. The extracted data can be cross-checked and corrected by the person performing the task, ensuring higher accuracy.
- **Scalability**: By implementing an automated solution, Mr. X Analytics can easily scale their operations to handle a larger volume of documents. They can process more documents within a given time period without the need for substantial manpower.
- **Improved Profitability**: By reducing the time and effort required for data entry, Mr. X Analytics can increase their productivity and handle more clients or projects. This ultimately leads to improved profitability for the company.
- **Seamless Integration**: The backend functionality of the project can be seamlessly integrated into Mr. X Analytics' existing software infrastructure. This allows for a smooth transition from manual data entry to automated data extraction without disrupting the existing workflow.
