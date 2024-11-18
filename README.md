# cintel-04-local

This project assumes you have cloned this repo down to your mechine and created and activated a virtual enviornment 

## Activate the app in your browser
in a terminal with your .venv active, run the following line of code:

```
shiny run --reload --launch-browser penguins/app.py
```

## Open a new terminal
while the app is running in your browser, the terminal you used to open it will be occupied. To continue making changes, open a new terminal.

## Building the app to the docs folder and testing it locally
With your project virtual environment active in the terminal and the necessary packages installed into our .venv project virtual environment, remove any existing assets and use
shinylive export to build the app in the penguins folder to the docs folder:
```
shiny static-assets remove
shinylive export penguins docs
```
## serve the app locally from the docs folder
run the following command from the root of the project folder with the project virtual environment active:
```
python -m http.server --directory docs --bind localhost 8008
```

