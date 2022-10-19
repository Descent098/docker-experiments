FROM nogil/python

COPY requirements.txt requirements.txt
RUN python3 -m pip install -r requirements.txt

COPY . .

CMD [ "python3", "routes.py"]