# Discipline
---
The Discipline domain is based upon the concepts of a DisciplineIncident (i.e., the violation or offense) and a DisciplineAction (i.e., the punishment).
* A DisciplineIncident represents the actions or behaviors that constitute an “offense” in violation of laws, rules, policies, or norms of behavior. The DisciplineIncident is associated with the school where the incident occurred.
* StudentDisciplineIncidentAssociation links students to DisciplineIncidents and indicates their role in that incident. When multiple students are involved in a DisciplineIncident, the StudentParticipation attribute indicates what the involvement of the student was in that incident (e.g., perpetrator, victim, witness). The Behaviors attribute is used when students have different levels of involvement, and therefore different offenses, for the same discipline incident (e.g., one might have used a knife in a fight versus another who fought without a weapon).
* A DisciplineAction represents the punitive or other actions taken against the students. One or more DisciplineActions may be applied to one DisciplineIncident(e.g., suspension plus after-school study hall). Alternatively, one DisciplineAction could have multiple Disciplines as an attribute to accomplish the same thing.



#### Discipline Model Entities

| Name        | Description  |
|-----------------|------------------|
| DisciplineAction | This event entity represents actions taken by an education organization after a disruptive event that is recorded as a discipline incident. |
| DisciplineIncident | This event entity represents an occurrence of an infraction ranging from a minor heavioral problem that disrupts the orderly functioning of a school or classroom (such as tardiness) to a criminal act that results in the involvement of a law enforcement official (such as robbery). A single event (e.g., a fight) is one incident regardless of how many perpetrators or victims are involved. Discipline incidents are events classified as warranting discipline action. |
| School | This entity represents an educational organization that includes staff and students who participate in classes and educational activity groups. |
| Staff | This entity represents an individual who performs specified activities for any public or private education institution or agency that provides instructional and/or support services to students or staff at the early childhood level through high school completion. For example, this includes:<br/>    1. An "employee" who performs services under the direction of the employing institution or agency is compensated for such services by the employer and is eligible for employee benefits and wage or salary tax withholdings<br/>    2. A "contractor" or "consultant" who performs services for an agreed upon fee or an employee of a management service contracted to work on site<br/>    3. A "volunteer" who performs services on a voluntary and uncompensated basis<br/>    4. An in-kind service provider<br/>    5. An independent contractor or businessperson working at a school site. |
| Student | This entity represents an individual for whom instruction, services, and/or care are provided in an early childhood, elementary, or secondary educational program under the jurisdiction of a school, education agency or other institution or program. A student is a person who has been enrolled in a school or other educational institution. |
| StudentDisciplineIncidentAssociation | This association indicates those students who were victims, perpetrators, witnesses, and reporters for a discipline incident. |


![Discipline Model Diagram](/path/to/domain-model.png)
#### Discipline Model  

