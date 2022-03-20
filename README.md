# AIDI2004-Lab4

## About

This is a project to show my working knowledge of how to deploy a machine learning model to Heroku using flask so that users can query the model through a front-end built in HTML and CSS. A classification model was built in order to predict the species of a fish based on certain features of the fish. The model can be queried at the following Heroku webpage: https://fish-predict-species.herokuapp.com/

## Project components

* The css file for the project is located in the folder ```static/css```.
* The HTML file for the project is located in the folder ```templates```.
* AIDI2004_Lab_4.ipynb is the Jupyter notebook that contains the code for building the classification model. This file is not needed for the project unless you wish to make changes to the model that is being used.
* Fish.csv is the dataset that the model was trained and tested on. This dataset is not required to run the project, but is required if you wish the make changes to the existing model.
* FlaskApp.py contains the flask code for the project.
* Procfile contains the commands that are to be executed by the project on startup. This file is necessary if you are deploying the project to Heroku, but is not needed if the project is running locally.
* model.pkl is the classification model being used in the project.
* requirements.txt contains a list of all the libraries that the project uses with the exact versions that were being used when the project was built.

## Dependencies

This project runs on ```python```, so that needs to be installed.

All the pre-requisite packages required for the project are listed in ```requirements.txt```. Most of these packages are pre-requisites for deploying to Heroku, which Heroku will handle on its own. To deploy the project locally, the following libraries need to installed:


*   pandas
*   sklearn
*   pickle
*   numpy
*   flask

To install these libraries, first ensure that you have ```pip``` installed on your machine. These can be installed using the following pip command through your CLI:


```
pip install <PACKAGE_NAME>
```

It is a good idea to run this command for the libraries listed above even if you already have them just to ensure that you're running on the latest version of the libraries so that there is no room for error. 

Alternatively, if you're too lazy to run the commands one-by-one for the list of libraries above, you can also use the following command:

```
pip install -r requirements.txt
```

This will install all the libraries inside requirements.txt with the exact version that was used in my implementation. 

**Note:** *This alternative method will also install all the libraries that were used by Heroku but were not needed for local deployment.*


## How to Use

### Online

The fish species classifier can be found at https://fish-predict-species.herokuapp.com/

### Locally

Clone/download this repository. In your CLI, go to the local directory where the files are located using the ```cd``` command. Then, enter the following command:

```python FlaskApp.py```

The project can then be viewed using any web browser such as chrome at the following address:

```http://127.0.0.1:5000/```


## Credits

This project was done under the guidance of prof. Noopa Jagadeesh. The majority of the code was provided by them.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.

## How to contribute

To contribute to this project, contact me at jaspreetsm123@gmail.com.
