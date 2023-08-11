# Real-Time Earthquake Mapping + News

## Description

This web application utilizes APIs from USGS [[1]](#references), News [[2]](#references), and Google Cloud Platform (Google Map) [[3]](#references) to create a real-time visualization of recent earthquake events worldwide.

****Features****:
- Recent earthquake data are plotted on the map. The radius of the circle represents magnitude.
- The search bar allows user to input a country name to retrieve related recent news.

****Model View Controller (MVC)**** design pattern is used for this project.
- ****Front-end****: Client side UI: Use Bootstrap for styling and JavaScript events for interactivity.
- ****Back-end****: Server side API: Data are retrived from APIs and processed in JSON format through JavaScript asynchronous programming. Additionally, local storage is set up to allow for continuity of user interaction.

## Demo

![Earthquake](assets/earthquake.gif)

## Local Installation & How to Use

One time set up for virtual environment:
```console
$ python3.10 -m venv .venv
$ source .venv/bin/activate
$ python -m pip install -U pip
$ python -m pip install -r utilities/requirements.txt
$ deactivate
```

Start the application:
```console
$ python -m http.server
```

In the code, replace `insertApiKey` with valid api key.

## Future Improvement

- Filter earthquake and news by date range or magnitude.
- Allow for more search options than just country.
- Need a legend to explain what is being shown on the map.

## Reflection

Overall, I learned to extract data from APIs. Some struggles are as follow:
- Async & await: requested/retrieved data don't show up on time.
- At times, the amount of data are too big and it takes a long time to load.
- API documentations sometimes don't give clear explanations of how to use.
- Many API sources don't give easy or free access.

## References

[1] [USGS | API Documentation](https://earthquake.usgs.gov/fdsnws/event/1/)</br>
[2] [News | API Documentation](https://newsapi.org/)</br>
[3] [Google Cloud Platform | API Documentation](https://cloud.google.com/docs/)</br>

## License

[MIT License](LICENSE)
