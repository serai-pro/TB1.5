# What's TB1.5
TB1.5 it's a powerfull model language, powered by SerAI. Using informations from Google/Bing that are searched when a user sends a message.
Ofcourse it can think by himself too, the Google/Bing is in-built feature used only if you don't select any type

example:

```https://serai.pro/api/1.5/api?key=DEMO&type=1/0&msg=test```

# Let's show the types and everything.

/api/1.5 => this is the ThunderBird 1.5 model language.

/api/1.0 => this is the Thunderbird 1.0 model language.

api.php/api => this is the request you're gonna fetch and result the Output of the overall message.

key=YOUR_KEY => this is used to identify what API KEY you're using, if it's NULL (0, empty) there won't be any output from the api, for a api key go to https://serai.pro/SerAI_Settings

type= 1 or 0 => this is the TYPE used for the Google/Bing/YouTube, when the type is 0 it won't search on google/bing, when the type is 1 it will, DEFAULT:1.

YouTube Data API => We use this for the music, so when you search for example:
Play: A music name
It will play on the website the music, when you tell him to pause/stop it will stop it, for pause it will stop it for a amount or time or till you start it again.

msg=Your_Message => this is used for the output, like when you fetch a message it gotta have a $input_text like this:
```https://serai.pro/api/1.5/api?key=DEMO&msg=hi```
it will output this: What's up? how are you doing today?

# How serai.pro works

The AI it will send a request to 3 files:

save_chat.php => used to save the chat in a database with user masssage/ip etc (this is used for actually tracking the person messages, if the message is blacklisted it won't be saved)

Thunderbird_Verification_System?search=a => this will search "a" on bing/google only if theres a type=0 it won't. It will try to verify user message too so there won't be any blacklisted messages or something like that, so the AI will can't be jailbreaked or be modified by the user preference, example: it can't be shutted down with a prompt.

thunderbird => it's the API using the latest model.
