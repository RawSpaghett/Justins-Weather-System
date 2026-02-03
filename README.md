Justin's C++ Markov Weather System
Why?
Cause it’s cool! Previous to creating this, I had no idea what a ‘Markovs chart Weather Probability simulator” even was and it took me about an hour to wrap my head around it. After I got my bearings, I discovered what it could do. A fluid and realistic weather simulation that can be implemented into games.

Resources
  Intro to Markovs Chart
  C++ standard library headers
  Differences between c# and c++

Key points
  Provides output to external weather system
  Linearly Interpolated Seasons
  Realistic weather patterns


DONT FORGET
  Assume user inputs “banana” for everything

Psuedo-code

#Include
  Random Number
  Vectors
  Strings
  Iostream
  Map

Initialize 
  CurrentWeather
  CurrentSeason
  CurrentDay = 0;
  SeasonLength
  RandomNumber
  Tomorrow's Weather
  Continue

  4 3x3 Seasonal matrices ( Sunny, Rainy, Cloudy )
  Spring
    Cloudy, rainy, and sunny
  Summer
    Rainy and sunny
  Fall
    Cloudy and sunny
  Winter
    Cloudiest

Supporting Functions
  MarkovFunction(CurrentSeason,CurrentWeather,RandomNumber)
    Updates Season
    If CurrentDay is more than Seasonlength, change season to the next season
    Debug.log “Welcome to” + CurrentSeason”;
    Determine Matrix (using season)
    Determine Row (using current)
    Determine index (using Random)
    Update TommorowWeather
    Debug.log “Tommorows weather is “ +TommorowWeather
Main Function
  Determine the current season (Input)
    Convert to int
  Determine the current days weather (Input)
    Convert to int
  Determine length of seasons (input)
  Determine random integer(<random>)
  MarkovFunction
  Wait for input to continue to next day
  If y
    While ( Continue )
    CurrentWeather = TomorrowWeather
    Determine random integer
    MarkovFunction(CurrentSeason,CurrentWeather,RandomNumber)
    Continue? input
  If n 
    Continue != Continue
  If y
    CurrentWeather = TomorrowWeather
    CurrentDay++
  else
    Thanks for using Justin's Weather Simulator
    Return 0;



