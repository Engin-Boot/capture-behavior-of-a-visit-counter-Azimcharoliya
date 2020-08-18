# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given the hospital has visitor count sensor system and server system working\
  When I requests the report of patient visits\
  Then compute and display patient visits during working days and holidays.
  
Scenario: Compute parking slots to reserve for visiting specialists

  Given the hospital has parking system working\
  When I requests to reserve parking slots\
  Then check availability of parking spots
  if available then reserve the spots
  else display parking slots not available and
  notify when the parking spots are available.
