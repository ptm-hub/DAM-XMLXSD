# DAM-XMLXSD
# Mobile Weather Report App – XML & XSD Project

## 1. App and API Description

This project represents a mobile application that sends weather-related data
to a remote database through a RESTful API using XML as the data exchange format.

The mobile app allows users to report weather conditions or incidents from
their mobile devices. The data is sent in XML format to a Node.js RESTful API,
which validates the incoming XML documents using an XML Schema (XSD) before
processing or storing the information.

The project is inspired by the professor’s example repository and focuses on
XML structure, validation, and data integrity.

---

## 2. Description of the Data Exchanged Between the App and the API

The information exchanged between the mobile app and the API includes:

- Report identifier
- Timestamp of the report
- User and device information
- Geographic location (city, latitude, longitude)
- Weather data (temperature, humidity, wind speed, precipitation)
- Type of weather incident

Two different XML documents are used to represent different data sources:

### XML Documents

1. **weather_report_manual.xml**
   - Simulates data manually entered by a user through the mobile application.

2. **weather_report_aemet.xml**
   - Based on meteorological OpenData from AEMET (Spanish Meteorological Agency),
     adapted to the structure of the application.

Both XML documents are validated using the same XML Schema.

---

## 3. XML Schema (XSD)

The file **weather_report_schema.xsd** defines the structure, data types, and
constraints for all XML documents used in the application.

The schema ensures:
- Correct element order
- Proper data types (dateTime, decimal, integer)
- Reusability for future XML documents

---

## 4. XML Validation Evidence

The XML documents were verified following two steps:

### Well-Formed XML
- Visual Studio Code was used to check that the XML documents are well-formed.
- No syntax errors or warnings are shown in the editor.

### XML Schema Validation
- The XML documents were validated against the XSD using an online XML validator.
- The validator confirms: **“The XML document is valid.”**

Screenshots demonstrating these validations are included in the `screenshot`
folder of this repository.

---

## 5. OpenData Source

One of the XML documents is based on public OpenData provided by:

- **AEMET – Agencia Estatal de Meteorología (Spain)**

The original OpenData was adapted to match the XML Schema while preserving
its original meaning and structure.

---

## 6. Tools and Websites Used

The following tools and resources were used in this project:

1. GitHub – repository hosting and version control
2. Visual Studio Code – XML and XSD editing
3. Node.js – RESTful API backend (reference)
4. Express.js – API framework (reference)
5. FreeFormatter XML Validator – XML/XSD validation
6. AEMET OpenData Portal – weather data source

---

## 7. General Impression

This project was developed as part of an academic assignment and meets all the
required objectives. It demonstrates the correct use of XML and XML Schema (XSD)
for data exchange, validation, and documentation.

The work follows the guidelines provided and includes all the elements required
for the submission of the task.

---

**Author:** Pablo Tapia
**Language:** English
