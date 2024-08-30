![image](https://github.com/user-attachments/assets/10013608-1d4c-412d-8b11-d2138cdd6d6e)


# Discord Activity

이 프로젝트는 디스코드에서 제공하는 문서를 바탕으로 개발되었습니다. [Building An Activity](https://discord.com/developers/docs/activities/building-an-activity) tutorial in the Discord Developer Docs.

Read more about building Discord Activities with the Embedded App SDK at [https://discord.com/developers/docs/activities/overview](https://discord.com/developers/docs/activities/overview).

## project files
 ```
├── client
│   ├── main.js       -> your Activity frontend
│   ├── index.html
│   ├── package.json
|   |── rocket.png
│   ├── vite.config.js
├── server
│   ├── package.json
│   ├── server.js     -> your Activity backend
└── .env              -> your credentials, ids and secrets
```

## Set Up Your Environment Variables
```
cp example.env .env
```

## Set Up Your Frontend
```
# from inside the root directory:

cd client
npm install
npm run dev
```

## Running your app locally in Discord
```
# from inside the root directory:

cd client
npm run dev

cloudflared tunnel --url http://localhost:5173
```

## Set up your Activity URL Mapping
