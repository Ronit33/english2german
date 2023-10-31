# english2german
## To run this tranlator directly:

```

def predict(text):
  from transformers import pipeline
  pipe = pipeline(model="ronit33/english2german")
  prefix = "translate English to German:"

  input = f"{prefix} {text}"

  output = pipe(input)

  return output[0]["generated_text"]
```
### Just change the text
```
predict("Hello, I am Ronit. I like NLP.")
```
### Sample output
```
Hallo, ich bin Ronit. Ich mag NLP.

```
