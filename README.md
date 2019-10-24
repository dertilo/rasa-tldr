# rasa TLDR 

## [minimal_project](https://rasa.com/docs/rasa/user-guide/rasa-tutorial/)

    mkdir minimal_project && cd minimal_project
    rasa init --no-prompt # create config-ymls and trains NLU + Core
    rasa shell # interact with chatbot
    rasa train # trains NLU+Core if nlu.md or stories.md have changed since last training
    
* in [stories.md](minimal_project/data/stories.md) lines that start with `-` are actions taken by the bot
* [domain.yml](rasa-tldr/minimal_project/domain.yml) : 
    1. intents: things you expect users to say
    2. actions:	things the bot can do and say
    3. templates: for natural language generation
    