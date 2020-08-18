# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given the hospital has visitor count sensor system working\
  When the facilities manager requests the report of visitor trends\
  Then display visitor trends during a week of operation to facilities manager.

Scenario: Alert when seating capacity is full

  Given the hospital has visitor count sensor system working\
  When the count of active visits is greater than set seating capacity threshold\
  Then alert the facilities manager.
  
Scenario: Alert when parking capacity is full

  Given the hospital has parking system working\
  When the occupied parking is greater than set parking capacity threshold\
  Then alert the facilities manager.
