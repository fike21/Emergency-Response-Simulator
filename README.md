#🚒 Emergency Response Simulator
 
 BY [Fikire Tibebu]  
 
 📝 Description
 
 C# console application simulating emergency unit dispatch to random city incidents, demonstrating OOP principles.
 
  🚀 Features
 - Police, Firefighter, and Ambulance units
 - Random incident generation
 - Scoring system
 - Clean OOP architecture

 - 
 🛠️ How to Run
 ```bash
 dotnet run
 ```

 📊 Class Diagram
 ```mermaid
 classDiagram
     class Incident {
         +string Type
         +string Location
     }
     
     class EmergencyUnit {
         <<abstract>>
         +string Name
         +int Speed
         +bool CanHandle(string)
         +void RespondToIncident(Incident)
     }
     
     EmergencyUnit <|-- Police
     EmergencyUnit <|-- Firefighter
     EmergencyUnit <|-- Ambulance
 ```
