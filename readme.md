## Project Abstract

![project_diagram](/Users/JakeCannon/Desktop/spotify_project/images/project_diagram.png)A web application that adds functionality to Spotify. The idea for this app is to make a collaborative playlist between two people. The idea is not for it to be manually created but to create a Discover playlist between two users and their music interests. A *Discover* playlist, if you are not familiar, is a weekly or daily playlist, generated by Spotify prediction algorithms, of songs that you might like based on your previous listening history. This could be created without a web app of course, but, a web app could provide a user interface for non-technical users.

TLDR:  Curate a Spotify Discover playlist between two users.



## Project Relevance

This project could be relevant for the following reasons:

- Backend API design
- Object-oriented design for the backend and perhaps frontend
- Interacting with web APIS (such as the Spotify API)
- API will use JSON and perform some of the CRUD operations
- Unit testing
- Parallel computing by way of AWS or other cloud providers (If project was hosted)
- May need a Relational Database System (not sure yet)



## Conceptual Design

This is not an existing open source project so the group will just create the web app from scratch as an open-source program. The bulk of the design and work would be on creating a backend API to gather data from the Spotify API, run algorithms, then publish or display results. Being a web app there will need to be a frontend interface. However, I imagine we can get away with a pretty basic frontend. The end result is a genereated playlist that has *merged* two users interests. The frontend would primarily be an interface to map two users and trigger the backend API. Finally, being a web app, the team could use a cloud platform to host the app which creates all kinds of other problems/challenges.



## Background

**URL:** 



**Running:**

- Build your Flask image:

```
docker build -t 3308_spotify_project .
```

- Run a container based on your image:

```
docker run -d --name 3308_spotify_project -p 80:80 3308_spotify_project
```

- Navigate to localhost at

```
http://127.0.0.1/
```

- To shut down the container

```
docker container stop 3308_spotify_project
```

- To start a previously shut down container

```
docker start 3308_spotify_project
```



More detailed explantion [here](https://github.com/tiangolo/uwsgi-nginx-flask-docker)



## Required Resources

- ?



## Other Resources

Similar Spotify features/problems others have already sovled/worked on

- https://towardsdatascience.com/curating-a-spotify-discover-playlist-for-two-people-with-k-means-clustering-a926a9e1ec7d
- https://towardsdatascience.com/friendshipify-a-playlist-generator-for-friends-f79297f08b03



Creating ML API on AWS

- https://towardsdatascience.com/deploy-a-machine-learning-model-as-an-api-on-aws-43e92d08d05b
- https://medium.com/analytics-vidhya/build-and-deploy-an-machine-learning-model-using-aws-and-apis-1d22eadb2b83
- https://medium.com/datadriveninvestor/dockerize-and-deploy-your-machine-learning-application-on-aws-e2537bd3df21