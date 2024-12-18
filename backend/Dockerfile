FROM python:latest

RUN apt update && apt -y upgrade && apt install -y \
    python3 \
    python3-pip
    
RUN pip install django \
    chmod +x ./backend/manage.py

EXPOSE 8000

ENTRYPOINT ["python3"]
CMD ["./manage.py", "runserver", "0.0.0.0:8000"]