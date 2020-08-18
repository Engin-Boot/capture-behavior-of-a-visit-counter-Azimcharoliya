# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the hospital has visitor count sensor system working\
  When the director requests the report of patient visits\
  Then display patient visits during working days and holidays to director.
  
Scenario: Compute parking slots to reserve for visiting specialists

  Given the hospital has visitor count sensor system working\
  When the director requests to reserve parking slots\
  Then check availablity of parking spots
  if available then reserve the spots
  else display parking slots not available to director and
  notify the director when the parking spots are available.
