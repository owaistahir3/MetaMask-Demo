Note: 

Sorry forgot to add balance display feature but it can be easily added through following command:

web3.eth.getBalance


#### Launch the demo using Docker Compose:

```bash
docker-compose up -d
```

This will leave a the bakcend listening on `localhost:8000` and the frontend on `localhost:3000`.

#### Launching the demo using Docker:

Build and launch the backend:

```bash
cd backend
docker build -t login-backend .
docker run -d -p 8000:8000 login-backend
```

Build and launch the frontend:

```bash
cd frontend
docker build -t login-front .
docker run -d -p 3000:3000 login-frontend
```

You can then access the app on `localhost:3000`.

#### Start the demo using Yarn:

From the root folder of this repo, run

```bash
yarn install # Install the dependencies
yarn start # Will launch the frontend and the backend at the same time
```

The backend should be running on `localhost:8000`, and the frontend on `localhost:3000`.
