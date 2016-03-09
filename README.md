# Church Online Platform API Documentation

## Events End Point
An JSON end point for Church Online Platform events.

**Note:** *mychurch* in the URL is from your church's unique Church Online Platform URL.

### Current Event
Returns the current event.

#### URI
http://*mychurch*.churchonline.org/api/v1/events/current

#### Example Response
```json
{
   "meta":{
      "status":200
   },
   "response":{
      "item":{
         "isLive":true,
         "eventStartTime":"2016-03-09T03:39:00Z"
      }
   }
}
```

### All Events
Returns all events.

#### URI
http://*mychurch*.churchonline.org/api/v1/events

#### Example Response
```json
{
   "meta":{
      "status":200
   },
   "response":{
      "count":2,
      "items":[
         {
            "id":12345,
            "organizationId":1234,
            "description":"Church Online Campus",
            "duration":30,
            "enabled":false,
            "speaker":"Tim Smart",
            "title":"A Sunday Service",
            "eventNotes":"",
            "volunteerNotes":"",
            "facebookMessage":null,
            "twitterMessage":null,
            "emailMessage":null,
            "socialLink":null,
            "slidesPaused":false,
            "enabledFeatures":[
               "chat",
               "notes",
               "map_default_opened"
            ],
            "customTab":{
               "id":1234,
               "title":"Who is Jesus?",
               "content":"<p>Jesus is tha man.</p>",
               "sort_order":null,
               "visible":true,
               "permanent":false,
               "created_at":"2015-04-13T02:45:20.724Z",
               "updated_at":"2015-04-13T02:45:20.724Z",
               "organization_id":1234
            },
            "videoProfileStatus":"default"
         },
         {
            "id":12346,
            "organizationId":1234,
            "description":"Church Online Campus",
            "duration":61,
            "enabled":false,
            "speaker":"Tim Smart",
            "title":"The Lion and the Lamb",
            "eventNotes":"",
            "volunteerNotes":"",
            "facebookMessage":null,
            "twitterMessage":null,
            "emailMessage":null,
            "socialLink":null,
            "slidesPaused":false,
            "enabledFeatures":[
               "chat",
               "notes",
               "map_default_opened"
            ],
            "customTab":{
               "id":1234,
               "title":"Who is Jesus?",
               "content":"<p>Jesus is tha man.</p>",
               "sort_order":null,
               "visible":true,
               "permanent":false,
               "created_at":"2015-04-13T02:45:20.724Z",
               "updated_at":"2015-04-13T02:45:20.724Z",
               "organization_id":1234
            },
            "videoProfileStatus":"simulated"
         }
      ]
   }
}
```
