# Neural-machine-translation-NMT
![NMT](https://github.com/nageshsinghc4/Neural-machine-translation-NMT/blob/master/021519-pic2.png)

Machine translation is a subfield of computational linguistics that is focused on the task of automatically converting source text in one language to text in another language.

In machine translation, the input already consists of a series of symbols in some language, and the computer program must convert this into a series of symbols in a different language.

Neural machine translation (NMT) is a proposition to machine translation that uses an artificial neural network to predict the probability of a sequence of words, typically modeling whole sentences in a single integrated model.

With the power of Neural networks, Neural Machine Translation (NMT) has emerged as the most powerful algorithm to perform this task. This state-of-the-art algorithm is an application of deep learning in which massive datasets of translated sentences are used to train a model capable of translating between any two languages.

Here, we will create a LSTM encoder-decoder model that will translate English sentences into their French-language counterparts using Keras and python.

The data set can be downloaded from [here](http://www.manythings.org/anki/).

For more information and step by step explaination, please the article on [www.theaidream.com](https://www.theaidream.com/post/how-ai-is-changing-personal-data-tracking) 

## Predictions
To test the performance we will randomly choose a sentence from the input_sentences list, retrieve the corresponding padded sequence for the sentence, and will pass it to the translate_sentence() method. The method will return the translated sentence.
```
i = np.random.choice(len(input_sentences))
input_seq = encoder_input_sequences[i:i+1]
translation = translate_sentence(input_seq)
print('Input Language : ', input_sentences[i])
print('Actual translation : ', output_sentences[i])
print('French translation : ', translation)
```

**Results:**

![Results](https://github.com/nageshsinghc4/Neural-machine-translation-NMT/blob/master/Screenshot%202020-10-16%20at%209.43.26%20AM.png)

You can follow my kaggle kernel for [NMT with attention mechanism](https://www.kaggle.com/nageshsingh/neural-machine-translation-attention-mechanism) implementation.
