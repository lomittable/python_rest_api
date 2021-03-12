## Build Python REST API

Getting Started:
1. Download XCode from the Macbook Appstore
2. Download PyCharm IDE Community Mac Edition (.dmg Intel): [here](https://www.jetbrains.com/pycharm/download/#section=mac)
3. Wherever you want to house your code, create a folder (you can make one under Desktop or Documents called "python_code")
4. In "python_code" folder, add another folder called something like "my_first_python_app"
5. Open PyCharm & create a new project
6. For "Location" set the folder you created ("my_first_python_app") & leave other settings as is
7. You now have a runnable project with its own virtual environment. The starting point or top level of your app lives in main.py which orchestrates how your code is run
8. click the little green triangle next to the main method and select Run 'main' -> you'll see the output in your terminal

In IDE terminal (near bottom of window):
1. run `pip install flask`
2. run `pip install flask_restful`
3. run `pip install pandas`
4. create your initialization file with `touch __init__.py` -> after you'll see it in your project
5. run `touch user_api.py`
6. open your user_api.py file & copy the code from my file in [my GitHub repo](https://github.com/lomittable/python_rest_api)
7. Also copy the users.csv file into your "my_first_python_app" folder: this will act as our database (easier setup than a SQL/MongoDB/Cassandra or whatever is popular these days)

Run your app
1. select Run 'main'
2. you'll see the following in your terminal: `Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)`

Open POSTMAN
1. Download Postman: [here](https://www.postman.com/downloads/)
2. Do a GET at endpoint `http://127.0.0.1:5000/users`
3. You'll see the data from your users.csv in JSON format 

Voila! Your first API
