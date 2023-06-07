# Terminated

## Description

The assignment was terminated by the learner and not any more statements will be sending for the launched assignment session.
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
      "id": "http://adlnet.gov/expapi/verbs/terminated"
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
      "duration": "PT16.36S"
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `http://adlnet.gov/expapi/verbs/terminated` |
| object.definition.type | Must be `http://adlnet.gov/expapi/activities/cmi.interaction` |

## Rules

- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/quiz` id.
- `result.score`: EXCLUDED.
- `result.success`: EXCLUDED.
- `result.completion`: EXCLUDED.
- `result.duration`: INCLUDED.
- `timestamp`: INCLUDED.