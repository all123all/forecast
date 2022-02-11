# Forecast

  ## Description 
  This project was made using ReactJS, Axios and the OpenWeatherMap API. Basically it has an input where you enter the name of the city then the page shows a card with some forecast information about the city you entered.
  
  ## Installation 
  In `./src/api/` you will need a file called `fetchWeather.js`. Create one by yourself then write the code below using your OpenWeatherMap `API_KEY`:
```
    import axios from 'axios';

    const URL = "https://api.openweathermap.org/data/2.5/weather";
    const API_KEY = ""; //insert you API_KEY here

    export const fetchWeather = async (query) => {
        const { data } = await axios.get(URL, {
            params: {
                q: query,
                units: 'metric',
                APPID: API_KEY,
            }
        });
        return data;
    }
```

![Home Page](print.png)

  ## Contact me
  If you want to know more about me or the projects i'm working on you can contact me on allyson2308h@gmail.com. You can view more of my projects at                   https://github.com/all123all.

