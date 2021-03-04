# wen-events

A community Moderated list of events displayed on https://wen.pm

In this repo you can collaboratively add events that will be included in wen.pm. 
Just make sure that the JSON format is still valid when you add something.
Please only add your own content and don't delete or modify others content!

## How To
To add a stream event edit the `streams.json` and add a new entry.

### Entries
Entries look like this:

```json
{
  "title": "Lovelace Academy",
  "blurb": "The Cardano Revolution. Why you should build on Cardano.",
  "url":   "https://www.youtube.com/watch?v=sM0_V53_kGo",
  "language": "en",
  "timestamp": "1614803400",
  "duration": "3600"
}
```
### Fields:

* `title`: The title of your next stream (eg: "ShowXYZ: How many pools should one delegate to?")
  Please try and keep the title below 80 chars.
* `blurb`: This will be displayed below your title. There is more place for text here.
* `url`: The Url where the stream will be, or the page where you want people to get when they click on your event
* `language`: In what language is this event going to be? NOTE: this will be used by wen.pm in the future but you must add it now
* `timestamp`: A unix timestamp of when your event starts. Tip: https://www.unixtimestamp.com/ can help you make that
* `duartion`: How long will your event last (in seconds). If your event is currently running, visitors of https://wen.pm will see a _"Now on Air!"_ sign.

### Syntax

JSON requires you to separate list items with a comma `,` but blows up if you add a comma to the last item. Make sure before you save that the document is valid JSON like this:

```json
[{
  "title": "Event1",
  "blurb": "The Cardano Revolution....",
  "url":   "https://www.youtube.com/watch?v=sM0_V53_kGo",
  "language": "en",
  "timestamp": "1614803400",
  "duration": "3600"
},
{
  "title": "Some Cool Title!",
  "blurb": "How many Xs....",
  "url":   "https://www.youtube.com/watch?v=sM0_V53_kGo",
  "language": "en",
  "timestamp": "1614803401",
  "duration": "3600"
}]
```
