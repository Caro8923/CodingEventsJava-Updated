1. The purpose of this app is to provide a dynamic event's page,
  where users can search existing events based on their favorite event categories,
  create new events, and save upcoming events to their personal event calendar. 

2. The app currently contains an Event Repository the stores existing and new events. It also
   organizes events by relating each event to an event category. Event categories can correspond
   to multiple events, and can be updated dynamically as new event types are created. The Event
   and EventCategory are connected to MySQL so that the data can be stored in a database. Users
   can visit the webpage, search events by category, and create unique events.

4. I intend to add a Person class that gives the user a personalized profile.
     The person class would contain these fields :
       id (int)
       firstName (String)
       lastName (String)
       email (String)
       password (String)

       Getters for all fields, Setters for all fields excluding id.

     The person class would reference :
       PersonProfile (class to gather user info)
       List<Events> eventsAttending (stores events user wants to attend)
       List<Events> eventsOwned (stores user-created events)

     Person and Event have a many-to-many relationship via eventsAttending
     Person and Event would have a one-to-many relationship via eventsOwned
     
