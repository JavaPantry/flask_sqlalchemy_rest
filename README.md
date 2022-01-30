# REST API With Flask & SQL Alchemy

> Products API using Python Flask, SQL Alchemy and Marshmallow

## Quick Start Using Conda local environment (Pipenv conflicting with conda)



``` bash
# deactivate default conda base environment
(base) $ conda deactivate
# create empty local environment
$ conda create --prefix ./envs

# activate local environment
$ conda activate ./envs

# install pip in local environment
(/env) $ conda install pip

# at this point VsCode ask to activate this virtual environment in current workspace

# install required dependencies
(/env) $ pip install flask flask-sqlalchemy flask-marshmallow marshmallow-sqlalchemy

(/env) $ python app.py


# Create DB
$ python
>> from app import db
>> db.create_all()
>> exit()

# Run Server (http://localhst:5000)
python app.py
```

## Endpoints
* GET     /test
* GET     /product
* GET     /product/:id
* POST    /product
* PUT     /product/:id
* DELETE  /product/:id