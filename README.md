# event_management
# Django REST API - Event Management  

# Clone the repository

git clone https://github.com/yourusername/event-management.git
cd event-management
  

# Create a virtual environment  
 python3 -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate  

# Install dependencies  
$ pip install -r requirements.txt  

# Optional commands, Because execute with docker 

## Apply database migrations 
$ python3 manage.py migrate  

## Create a superuser 
$ python3 manage.py createsuperuser  

## Run the development server
$ python3 manage.py runserver  



# Testing API endpoints : 

# Authentication after registered user

- POST : http://127.0.0.1:8000/api/token/	

Payload:  
```json
{
  "username": "your_username",
  "password": "your_password"
}
```

# Running with Docker :

## Build and start containers
docker-compose up --build
##### OR
docker-compose build --no-cache 

docker-compose up

## Run migrations inside Docker container
docker-compose exec web python manage.py migrate

## Create superuser inside Docker container (optional)
docker-compose exec web python manage.py createsuperuser
# event_management
# event_management
