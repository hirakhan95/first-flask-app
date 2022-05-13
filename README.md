# First Flask Application

This is my first flask application. Please use it wisely.

### Features

Features are following
- Login
- Logout
- Edit email

```Python
## To register sql db to Flask app
app = Flask(__name__)
app.secret_key = "hello"
app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///users.sqlite3'
app.config['SQLALCHEMY_TRACK_MODIFICATIONS']= False
app.permanent_session_lifetime = timedelta(minutes=5)

db = SQLAlchemy(app)
```
