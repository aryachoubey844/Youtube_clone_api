# Flask Video REST API

Simple REST API using Flask, Flask-RESTful and SQLAlchemy.

## Endpoints

| Method | URL | Body | Description |
|--------|-----|------|-------------|
| GET | /video/<id> | None | Get video by id |
| PUT | /video/<id> | {"name","views","likes"} | Create new video |
| PATCH | /video/<id> | {"name"/"views"/"likes"} | Update video (partial) |
| DELETE | /video/<id> | None | Delete video |

## Setup
pip install -r requirements.txt
python main.py

Server runs at http://127.0.0.1:5000

## Test with Postman
PUT http://127.0.0.1:5000/video/1
Body raw JSON:
{
  "name": "My Video",
  "views": 100,
  "likes": 10
}