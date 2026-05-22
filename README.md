# So when you go to test things for each task:

## Task 0 -
`docker build -f ./Dockerfile -t softy-pinko:task0 .
docker run -it --rm --name softy-pinko-task0 softy-pinko:task0`

## Task 1 -
`docker build -f ./Dockerfile -t softy-pinko:task1 .
docker run -p 5252:5252 -it --rm --name softy-pinko-task1 softy-pinko:task1`

## Task 2 -
`docker build -f ./front-end/Dockerfile -t softy-pinko-front-end:task2 ./front-end
docker run -p 9000:9000 -it --rm --name softy-pinko-front-end-task2 softy-pinko-front-end:task2`

(Go open the localhost page on localhost:9000 and see that it should work)

## Task 3 -
terminal 1
`docker build -f ./back-end/Dockerfile -t softy-pinko-back-end:task3 ./back-end
docker run -p 5252:5252 -it --rm --name softy-pinko-back-end-task3 softy-pinko-back-end:task3`

terminal 2
`docker build -f ./front-end/Dockerfile -t softy-pinko-front-end:task3 ./front-end
docker run -p 9000:9000 -it --rm --name softy-pinko-front-end-task3 softy-pinko-front-end:task3`

(go open the localhost page again on the same localhost address as before and notice how it interacts with both the front and back ends in the CLI)

## Task 4 -
`docker compose build`
`docker compose up`

One builds, one runs. Website works like a charm

## Task 5 -
`docker compose build
docker compose up`

Then visit http://localhost:80 now instead of localhost:8000

## Task 6 -
`copypaste the line of code in 2-api-servers.txt then do
docker compose up`

visit the webpage, and refresh the page multiple times
NOTE: I originally had it as backend and frontend in the previous questions but for the brief i've fixed it so it matches the brief here.
