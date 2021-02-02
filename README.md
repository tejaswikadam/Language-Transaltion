# Language-Transaltion
The language that I attempted to translate is Marathi-English Translation. The dataset is from the site “ http://www.manythings.org/anki/”


# Character Model:

-	As the dataset taken is small, I have used pretrained model for English language obtained from “ https://nlp.stanford.edu/projects/glove/” to train the model better. The text file taken is “glove.6B.300d.txt” which is of 300 dimensions.

-	The following is observed after training the model.
- The maximum training accuracy of the model is 44% while that of validation is 33%. 
- This model needs lot more learning.	

# Word Model:

-	As the dataset taken is small, I have used pretrained model for English language obtained  from “ https://nlp.stanford.edu/projects/glove/” to train the model better.  Similarly, for pretrained model for Marathi language is obtained from “https://fasttext.cc/docs/en/pretrained-vectors.html” .  The text file taken is “glove.6B.300d.txt” and “indicnlp.v1.mr.vec” respectively which is of 300 dimensions.

-	The following is observed after training the model.
- The maximum training accuracy of the model reached 87% while that of validation is around 78%.
- The model took less time to train than that of character level model.

# Attention Mechanism:

-	Used Bahdanau attention for the encoder.
-	With an attention mechanism, there was no need to try an encode the full source sentence into a fixed-length vector. Rather, it allowed the decoder to “attend” to different parts of the source sentence at each step of the output generation. 
-	Importantly, the model learnt what to attend based on the input sentence and what it has produced so far.
