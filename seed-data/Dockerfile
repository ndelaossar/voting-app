FROM python:3.9-alpine

WORKDIR /seed

COPY . .

# create POST data files with ab friendly formats
RUN python make-data.py

CMD /seed/generate-votes.sh