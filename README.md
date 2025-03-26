# 🚀 Hacktivists - Smarter Reconciliation And Anomaly Detection Using Gen AI

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

🔗 [Live Demo](#) Video demo is present in the demo folder under arifacts folder.
📹 [Video Demo](#)Video demo is present in the demo folder under arifacts folder.
🖼️ Screenshots:

![Screenshot 1](link-to-image)

## 💡 Inspiration

Anomaly detection is very critical as far as banking sectors are concerned. When some fund is transferred from a source account to a target account, anomaly detection is very much neessary in order to come up with a smart reconciliation process. The criticality of the problem statement has inspired me to come up with a smart reconciliation process using Gen AI.

## ⚙️ What It Does

Our project takes two excel files as input. One excel file is for the real time data and another excel file is related to the historical data. Then it finds out the balance differences between the 2 source systems and accordingly, comes up with the match status 'Match' or 'Break'. In case of breaks, our solution checks the historical data in order to find out the anomalies for different combinations of scenarios. After detecting the anomalies, it takes help of the respective LLM(large Language Model) to get the comments or corrective actions for the abnormal breaks i.e. the anomalies and also for the normal breaks. For interacting with the LLM, our solution uses well crafted prompt in order to ensure consistent desired response from the LLM.

## 🛠️ How We Built It

We have proposed 2 approaches here.
For the first approach, we have created a web app through which we are uploading two excel files for real time data and historical data. When the 2 excel files are uploaded, one endpoint gets triggered and this endpoint is responsible for performing all the necessary operations to determine anomalies and comments. In return, the endpoint returns one resposne json based on which the results get displayed in a tabular format in UI.
For the second approach, we can run one python script which takes 2 excel files for the real time data and historical data and generates one output file which contains all the necessary derived columns like Balance Difference, Match Status, Anomaly and Comments.

For both the approaches mentioned above, we have ceated an Agentic AI which is responsible for running a workflow using Langgraph framework.

The following technologies and frameworks have been used for the approaches mentioned above.

- 🔹 Frontend: React
- 🔹 Backend: Python / FastAPI
- 🔹 LLM Framework: Langgraph
- 🔹 Other Library: Pandas / Material UI

## 🚧 Challenges We Faced

The challenges that we faced during the development are mentioned below.

- 🔹Determining the different combination of patterns in the dataset.
- 🔹Constructing the prompt to get the uniform desired response from the respective LLM based on the category of break and anomaly.
- 🔹Implementation of Agentic AI using Langgraph for the solution.

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
