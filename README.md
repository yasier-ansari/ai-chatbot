<<<<<<< HEAD
# Implementation of a Contextual Chatbot in PyTorch.  
Simple chatbot implementation with PyTorch. 
- The implementation is straightforward with a Feed Forward Neural net with 2 hidden layers.
- Customization for your own use case is super easy. Just modify `intents.json` with possible patterns and responses and re-run the training (see below for more info).

The approach is inspired by this article and ported to PyTorch: [https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077](https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077).


## Installation

### Create an environment
Whatever you prefer (e.g. `conda` or `venv`)
```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

### Activate it
Mac / Linux:
```console
. venv/bin/activate
```
Windows:
```console
venv\Scripts\activate
```
### Install PyTorch and dependencies

For Installation of PyTorch see [official website](https://pytorch.org/).

You also need `nltk`:
 ```console
pip install nltk
 ```

If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Usage
Run
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```
## Customize
Have a look at [intents.json](intents.json). You can customize it according to your own use case. Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```
=======
[//]: # (# Implementation of a Contextual Chatbot in PyTorch.  )

[//]: # (Simple chatbot implementation with PyTorch. )

[//]: # ()
[//]: # (- The implementation should be easy to follow for beginners and provide a basic understanding of chatbots.)

[//]: # (- The implementation is straightforward with a Feed Forward Neural net with 2 hidden layers.)

[//]: # (- Customization for your own use case is super easy. Just modify `intents.json` with possible patterns and responses and re-run the training &#40;see below for more info&#41;.)

[//]: # ()
[//]: # (The approach is inspired by this article and ported to PyTorch: [https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077]&#40;https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077&#41;.)

[//]: # ()
[//]: # (## Watch the Tutorial)

[//]: # ([![Alt text]&#40;https://img.youtube.com/vi/RpWeNzfSUHw/hqdefault.jpg&#41;]&#40;https://www.youtube.com/watch?v=RpWeNzfSUHw&list=PLqnslRFeH2UrFW4AUgn-eY37qOAWQpJyg&#41;)

[//]: # ()
[//]: # (## Installation)




[//]: # ()
[//]: # (### Create an environment)

[//]: # (Whatever you prefer &#40;e.g. `conda` or `venv`&#41;)

[//]: # (```console)

[//]: # (mkdir myproject)

[//]: # ($ cd myproject)

[//]: # ($ python3 -m venv venv)

[//]: # (```)

[//]: # ()
[//]: # (### Activate it)

[//]: # (Mac / Linux:)

[//]: # (```console)

[//]: # (. venv/bin/activate)

[//]: # (```)

[//]: # (Windows:)

[//]: # (```console)

[//]: # (venv\Scripts\activate)

[//]: # (```)

[//]: # (### Install PyTorch and dependencies)

[//]: # ()
[//]: # (For Installation of PyTorch see [official website]&#40;https://pytorch.org/&#41;.)

[//]: # ()
[//]: # (You also need `nltk`:)

[//]: # ( ```console)

[//]: # (pip install nltk)

[//]: # ( ```)

[//]: # ()
[//]: # (If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:)

[//]: # (Run this once in your terminal:)

[//]: # ( ```console)

[//]: # ($ python)

[//]: # (>>> import nltk)

[//]: # (>>> nltk.download&#40;'punkt'&#41;)

[//]: # (```)

[//]: # ()
[//]: # (## Usage)

[//]: # (Run)

[//]: # (```console)

[//]: # (python train.py)

[//]: # (```)

[//]: # (This will dump `data.pth` file. And then run)

[//]: # (```console)

[//]: # (python chat.py)

[//]: # (```)

[//]: # (## Customize)

[//]: # (Have a look at [intents.json]&#40;intents.json&#41;. You can customize it according to your own use case. Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.)

[//]: # (```console)

[//]: # ({)

[//]: # (  "intents": [)

[//]: # (    {)

[//]: # (      "tag": "greeting",)

[//]: # (      "patterns": [)

[//]: # (        "Hi",)

[//]: # (        "Hey",)

[//]: # (        "How are you",)

[//]: # (        "Is anyone there?",)

[//]: # (        "Hello",)

[//]: # (        "Good day")

[//]: # (      ],)

[//]: # (      "responses": [)

[//]: # (        "Hey :-&#41;",)

[//]: # (        "Hello, thanks for visiting",)

[//]: # (        "Hi there, what can I do for you?",)

[//]: # (        "Hi there, how can I help?")

[//]: # (      ])

[//]: # (    },)

[//]: # (    ...)

[//]: # (  ])

[//]: # (})

[//]: # (```)


add imports
>>>>>>> 4783903 (hello)
