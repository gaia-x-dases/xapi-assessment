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
            "interactionType": "choice",
            "type": "http://adlnet.gov/expapi/activities/cmi.interaction"
      }
   },
   "context": {
      "contextActivities": {
         "category": [
            {
               "id": "https://w3id.org/xapi/assessment",
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

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `http://adlnet.gov/expapi/verbs/answered` |
| object.definition.type | Must be `http://adlnet.gov/expapi/activities/cmi.interaction` |

## Rules

- `object.definition`: CMI interaction, including a content type set to `http://adlnet.gov/expapi/activities/cmi.interaction` and other related properties as described in the xAPI specification.
- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/assessment` id.
- `context.contextActivities.parent`: INCLUDED, MUST be the asssessment activity.
- `result.score.min`: RECOMMENDED.
- `result.score.max`: RECOMMENDED.
- `result.score.scaled`: RECOMMENDED.
- `result.success`: RECOMMENDED.
- `result.response`: RECOMMENDED.
- `timestamp`: INCLUDED.