# MoodBot
Sample bot to showcase the use of fetching data from MySQL db into the bot developed using Rasa.

[dbConnect.py](https://github.com/JiteshGaikwad/MoodBot/blob/master/dbConnect.py) file contains the code for:
- setup the database connection
- setup the cursor to execute the sql query
- return the all the rows fetched from the database

**Step1**: Install the `mysql-connector` using the below command:

> python -m pip install mysql-connector

**Step2**: Add the [`dbConnect.py`](https://github.com/JiteshGaikwad/MoodBot/blob/master/dbConnect.py) file in your project directory as shown above

**Step3**: Import `getData` method from `dbConnect` module into your `actions.py` file:
> from dbConnect import getData

**Step4**: pass your sql query to the `getData()` method:
> getData("select * from customer")
