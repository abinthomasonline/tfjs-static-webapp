# Finetune Mobilenet for Tensorflow.js WebApp

This is a simple example of how to finetune a Mobilenet model and use it in a web application using Tensorflow.js. The web application will allow you to upload a picture and classify it using the finetuned model.


## Demo

You can try the web application [here](https://abinthomas.in/mobilenet-tf/) (Hosted on github-pages).
[![WebApp Demo](demo.gif)](https://abinthomas.in/mobilenet-tf/)

## Installation

First, clone the repository and install the required packages:

```bash
git clone https://github.com/abinthomasonline/mobilenet-tf.git
cd finetune-mobilenet-tfjs
pip install -r requirements.txt
```

The code is tested with Python 3.11.7 in OSX.

## Kaggle Authentication for Dataset

To download the dataset, you need to have a Kaggle account and a Kaggle API key. You can create a new API key from your Kaggle account settings. Once you have the API key, create a new file `kaggle.json` in the secrets directory of the project and add the API key to the file as shown below:

```json
{
  "username": "your-kaggle-username",
  "key": "your-kaggle-api-key"
}
```

## Finetune Mobilenet

To finetune the Mobilenet model, run the `main.ipynb` notebook. The notebook will download the dataset, finetune the model, save the model in the `runs` directory, and convert the model to a Tensorflow.js model.

## Run the Web Application

To run the web application, run the following command:

```bash
cd webapp
python -m http.server
```
Open your browser and go to `http://localhost:8000` to use the web application.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
