**Task 6: Attention and Transformer Reflection**



**Question** - Why RNNs struggle with long-term dependencies

***Answer:***

RNNs struggle with very long sequences because of the vanishing gradient problem.



**Technical reason**

During backpropagation, gradients are repeatedly multiplied through many time steps. If these values are small, the gradient can shrink rapidly toward zero.



**Practical result**

The model gradually “forgets” how earlier words influenced later outputs.



**Analogy**: It is like passing a message through a long whisper chain. By the time the message reaches the last person, it becomes faint or distorted.



This is why plain RNNs are weak at capturing long-term dependencies.



\--------------------------------------------------------------------



**Question -** How LSTMs help with memory

**Answer:** 

LSTMs were designed to solve the main weakness of RNNs.



They introduce:



a cell state for long-term memory

a hidden state for short-term output

gates that control what information is kept, forgotten, or exposed

Why LSTMs work better

Instead of treating all information equally, LSTMs selectively manage memory.



Analogy: Think of packing for a trip.



the forget gate throws out what you no longer need

the input gate adds important new items

the output gate decides what to take out and use right now

This controlled memory flow helps LSTMs handle long sequences much better than standard RNNs.



\--------------------------------------------------------------------



**Question -** What attention solves in sequence-to-sequence tasks

**Answer:**

Attention allows the model to focus on the most relevant parts of the input sequence while generating each output token. Instead of relying only on the final encoder state, the decoder can “look back” at all encoder states and decide which ones matter more.



*Why attention matters*

Not every word in the input is equally important for generating every word in the output.



Example

In translation, when generating a translated verb, the model may need to pay special attention to the corresponding verb in the source sentence.



Analogy

It is like studying with a highlighter. For each question, you revisit the exact lines that matter instead of rereading everything equally.



\--------------------------------------------------------------------



**Question -** Why transformers are important in modern NLP and Generative AI

**Answer**



Transformers are architectures built primarily around attention rather than recurrence.



This was a major shift because transformers can process all words in a sequence in parallel, unlike RNNs, which process one step at a time.



Why transformers became dominant



They offer:

better handling of long-range dependencies

parallel computation

greater scalability

strong performance on many NLP tasks

Positional Encoding

Since transformers process tokens in parallel, they need a way to represent word order.



This is done using positional encoding.



Analogy

Imagine receiving all the pieces of a jigsaw puzzle at once. You still need clues about where each piece belongs. Positional encoding provides that order information.



Why this matters for generative AI

Transformers form the backbone of modern models such as:



GPT

BERT

These models power many applications in generative AI and language understanding.

