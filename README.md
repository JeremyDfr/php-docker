# PHP docker environment
## Running
- Create a `.env` file based on `.env.example` file.
- Build the environment image with the following command:
```
docker compose build app
```
- When the build is finished, you can run the environment in background mode with:
```
docker compose up -d
```
Now you can go to your browser at `http://localhost:8000` or if the environnement running to a server, use `http://server_domain_or_ip:8000`

## More informations
- You can use this following command to execute command into the container:
```
docker compose exec app composer
```
- To stop the entire service use this command:
```
docker compose stop