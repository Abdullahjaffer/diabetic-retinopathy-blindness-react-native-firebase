# Built with React Native, Expo and Firebase

create `.env` to get started

looks like

```
API_KEY=
AUTH_DOMAIN=diabetic-retinopathy-blindness.firebaseapp.com
PROJECT_ID=diabetic-retinopathy-blindness
STORAGE_BUCKET=diabetic-retinopathy-blindness.appspot.com
MESSAGING_SENDER_ID=
APP_ID=
DATABASE_URL=https://diabetic-retinopathy-blindness.firebaseio.com
```

uses signed s3 url to upload images
config in `config/server.js`

### Custom server interaction

1. get_signed_url_path to get s3 signed url,
2. upload to signed url
3. post to get_results with image name returned when getting signed url

done in `screens/uploadscreen.js`
