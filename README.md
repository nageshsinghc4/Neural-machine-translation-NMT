# Neural-machine-translation-NMT
![NMT](https://github.com/nageshsinghc4/Neural-machine-translation-NMT/blob/master/021519-pic2.png)

Here, we will create a LSTM encoder-decoder model that will translate English sentences into their French-language counterparts using Keras and python.

The data set can be downloaded from [here](http://www.manythings.org/anki/).

For more information and step by step explaination, please go through this medium article: https://www.theaidream.com/post/how-ai-is-changing-personal-data-tracking

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
