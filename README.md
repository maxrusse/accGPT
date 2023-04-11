# AI Chatbots for Imaging Recommendations Aligned with ACR Guidelines

### This project demonstrates the use of AI chatbots to provide imaging recommendations aligned with ACR (American College of Radiology) guidelines. It combines the outputs of different AI models to generate more precise and reliable recommendations.

### You can directly use the Jupyter notebook file provided in the project. The notebook contains all the necessary code and comments to help you understand and execute the project.



### To get started with the Jupyter notebook:

1. Download the notebook file Demo of all Chatbots.ipynb 
2. Upload the notebook to Google Colab, JupyterLab, or your preferred Jupyter notebook environment.
3. Install the required dependencies by running the cells containing the !pip install commands.
4. Set your OpenAI API key and the folder path containing the ACR guidelines in the corresponding cells.
5. Run the cells in the notebook to set up the index, launch the interface, and interact with the AI chatbots.

By using the Jupyter notebook, you can easily modify, extend, or experiment with the code as needed.


### How It Works
The script uses a combination of AI models to generate imaging recommendations based on the provided case information:

accGPT: Queries an index created from ACR guidelines and gets the response from the top 3 text nodes using GPT-3.5-Turbo.
GPT-3.5-Turbo: Provides a response based on the GPT-3.5-Turbo model.
GPT-4: Provides a response based on the GPT-4 model.
The responses from all models are combined and displayed in the interface.


### Screenshot of the Chatbot user interface with example case

![Screenshot of the Chatbot user interface with example case](https://github.com/maxrusse/accGPT/blob/b11a3c9f3d652187d74181afa4758ad6497234a4/example.jpg)



### Alternative using the python script by cloning the project:

Dependencies
To set up the project, you need to install the following dependencies:

```
pip install requirements.txt
```

Setup
Obtain an OpenAI API key from https://platform.openai.com/account/api-keys and set the OPENAI_API_KEY environment variable in the script.
```
os.environ["OPENAI_API_KEY"] = 'your_api_key_here'
```
Set the folder path containing the ACR guidelines in PDF format:
```
FOLDER_PATH = "ACR"
```

Run the script to set up the index and launch the interface.
```
if __name__ == "__main__":
    main()
```



