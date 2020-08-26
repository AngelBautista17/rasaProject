## need something 
* greet
  - utter_greet
* need_something{"something":"hospital"}
  - utter_place
* give_info{"place":"Chicago"}
  - buscar_lugar
* thanks
  - utter_youreWelcome

## need something + place 
* greet
  - utter_greet
* need_something{"something":"hospital","place":"Chicago"}
  - buscar_lugar
* thanks
  - utter_youreWelcome
  
## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
