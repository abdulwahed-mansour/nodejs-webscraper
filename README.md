# NodeJS Webscraper
Demo for showing how to scrape data and get backend data to the frontend. This repository is for the video tutorial [here](https://youtu.be/-3lqUHeZs_0)


## To run this project

You can run this project on your local machine. Just pull it down and do the following:

### `npm i`

### `npm i nodemon`


1. Run the command above to install all the packages

### Start the Project

2. Now run the server:

```bash
npm run start
```

3. Open [http://localhost:8001/results](http://localhost:8001/results) with your browser to see the results of the scrape in your terminal.

4. Finally, open the index.html file in your browser to see the results showing up.

### https://www.youtube.com/watch?v=3xDAU5cvi5E

## Build docker image

```bash
docker build .
```

#### Delete no name image ... last image

```bash
docker image rm 879hrr3457kkia423
```

#### Create New One with name react-image

```bash
docker build -t react-image .

```

#### Create first container

```bash
docker run -d --name react-app react-image
```

#### docker containers

```bash
docker ps
```

#### Kill last container
```bash
docker rm react-app -f
```

#### important with PORT 3000

```bash
docker run -d p 3000:3000 --name react-app react-image

```
## Mounting a docker volume for powershell windows
### Mount current directory as a volume in Docker on Windows 10

##### In Windows Command Line (cmd), you can mount the current directory like so:

```bash
docker run -e CHOKIDAR_USEPOLLING=true -v %cd%\src:/app/src -d p 3000:3000 --name react-app react-imag

```

##### In PowerShell, you use ${PWD}, which gives you the current directory:

```bash
docker run -e CHOKIDAR_USEPOLLING=true -v ${PWD}/src/:/app/src -d p 3000:3000 --name react-app react-image
```
##### On Linux:

```bash
docker run -e CHOKIDAR_USEPOLLING=true -v $(pwd)/src:/app/src -d p 3000:3000 --name react-app react-image

```


```bash
testiIIIIIIIIII
```
