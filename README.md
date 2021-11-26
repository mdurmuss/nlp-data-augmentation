# Data Augmentation for NLP
Data augmentation is a very popular method in computer vision but they can be useful when your data is text.



### Data Augmentation Techniques

1. **Back Translation** :traffic_light:

   Translate the text to another language and then translate it back to your language. This may generate text data with different words without changing the meaning of the sentence.

   ![](https://lh6.googleusercontent.com/x3ZAhTDLT1QVSD8gCdaBVMquM2dcYA15A-orfzXyTzhTP8m0ZKLXz_2NrJdWlTgWKRS7BimExM8RO9Ce_uVVVdRR29vGeP0VZdncDZY0GTwkctocQyYg7HK9VL5ay3QC4JhbSXBK)

	Google-translate, yandex etc. can be used here. --> Web scraping.

2. **Easy Data Augmentation (EDA)** :tractor:

   EDA is a simple and traditional method for data augmentation. Consist of 4 operations.

   - **Synonym Replacement**

     Select a word that is not a stop words and replace it its synonym.

     ```
     lorem ipsum
     ```

     ```
     lorem ipsum
     ```

   - **Random Insertion**

     Find a random synonym of a random word in text date and insert into a random place.

     ```
     lorem ipsum
     ```

     ```
     lorem ipsum
     ```

   - **Random Swap**

     Randomly select 2 words in the text and swap the positions.

     ```
     lorem ipsum
     ```

     ```
     lorem ipsum
     ```

   - **Random Deletion**

     Randomly select n words and remove it.

     ```
     lorem ipsum
     ```

     ```
     lorem ipsum
     ```

3. **NLP Albumentation** :camera:

   If the given text contains multiple sentences then just shuffled them.

   Given text:

   ```
   <Sentence1><Sentence2><Sentence3><Sentence4><Sentence5>
   ```

   Augmented text:

   ```
   <Sentence5><Sentence3><Sentence4><Sentence2><Sentence1>
   ```

4. **NLP Aug Library** :books:

   NLPAug is a library that helps you to implement all the data augmentation methods above on your projects. 



## References

- https://neptune.ai/blog/data-augmentation-nlp
- https://towardsdatascience.com/data-augmentation-in-nlp-2801a34dfc28
- https://github.com/makcedward/nlpaug
