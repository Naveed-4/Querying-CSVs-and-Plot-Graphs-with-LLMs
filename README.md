# Querying-CSVs-and-Plot-Graphs-with-LLMs
This app was developed as part of an assignment using LangChain and the Gemini 1.5 Flash model. Right now, it's running on the free version of the Gemini API. Upgrading to a more advanced model can improve the quality of responses from the language model and provide even better insights.

This Streamlit application allows users to upload CSV files, perform data analysis, and generate insights using AI-powered language models.

### Solution Approach
For detailed information about the solution approach, refer to the [SOLUTION_APPROACH.md](SOLUTION_APPROACH.md) file.

### Working Video
The video passed multiple times to wait for free API to reset as it was getting exhausted. You get idea how it works. It will work more better if used with paid advanced llms.
Checkout the video here:
On Github a low quality one as size limit is 25mb, here [Working_SD_Video.mp4](Working_SD_Video.mp4) file.
On Google Drive a high quality video, here [Working_HD_Video](https://drive.google.com/file/d/1VfM7D53ZQuGkCYYVMspzNH-77cPM2Nn4/view?usp=sharing) file.

### Features:
1. CSV file upload and preprocessing
2. Data summary and statistical analysis
3. AI-generated insights and visualizations
4. Custom visualization creation
5. Interactive Q&A with the dataset

### Requirements:
- Python 3.8+
- Streamlit
- Pandas
- Matplotlib
- Seaborn
- LangChain
- Google Generative AI

### Installation:
1. Clone this repository:
    ```bash
    git clone https://github.com/Naveed-4/Querying-CSVs-and-Plot-Graphs-with-LLMs
    cd Querying-CSVs-and-Plot-Graphs-with-LLMs
    ```

2. Create a virtual environment (optional but recommended):

    - **On macOS/Linux**:
        ```bash
        python -m venv venv
        source venv/bin/activate
        ```

    - **On Windows**:
        ```bash
        python -m venv venv
        venv\Scripts\activate
        ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your Google API key:
- Obtain a Google API key from the Google Cloud Console
- Set the environment variable:

    - **On macOS/Linux**:
        ```bash
        export GOOGLE_API_KEY=your_api_key_here
        ```

    - **On Windows**:
        ```bash
        set GOOGLE_API_KEY=your_api_key_here
        ```
5. **Only if uploading a csv encounters an error**
   In the working directory, create a folder .streamlit. In that folder create a file named config.toml and paste below config:
   ```bash
   [server]
   enableXsrfProtection = false
   ```
   Make sure .streamlit folder and app.py are in same directory. This will fix the file upload error

### Usage:
1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Open your web browser and go to the URL displayed in the terminal (usually http://localhost:8501)

3. Upload a CSV file using the file uploader in the sidebar

4. Explore the different tabs:
- Data Summary and Statistical Analysis
- Auto-generated Insights
- Custom Visualization
- Data Q&A

5. Interact with the visualizations and ask questions about your data

### Note:
This application uses the Gemini 1.5 Flash model from Google's Generative AI. The free version of the API is currently in use, which may limit the quality and speed of responses. For better performance, consider upgrading to a paid plan or a more advanced model.

### Contributing:
Contributions, issues, and feature requests are welcome. Feel free to check the issues page if you want to contribute.

### License:
This project is licensed under the MIT License.
