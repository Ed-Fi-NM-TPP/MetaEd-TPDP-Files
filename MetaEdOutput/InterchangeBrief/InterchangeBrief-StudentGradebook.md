# Student Gradebook Interchange

# Overview

The Student Gradebook interchange describes student gradebook entries. Gradebook entries are assignments and students' results on those assignments. The assignments themselves may be linked to learning standards or learning objectives.



Like all standard Ed-Fi interchanges, this schema references the Ed-Fi Core XSD and can be extended using the Ed-Fi Extensions Framework. See the [Ed-Fi Data Standard - Developers' Guide] for more information.


# Use Cases

The Student Gradebook Interchange can be used to:  

1. Exchange assignments created by teachers and optionally linked to learning standards or learning objectives.
    2. Exchange students' performance on assignments.


# Model Details

The following figure shows a logical view of the Student Gradebook Interchange schema:  

![Student Gradebook model details diagram](img/InterchangeStudentGradebook-interchange-brief.png)


# Entities

The following table describes the primary entities of which the Student Gradebook Interchange is composed.  

| Name | Description |
|----------|-----------------|
| SectionReference | This entity represents a setting in which organized instruction of course content is provided, in-person or otherwise, to one or more students for a given period of time. A course offering may be offered to more than one section. |
| GradebookEntry | This entity represents an assignment, homework, or classroom assessment to be recorded in a gradebook. |
| StudentGradebookEntry | This entity holds a student's grade or competency level for a gradebook entry. |
| LearningObjective | This entity represents identified learning objectives for courses in specific grades. |



# Extended References


This interchange includes the following Extended References.  

| Extended Reference Name | Description |
|-----------------------------|-----------------|
| ClassPeriodReference (in Section) | Required.  The class period during which the Section meets. |
| CourseOfferingReference (in Section) | Required.  The course offering taught in the Section. |
| GradingPeriodReference (in GradebookEntry) | Optional.  Identifies the grading period for the GradebookEntry. |
| LearningStandardReference (in GradebookEntry) | Optional.  LearningStandard(s) associated with the GradebookEntry. |
| LearningStandardReference (in LearningObjective) | Optional.  LearningStandard(s) included in this objective. |
| LocationReference (in Section) | Required.  The location, typically a classroom, where the Section meets. |
| MandatingEducationOrganizationReference (in LearningObjective) | Optional.  Optionally relates the entity mandating the use of the content standard. |
| StudentSectionAssociationReference (in StudentGradebookEntry) | Required.  Relates the student associated with the GradebookEntry. |



# Descriptor Dependencies

This interchange references the following Ed-Fi Descriptors, thus requiring them to have been defined using the Descriptors interchange prior to this interchange. For more information on the Ed-Fi Descriptor Pattern, see the [Ed-Fi Data Standard - Developers' Guide].  

| Descriptor Name | Description |
|---------------------|-----------------|
| AcademicSubjectDescriptor | Required.  This descriptor holds the description of the content or subject area (e.g., arts, mathematics, reading, stenography, or a foreign language). |
| CompetencyLevelDescriptor | Optional.  This descriptor defines various levels for assessed competencies. |
| GradeLevelDescriptor | Required.  This descriptor defines the set of grade levels. The map to known Ed-Fi enumeration values is required. |


