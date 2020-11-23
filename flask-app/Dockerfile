#Use Python Image
FROM python:3.7

# Install apt dependencies
RUN apt update
RUN apt install python3-pip -y
 
# run pip dependencies
RUN pip install flask
RUN pip install flask_sqlalchemy
RUN pip install pymysql

#Copy neccecery files
COPY . .
 
# Expose correct port
EXPOSE 80

# Create an entrypoint
ENTRYPOINT ["python", "app.py"]
