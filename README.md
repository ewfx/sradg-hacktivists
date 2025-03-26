# 🚀 Project Name

## 📌 Table of Contents

- [Introduction](#introduction)
- [Demo](#demo)
- [Inspiration](#inspiration)
- [What It Does](#what-it-does)
- [How We Built It](#how-we-built-it)
- [Challenges We Faced](#challenges-we-faced)
- [How to Run](#how-to-run)
- [Tech Stack](#tech-stack)
- [Team](#team)

---

## 🎯 Introduction

The objective of this project is to compare 2 data sources and historical data and based on the comparison, the project is responsible for detecting anomalies and generating comments or corrective actions after interacting with the respective Large Language Model(LLM).

## 🎥 Demo

🔗 [Live Demo](#) (if applicable)  
📹 [Video Demo](#) (if applicable)  
🖼️ Screenshots:

![Screenshot 1](link-to-image)

## 💡 Inspiration

What inspired you to create this project? Describe the problem you're solving.

## ⚙️ What It Does

Explain the key features and functionalities of your project.

## 🛠️ How We Built It

Briefly outline the technologies, frameworks, and tools used in development.

## 🚧 Challenges We Faced

Describe the major technical or non-technical challenges your team encountered.

## 🏃 How to Run

# Steps for running the standalone python script

1. Pull the codebase from the main branch of the following github repository.
   ```sh
   git clone -b main -c core.longapths=true https://github.com/ewfx/sradg-hacktivists.git
   ```
2. Install python in the local system.
3. Install anaconda in the local system.
4. Open anaconda prompt.
5. Navigate to the project folder in the conda prompt window.
6. Create a virtual environment using the following conda command.
   ```sh
   conda create -p "<Path Of the Virtual Environment>" python="<Version Of Python>" -y
   ```
7. Check the environment list by using the following conda command.
   ```sh
   conda env list
   ```
8. Copy the desired environment path from the list and then activate the virtual environment by using the following conda command.
   ```sh
   conda activate "<Path Of the Virtual Environment>"
   ```
9. Install the necessary python libraries by running the following comand in the conda prompt window.
   ```sh
   pip install -r requirements.txt
   ```
10. Create a GROQ account by navigating to the following URL.

```sh
https://consol.groq.com
```

11. Create a GROQ API key.
12. Create .env file under the project folder and set the GROQ API key in .env file like the following.
    ```sh
    GROQ_API_KEY="<GROQ API KEY>"
    ```
13. Install Visual Studio Code in the local system.
14. Open Visual Studio Code IDE and navigate to the project folder.
15. Place the excel files for both real time data and historical data in some path.
16. Open the python file "Anomaly_Detection_Workflow.py"
17. Change the file path for real time data at line no 17
18. Change the file path for historical data at line no 18
19. Change the target file path at line no 120.
20. Run the python script using the following command.
    ```sh
    python -m Anomaly_Detection_Workflow.py
    ```

# Steps for running the Web Application

1. Pull the codebase from the main branch of the following github repository.
   ```sh
   git clone -b main -c core.longapths=true https://github.com/ewfx/sradg-hacktivists.git
   ```
2. Install python in the local system.
3. Install anaconda in the local system.
4. Open anaconda prompt.
5. Navigate to the project folder in the conda prompt window.
6. Create a virtual environment using the following conda command.
   ```sh
   conda create -p "<Path Of the Virtual Environment>" python="<Version Of Python>" -y
   ```
7. Check the environment list by using the following conda command.
   ```sh
   conda env list
   ```
8. Copy the desired environment path from the list and then activate the virtual environment by using the following conda command.
   ```sh
   conda activate "<Path Of the Virtual Environment>"
   ```
9. Install the necessary python libraries by running the following comand in the conda prompt window.
   ```sh
   pip install -r requirements.txt
   ```
10. Create a GROQ account by navigating to the following URL.

```sh
https://consol.groq.com
```

11. Create a GROQ API key.
12. Install Visual Studio Code in the local system.
13. Open Visual Studio Code IDE and navigate to the project folder.
14. Open anomaly_detection_service.py file and set the GROQ API KEY at line no 7
15. To run the backend server use the following command in the conda prompt window.
    ```sh
    fastapi dev code/src/
    ```
16. Install nodejs.
17. Open the frontend codebase in Visual Studio Code IDE
18. Open the terminal and run the following command.
    ```sh
    npm install
    ```
19. Run the frontend code using the following command.
    ```sh
    npm run start
    ```
20. Test the functionality using the following local URL.
    ```sh
    http://localhost:3000
    ```

## 🏗️ Tech Stack

- 🔹 Frontend: React
- 🔹 Backend: Python / FastAPI
- 🔹 LLM Framework: Langgraph
- 🔹 Other Library: Pandas / Material UI

## 👥 Team

- **Arnab Nath** - [GitHub](#) | [LinkedIn](#)
- **Manish Gupta** - [GitHub](#) | [LinkedIn](#)
- **Harsha V. Thummalapenta** - [GitHub](#) | [LinkedIn](#)
- **Uday Kumar Narayana** - [GitHub](#) | [LinkedIn](#)
- **Jamili Chakradhari** - [GitHub](#) | [LinkedIn](#)
