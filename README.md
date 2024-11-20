docker-compose up --build
./es_schema.sh

python3.10 -m venv venv
./venv/bin/pip install elasticsearch flask

./venv/bin/python3 film_loader.py 

./venv/bin/python3 app.py 
