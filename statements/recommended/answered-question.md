# Answered a question 

## Description

The user answered a question in the quiz.

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
            "type": "http://adlnet.gov/expapi/activities/question"
      }
   },
   "context": {
      "contextActivities": {
         "category": [
            {
               "id": "https://w3id.org/xapi/quiz",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ],
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/0f5c4525-8778-4403-8e3e-b75c4feed309",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/cmi.interaction"
               }
            }
         ]
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `http://adlnet.gov/expapi/verbs/answered` |
| object.definition.type | Must be `http://adlnet.gov/expapi/activities/question` |

## Rules

- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/quiz` id.
- `context.contextActivities.parent`: INCLUDED, MUST be the quiz activity.
<!-- - `result.score.min`: RECOMMENDED.
- `result.score.max`: RECOMMENDED.
- `result.score.scaled`: RECOMMENDED.
- `result.success`: RECOMMENDED. -->
- `result.response`: INCLUDED.
- `timestamp`: INCLUDED.