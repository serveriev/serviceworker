# Test Firebase Cloud Messaging

You can test usage on page: https://github.com/serveriev/serviceworker

<img src="ScreenRecord.gif" alt="" align="center">

## Send notification from HTTP client

```
POST /fcm/send HTTP/1.1
Host: fcm.googleapis.com
Authorization: key=fedHQRTvKG4:APA91bG9sBM2fFT4uO8ln-N57V9hx5EU74tEUpsCMZ-vuoE3EVi3c-Vv7JELJroM5BcY2wa_KPH6oIgncW1ulkyfwiiGIR1CSAJbYJMX4DGwYUZtGIGjNIQBdOAlEtl9KaMZFHyINQP3
Content-Type: application/json

{
  "notification": {
    "title": "Bubble Nebula",
    "body": "It's found today at 21:00",
    "icon": "https://serveriev.github.io/serviceworker/Bubble-Nebula.jpg",
    "click_action": "https://www.nasa.gov/feature/goddard/2016/hubble-sees-a-star-inflating-a-giant-bubble"
  },
  "to": "YOUR-TOKEN-ID"
}
```
