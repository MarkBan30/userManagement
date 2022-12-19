# How to use
Prepare venv under work directory
```bash
python3 -m venv venv
```

Activate the interpretor in project
```bash 
source venv/bin/activate
```

Install dependencies from pypi
```bash 
pip install -r requirements.txt
```

Start mongo db docker container
```bash 
docker run -d -p 30001:27017 -v /your_host_machine_dir:/data/db --hostname ztgg_mongo  --name=ztgg_mongo mongo
```


Run flask app
```bash
source startup.env
flask run
```

Each time you get in project VS code(IDE), need to pull the latest code, activate venv and app_env, install the latest dependencies added by peer
```bash
git pull
source venv/bin/activate
pip install -r requirements.txt
source startup.env
flask run
```
