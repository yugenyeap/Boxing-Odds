# Boxing-Odds
A NodeJS web application. A mashup of the BoxRec and Odds API

This project is one of favourite node.js projects I have created at university. As I am a huge boxing fan I created a node application which queries a sports betting odds API and the BoxRec API (The official record keeper for every professional boxer's profile).

The two API's that were used:
* OddsAPI - app.oddsapi.io
* BoxRec - https://www.npmjs.com/package/boxrec

The following tools were used:
* NPM
* Javascript
* HTML/Pug
* Bootstrap/CSS
* Docker

## User Guide:
After cloning this repository, the application can be run using npm or docker:

NPM:
1. Install the dependencies:
```bash
npm init
```
2. Run the npm server:
```bash
npm start
```
3. Navigate to localhost:3000 in a web browser

Docker:
1. Build the Dockerfile:
```bash
docker build -t boxing-odds .
```
2. Start the project:
```bash
docker run -p 80:3000 boxing-odds
```
3. Navigate to locahost in a web browser

The docker project is available on my private repository on dockerhub. It can be pulled from that repository using the following command:
```bash
docker pull yigeronni/boxing_odds:boxing-odds
```

# Screenshots of Usage:
Unfortunately due to COVID-19 shutting down most sporting events around the world, there are no major upcoming boxing matches (as of April 2020). Therefore the page will display nothing as there are no boxing bouts returned when querying the API. I have attached screenshots and explanations below of the working web pages below dated from September/October of 2019

Upon starting the application, it will present a list of tables containing the major upcoming professional boxing matches along with the event date and betting odds from particular bookmakers. Users are able to click on a button to load statistics for each fighter on a separate page.

<img src=boxing_odds_images/main_page.jpg width=500>

A typical table would display the fighters, the fight date, betting odds from particular bookmakers and buttons that will redirect the user to a separate page:

<img src=boxing_odds_images/example_table.jpg width=700>

Upon clicking on a button to see a particular boxer's information, the page would display the athelete's information.
In the example below, we have chosen to look up more information on Errol Spence Jr

<img src=boxing_odds_images/profile_example.jpg width=300>
