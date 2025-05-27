# IMDB Movie Review Data Classification

## Data
The data contains IMDB movie reviews and labels. Label 0 means negative and label 1 means positive review.

The objective is to fine tune BERT base multilingual cased model for the IMDB review data and build a classifier that classifies movie reviews as positive or negative.

The evaluation metrics on the test dateset are

|Training Loss|Validation Loss|Accuracy|F1-score|
|-------------|---------------|--------|--------|
|0.2022|0.2742|0.909|0.953|

The sample output is

<pre>```

This was a boring and a poorly directed film.
  Logits : tensor([[ 2.4590, -2.4597]]), Argmax : 0
  Probabilities : tensor([[0.9927, 0.0073]]), confidence : 0.9927443265914917
Sentiment : Negative

I really enjoyed this movie. The story, the plot and the acting was superlative. The ending felt a little stretched, 
    could have been reduced, but I liked it overall
  Logits : tensor([[-2.7041,  2.5022]]), Argmax : 1
  Probabilities : tensor([[0.0055, 0.9945]]), confidence : 0.9945477843284607
Sentiment : Positive

OMG ! What a collosal waste of time ! Avoid !!!
  Logits : tensor([[ 2.2393, -2.3877]]), Argmax : 0
  Probabilities : tensor([[0.9903, 0.0097]]), confidence : 0.9903112649917603
Sentiment : Negative

Das war ein wirklich lustiger Film, die Charaktere haben gut gespielt. Es hat Spaß gemacht, ihn anzuschauen.
  Logits : tensor([[-2.3759,  2.2326]]), Argmax : 1
  Probabilities : tensor([[0.0099, 0.9901]]), confidence : 0.9901312589645386
Sentiment : Positive

यह मूवी बहुत ख़राब है।  उन्होंने कुछ भी बना दिया है।  दो घंटे और तीस मिनट बर्बाद कर दिए।  मत देखो। 
  Logits : tensor([[ 0.2697, -0.4739]]), Argmax : 0
  Probabilities : tensor([[0.6778, 0.3222]]), confidence : 0.6777908802032471
Sentiment : Negative

Este foi um dos melhores filmes que assisti nos últimos meses. A história é ótima e a reviravolta no final me prendeu na ponta da cadeira. A cinematografia, a música ambiente e as atuações também são incríveis.
  Logits : tensor([[-2.8125,  2.5670]]), Argmax : 1
  Probabilities : tensor([[0.0046, 0.9954]]), confidence : 0.9954113364219666
Sentiment : Positive

C'est l'un des meilleurs films que j'ai vus depuis des mois. L'histoire est géniale et le rebondissement final m'a tenu en haleine. La photographie, la musique de fond et le jeu des acteurs sont également exceptionnels.
  Logits : tensor([[-2.9148,  2.5639]]), Argmax : 1
  Probabilities : tensor([[0.0042, 0.9958]]), confidence : 0.9958425164222717
Sentiment : Positive

```</pre>
