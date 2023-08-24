# Llama2 "AMA"
## What is this?

This is a basic web app to create chatbots that can be fed with your desired knowledge source to answer questions.

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