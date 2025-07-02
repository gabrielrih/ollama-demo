# ollama-demo
A demo using AI runnin on my local machine (Ollama).

## Ollama

Ollama runs a local web service that gives an OpenAI compatible endpoint and runs models locally using high performance C++ code.

If you don't have Ollama, install it here by visiting [https://ollama.com](https://ollama.com).

After it's installed, you should be able to visit here: ```http://localhost:11434```

> You might need to run `ollama serve`

For more ollama commands please run `ollama --help`

## Using a model

Now, you should choice and download a model from [https://ollama.com/search](https://ollama.com/search). The model called **llama3.3** is too large for home computers, so I recommend the use of a smaller one (like **llama3.2:1b**). For testing purpose you can focus on models with no more than 8B of parameters.

Then, you can pull it: ```ollama pull llama3.2:1b```

> To stop the model just run `ollama stop llama3.2:1b`

## Preparing the repo to be used

Starting by running `uv self update` to guarantee that you're using the latest version of uv.

And now simply run:
```
uv sync
```

## Demo notebooks

And finally, we can use this local AI model to run some demo notebooks:

- [questioning_and_answering_myself.ipynb](./notebooks/questioning_and_answering_myself.ipynb)
