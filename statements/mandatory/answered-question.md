# Answered a question 

## Description

The user answered a question in the assessment.

## Examples

```json
{
   "actor": {
      "account": {
         "name": "john",
         "homePage": "http://gaiax.org"
      }
   },
   "verb": {
      "id": "http://adlnet.gov/expapi/verbs/answered"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/12d4f3f2-58e0-4a42-b3c6-b9b9cd7b0a7c",
      "definition": {
         "interactionType": "choice"
      }
   },
   "context": {
      "contextActivities": {
         "category": [
            {
               "id": "http://schema.dases.eu/xapi/profile/assessment",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ],
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/0f5c4525-8778-4403-8e3e-b75c4feed309",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/assessment"
               }
            }
         ]
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Properties

- `verb.id`: INCLUDED, must be `http://activitystrea.ms/start`
- `context.contextActivities.parent`: MUST contain an activity with the `http://adlnet.gov/expapi/activities/assessment` definition.type.

## Rules

- `object.definition.interactionType`: INCLUDED, must be specified.
- `context.contextActivities.category`: MUST contain an activity with the `http://schema.dases.eu/xapi/profile/assessment` id.
- `result.score.min`: RECOMMENDED.
- `result.score.max`: RECOMMENDED.
- `result.score.scaled`: RECOMMENDED.
- `result.success`: RECOMMENDED.
- `result.response`: RECOMMENDED.
- `timestamp`: INCLUDED