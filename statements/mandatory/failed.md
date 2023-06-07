# Failed

## Description

The user has attempted and failed an assessment.
For a given assignment in a given course registration, not multiple `failed` statements can be generated for a given learner.

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
      "id": "http://adlnet.gov/expapi/verbs/failed"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/12d4f3f2-58e0-4a42-b3c6-b9b9cd7b0a7c",
      "definition": {
         "type": "http://adlnet.gov/expapi/activities/cmi.interaction"
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
      "success": false,
      "duration": "PT16.36S"
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `http://adlnet.gov/expapi/verbs/failed` |
| object.definition.type | Must be `http://adlnet.gov/expapi/activities/cmi.interaction` |

## Rules

- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/quiz` id.
- `result.success`: INCLUDED, MUST be set to `False`.
- `result.duration`: INCLUDED.
- `timestamp`: INCLUDED.