# pydata-pi-approx
#### Web-based Analysis &amp; Simulation Platforms with React/Redux, Flask, Celery, and Numpy
 
This project is based on a tutorial from a talk given by James Powell during a Pydata event.
[Here is the video](https://youtu.be/eEXKIp8h0T0) and [here](https://www.dropbox.com/sh/yus0uz132xeb7cs/AACw9MuHD6VZ0wMPtPrnvK1Ya?dl=0) is the original code location

### Install using conda
```
conda create -n jsim -c conda-forge bokeh sympy flask redis redis-py celery nodejs=11.14 python=3.6
pip install httpie flask-cors
```

Refer [here](https://stackoverflow.com/questions/55483235/redis-installation-using-conda-not-working-modulenotfounderror-no-module-named) to know why redis-py is required.



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
