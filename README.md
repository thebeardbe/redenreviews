# Reden Reviews

This is the source code for the Reden.reviews platform that will serve as a gui for the reviews that will be saved on the blockchain of [Redencoin](https://reden.reviews) of which the source code can be found on the [Redencore github](https://github.com/RedenCore/Reden)

This project gets live developed on my [twitch.tv stream](https://twitch.tv/thebeardbe). 

The goal of the project is to have users submit reviews, get them processed and uploaded to the blockchain that will serve as the ultimate database. 
The frontend will be use a local database that will get synced on fixed intervals with the blockchain, where the blockchain will always be correct version and overwrite the existing low latency local database. Similar in a way that an explorer for a blockchain works.

The submissions of reviews will be uploaded in a transaction on the blockchain. (TBD how to achieve this reliably)

## Stage 1 

Have a form that will accept only review requests, it will ask for some general info on the project, including but not limited to algorithm, type, links, ....

In a first stage this data will be saved in a local database and shown on the website as a project with some specs, I will select from this list to review on the twitch streams and update the website manually.

## Stage 2

On the projects specification page there will be a link to submit a complete review, there can be multiple reviews per project. Every review gets saved individually and will be shown seperatly on the website. 

Every projects page will have a overview that links to all the reviews done by users and it will have an overview with a score for every category, that is calculated from the average of the different reviews.

## Stage 3

Users can now rate via a point system the project and every review done individually, this score gets averaged out also shown to give an extra indication of the project fidelity. 

## Stage 4

Every project and it's specs get pushed into the blockchain and every review gets also saved in the blockchain with a link to the original blockchain. 
Voting on projects will require a limited amount of reden to be send to the reden address linked to the project. The proceeds from these votes get distributed among the reviewers.

## Stage 5

Projects can ask for a quicker review that will be done by one of our internal staff and there will be a fee for skipping the line. This fee will be also be distributed among all reviewers that have a certain average score per review given by users of the platform. 
To consult detailed reviews will require also a small reden fee to be sent to the projects address that again will be distributed among the reviewers that reviewed the project.
All this can be done through the website frontend in a very easy way. There will also be a link to a payment system that permits to buy reden on an exchange (TBD) 

# Language

The project will be coded in node.js, that way the project can be hosted locally and completely transparent to the user once the system is getting it's data from the blockchain and no longer from the local database. 

It will be distributed to an easy install package for linux, windows and mac.

