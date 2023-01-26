# Emojify
Built a sentiment classifier using word embeddings. This app understands sentiment of the sentence and adds one of the 5 emoji's:

`heart` : ❤️
         
`baseball`: ⚾
              
`smile` : 😄
         
`disappointed` : 😞
  
`fork_and_knife` : 🍴


### Example:

Rather than writing:
>"Congratulations on the promotion! Let's get coffee and talk. Love you!"   

The emojifier can automatically turn this into:
>"Congratulations on the promotion! 👍  I am very happy for you. 😄 Love you! ❤️"

### Working:
Used 2 models, one without using RNN and one with RNN, and can see that the model without RNN dosen't take order of words in account.

Where as the model will RNN understands the arrangement of words and gives better performance. Here we have used LSTM units and pre trained GloVe vectors as Embedding layer from `glove.6B.50d.txt` which can be downloaded from internet which greatly improves performance and helps in better understanding of the sentences.
