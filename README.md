# Docker Flask-app
- Simple Docker flask app testing.

# How to Run 
```bash
# Step:1 Build Images
- docker build -t flask-app .

# Step2: Create Container
- docker run --name flask-docker -p 80:80 flask-app

```

# 🧠Important
```bash
# If your Flask app runs on:
-  app.run(host="0.0.0.0", port=5000)

# Then you must map correctly:
-  docker run -d -p 80:5000 flask-app
-  Because container port is 5000

```

# After Completing All the Steps Open below URL In browser
- http://localhost
- http://localhost/health
