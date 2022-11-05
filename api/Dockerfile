FROM python:3.9

## Step 1:
# Create a working directory

WORKDIR /app

## Step 2:
# Copy Install packages from requirements.txt

COPY requirements.txt ./

RUN sudo apt install python-dev
RUN pip install -r requirements.txt

## Step 3:
# Copy source code to working directory

COPY ./ ./

## Step 4:
# Run app.py at container launch

CMD ["python", "manage.py", "runserver"]

