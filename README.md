# pydata-pi-approx
#### Web-based Analysis &amp; Simulation Platforms with React/Redux, Flask, Celery, and Numpy
 
This project is based on a tutorial from a talk given by James Powell during a Pydata event.
[Here is the video](https://youtu.be/eEXKIp8h0T0)

### Install using conda
```
conda create -n jsim -c conda-forge bokeh sympy flask redis redis-py celery nodejs=11.14 python=3.6
pip install httpie flask-cors
```

### Note to myself:
- run gulp:
```bash
$ cd frontend
$ node_modules/.bin/gulp watch
```

- run celery worker:
```bash
$ celery -A worker worker 
```

- run restapi server:
```bash
$ cd backend
$ pipenv run python restapi.py
```

- run website server:
```bash
$ python httpserver.py static/
```

### Todo:
- Add graphic representation using bokeh
