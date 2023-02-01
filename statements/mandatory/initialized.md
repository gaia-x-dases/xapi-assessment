# Initialized

## Description

A moderator has initialized an assessment.

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
      "id": "http://adlnet.gov/expapi/verbs/initialized"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/12d4f3f2-58e0-4a42-b3c6-b9b9cd7b0a7c",
      "definition": {
         "type": "http://adlnet.gov/expapi/activities/assessment",
         "name": {
            "en": "How much do you know about xAPI?"
         }
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
         ]
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```
## Properties

- `verb.id`: INCLUDED, must be `http://adlnet.gov/expapi/verbs/initialized`
- `object.definition.type`: INCLUDED, must be `http://adlnet.gov/expapi/activities/assessment`.

## Rules

- `context.contextActivities.category`: MUST contain an activity with the `http://schema.dases.eu/xapi/profile/assessment` id.
- `timestamp`: INCLUDED