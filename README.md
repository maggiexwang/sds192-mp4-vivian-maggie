# Studying Hollywood Movie Length with IMDb Data

The past few years have given rise to complaints about how major Hollywood productions are getting longer: this 2013 [Business Insider](http://www.businessinsider.com/movies-are-getting-longer-2013-1) article would serve as a reflection. But are movies truly getting longer throughout the years?

Our investigation of the IMDb relational database reveals the steady nature of Hollywood film lengths, and explore further the reason behind the popular perceptions by digging into the ratings and production information of long films.

**Contributions**: background research by Vivian, article jointly authored by Vivian and Maggie, code and graphics by Maggie.

## Findings

The study shows that Hollywood films are not getting longer over time. However, since the length of films often correlates to the quality of the story, budget of the studio, and qualifications of the director, it is likely that the longer films are receiving more public attention, thus creating a perception of movies growing longer during recent years.

Our findings can be summarized in these three main graphs supporting the article. Please refer to the .Rmd file for more detailed write-out and analysis process.

## Notes about code

* Data on Quentin Tarantino's *The Hateful Eight* was manually corrected.
```
ratelength$Length[ratelength$title == "The Hateful Eight"] <- as.integer(187)
```

* Hollywood movies are defined as feature films with 60+ minutes runtimes that were produced or jointly produced in the United States. The 60-minute limit was set as a compromise between the 40-minute standard held by the Academy of Motion Picture Arts and Sciences and the 80-minute line defined by the Screen Actors Guild.
