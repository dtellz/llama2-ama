# Llama2 "AMA"
## What is this?

This is a basic chainlit web app to run Llama2 in CPU machines. Its knowledge is constraint to the pdf file you store in the data folder. It is a simple way to get started with Llama2. For this example I used "Cracking the coding interview" book.

## How to use it?

1. Clone the repo
2. Download the model from the link below and put it in the model folder at root level
[Llama2-7B-Quantized model](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/blob/main/llama-2-7b-chat.ggmlv3.q8_0.bin)
3. Install the requirements
    using pip:

    ```bash
    pip install -r requirements.txt
    ```

4. Get your knowledge source into data folder and run the following command:

    Depending on the size of your knowledge source, this might take a while.

    ```bash
    python ingest.py
    ```

    This will create a directory called vectorstores in the root folder. This is where the knowledge source is stored in a vectorized format.

5. Run the following command to start the web app:

    ```bash
    chainlit run model.py -w  
    ```

    This will start the web app on port 8000. You can access it at http://localhost:8000

6. Ask questions and enjoy!
