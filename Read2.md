# Investigate appropriate APIs for the City Explorer System, you need to explain the following for each API that will be used:-

## When I created the city-explorer app, I used some APIs, including:-

1. Location API
2. Movie API
3. Weather API

***

## Location API:-

* API Description:-

**LocationIQ offers enterprise-grade location-based solutions that are adaptable. They collaborate with developers, entrepreneurs, and businesses all around the world to serve billions of requests every day.**

* API Usage:-

Requests can be sent to the following endpoint

> [GET https://maps.locationiq.com/v3/staticmap](https://maps.locationiq.com/v3/staticmap)

* API Endpoints/Request URLs:-

### We use `Static Maps`

**Requests can be sent to the following endpoint:**

> [https://maps.locationiq.com/v3/staticmap](https://maps.locationiq.com/v3/staticmap)

**Endpoints:**

**You'll need to utilize either the `Style Specification URL` or `Tile URLs`, depending on the Maps SDK you use.**

### Style Specification URL:-

**Use a Style Specification URL for Mapbox-GL SDKs. The following is an example of a Style URL:**

> [https://tiles.locationiq.com/v3/<theme>/<type>.json?key=<access_token>](https://tiles.locationiq.com/v3/<theme>/<type>.json?key=<access_token>)

**Tile URLs:**

**Tile URLs must be specified for LeafletJS and other mapping libraries:**

> [https://{s}-tiles.locationiq.com/v3/<theme>/r/{z}/{x}/{y}.<format>?key=<access_token>](https://{s}-tiles.locationiq.com/v3/<theme>/r/{z}/{x}/{y}.<format>?key=<access_token>)

* Authentication Key:-

**The key is protection for many requests, and there are specific requests for each key to maintain security.**

**My key is :- `pk.414d5512d3a845acb5bad64c1f17ff42`**

***

## Movie API:-

* API Description:-

**The Movie Database (TMDB) is a movie and television database created by the public. Since 2008, our incredible community has contributed every piece of information. TMDb's worldwide emphasis and data breadth are unrivaled, and it's something we're really proud of.**

* API Usage:-

  * search/movie

   **Requests can be sent to the following endpoint:**

   [https://api.themoviedb.org/3/search/movie](https://api.themoviedb.org/3/search/movie)

* API Endpoints/Request URLs:-

**Search for movie by:**

[`https://api.themoviedb.org/3/search/movie?api_key=${process.env.MOVIE_API_KEY}&query=${searchQuery}`](https://api.themoviedb.org/3/search/movie?api_key=${process.env.MOVIE_API_KEY}&query=${searchQuery})

* Authentication Key:-

**The key is protection for many requests, and there are specific requests for each key to maintain security.**

**My key is :- `a2411869623599fcff65ca236aa20474`**

***

## Weather API:-

* API Description:-

* A weather API is an Application Programming Interface that allows scripts and programs to query weather data. Weather APIs give both historical and forecast weather data through a simple, well-defined programming interface.

* On the web, the most accurate collection of historical weather observations. Multiple data sources are utilized, including station data, satellite data, radar, and more!

* API Usage:-

  * 16 Day Weather Forecast API (1 day interval)

    **Requests can be sent to the following endpoint:**
   > [http://api.weatherbit.io/v2.0/forecast/daily](http://api.weatherbit.io/v2.0/forecast/daily)

* API Endpoints/Request URLs:-

| Description | Required Parameters | Example(s)    |
| :---        |    :----:   |          ---: |
| Get forecast by lat/lon (Recommended)    | lat,lon   | &lat=38.123&lon=-78.543  |
***
**Example Request:**

[`https://api.weatherbit.io/v2.0/forecast/daily?city=Raleigh,NC&key=API_KEY`](https://api.weatherbit.io/v2.0/forecast/daily?city=Raleigh,NC&key=API_KEY)

* Authentication Key:-

**The key is protection for many requests, and there are specific requests for each key to maintain security.**

**My key is :- `daea5b55c97e4b488d70c878b1085e68`**

***
***

## Links

* Frontend:

  [GitHub repo link](https://github.com/Ahmad-Abulaban/city-explorer)

  [Live URL link - Netlify](https://city-explorer-labs.netlify.app/)

* Backend:

  [GitHub repo link](https://github.com/Ahmad-Abulaban/city-explorer-api)

  [Live URL link - Heroku](https://city-explorer9-api.herokuapp.com/)
