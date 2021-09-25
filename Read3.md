# What is white box testing?

**White Box Testing is a method of software evaluation that involves testing a product's fundamental structure, architecture, and code in order to evaluate input-output flow and improve design, usability, and security. White box testing is also known as Clear box testing, Open box testing, Transparent box testing, Code-based testing, and Glass box testing since the code is visible to the testers.**

***

## White Box Testing Pros and Cons

| Pros        | Required Pros |
| :---        |    :----   |
| Capability of achieving 100% code coverage.    | To automate, a significant amount of effort is required.   |
| It's simple to automate.    | Automation is expensive to maintain since it is sensitive to changes in the code base.   |
| Reduces the amount of time it takes for testers and developers to communicate.    | Expected functionality that does not exist in the source cannot be tested.   |
| Allows for ongoing code and development practice improvement.    | It's impossible to test from the user's point of view.   |

***

## Now let's go do a test for the backend:

![server image](Images/server.png)

**At first, we started with the server file. We did a test for cors, dotenv, express and axios if it was defined or not, by searching for them in the package.json file.**

![package.json](Images/package.png)

***

**Then we did a test for the data that comes from the movie.**

![dataMovie](Images/dataMovie.png)

**It's working. Now let's do a test of the weather data.**

![dataweather](Images/dataweather.png)

**It's working.**

**Now let's do a test for the port to see if the port is working or not.**

![port](Images/port.png)

**It's working.**

**Let's see if you add port and keys to weather and Movie.**

![BackendEnv](Images/BackendEnv.png)

**We do everything activated and added.**
***
## Now let's start doing a test for the weather page:-

![weather](Images/weather.png)

**First we did a test of the data link with my private key.**

![weatherT](Images/weatherTest.png)

**It's working.**

**Now let's try the cache.**

**When doing a test for cache, we will see that when we return the Amman request, we will see that it returns the data from the cashe and does not make another request.**

![cashe](Images/casheT.png)

***

**Now let's start doing a test for the Movie page:-**

![Movie](Images/Movie.png)

**First we did a test of the data link with my private key.**

![MovieT](Images/MovieT.png)

**It's working.**

**Now let's try the cache.**

**When doing a test for cache, we will see that when we return the Amman request, we will see that it returns the data from the cashe and does not make another request.**

![cashe](Images/MovieTest.png)

***
***

## Now let's start doing a test for the frontEnd:-

![Front1](Images-Frontend/Front1.png)

**First we want to do testing for axios and Bootstrap.**

![Front1Test](Images-Frontend/Front1T.png)

**Yes, all we need is defined.**

![Front2](Images-Frontend/Front2.png)

**Now I will test the searchQuery to see if it takes the value we enter or not?**

![frontT2](Images-Frontend/frontT2.png)

**It's working.**

**Now let's do a test for location url, weather url and movie url.**

### location

![LocationUrlT](Images-Frontend/LocationUrlT.png)

### weather
![weatherUrlT](Images-Frontend/weatherUrlT.png)

### movie
![MovieUrlT](Images-Frontend/MovieUrlT.png)

**Everything is good.**

**Now we will talk about Form.**

![MovieUrlT](Images-Frontend/Front3.png)

**I used the form in order to take a value from the user.**

![MovieUrlT](Images-Frontend/FormT.png)

**It works fine.**

**Now I will do a test for the card to see if it works or not.**

![MovieUrlT](Images-Frontend/CardT.png)

**When writing Amman in the form, the results appeared inside the card and it works fine**

***

## Now let's review the code inside the Movie.

![FrontMovie](Images-Frontend/FrontMovie.png)

**Here we have used Table to arrange the data inside a table and to make test we must run the code.**

![FrontMovie](Images-Frontend/TableT.png)

**We did a test for the table and these are the results, everything works fine.**

## Now let's review the code inside the weather.

![FrontMovie](Images-Frontend/FrontWeather.png)

**Let's run the code to see if it prints a WeatherResult which is date and description.**

![FrontMovie](Images-Frontend/WeatherRes.png)

**When I run the code, the results were the same as the results of the data in Weather.**

***