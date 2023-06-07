# Completed

## Description

The learner viewed or did all of the relevant activities in an assignment, by experiencing all relevant materials.
The criterion for determining relevant learning materials is defined by the course designer.
For a given assignment in a given course registration, not multiple `completed` statements can be generated for a given learner.

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
      "id": "http://adlnet.gov/expapi/verbs/completed"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/12d4f3f2-58e0-4a42-b3c6-b9b9cd7b0a7c",
      "definition": {
         "type": "http://adlnet.gov/expapi/activities/cmi.interaction",
         "name": {
            "en": "How much do you know about xAPI?"
         }
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
         ]
      }
   },
   "result": {
      "completion": true,
      "duration": "PT16.36S"
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `http://adlnet.gov/expapi/verbs/completed` |
| object.definition.type | Must be `http://adlnet.gov/expapi/activities/cmi.interaction` |

## Rules

- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/quiz` id.
- `result.score`: EXCLUDED.
- `result.success`: EXCLUDED.
- `result.completion`: INCLUDED.
- `result.duration`: INCLUDED.
- `timestamp`: INCLUDED.