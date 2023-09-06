
#### Overview

This project focuses on predicting stock prices based on historical data. The dataset consists of real stock prices for each working day from the end of 2015 to the end of 2019. Four variables influence the prediction: stock price, oil price, gold price, and the Euro to Dollar exchange rate.

---

#### Procedure

1. **Data Preprocessing**: The initial steps involve reformatting the data for ease of analysis. The "Date" column is converted into a datetime format and set as the index. This process facilitates efficient manipulation of time-based data. The training and test sets are selected in this step, with the test set comprising 20% of the total data.

2. **Data Cleaning**: The dataset contains several missing values, which need to be addressed before modeling. The missing values are interpolated to preserve the time-based structure of the data, providing a more accurate representation of underlying patterns.

3. **Model Construction**: A Recurrent Neural Network (RNN) is employed for predictions. RNNs are particularly suitable for time-series data as they have memory units that allow them to remember and process sequences of data, making them ideal for predicting stock prices based on historical data.

4. **Model Testing**: The constructed model is evaluated on the test set. The performance metrics, such as accuracy, help determine the effectiveness of the model in predicting stock prices.

---

#### Deep Learning Methods Employed

- **Recurrent Neural Network (RNN)**: RNNs are a class of neural networks designed for sequential data. They maintain a memory of previous inputs, making them adept at tasks like time-series forecasting. In the context of stock prediction, RNNs can capture patterns over time, allowing for more accurate predictions.

- **Attention Mechanism**: In addition to RNNs, attention mechanisms are explored. Attention allows the model to focus on specific parts of the input sequence when producing an output, enhancing the model's capability to capture crucial patterns in the data.

---

#### Benefits of Employed Methods

1. **RNNs**: RNNs can model sequential data effectively, making them ideal for time-series predictions like stock prices. Their ability to remember past inputs enables them to identify patterns in historical stock prices and use this knowledge for future predictions.

2. **Attention Mechanism**: Attention mechanisms enhance the model's capacity by enabling it to focus on the most relevant parts of the input data. This capability can lead to more accurate predictions, especially when the input sequences are long.

---

#### Conclusion

The project showcases the application of deep learning methods, particularly RNNs and attention mechanisms, in predicting stock prices. Through data preprocessing, cleaning, modeling, and testing, we can derive insights into stock price movements and develop models that can potentially guide investment decisions.

---

### Sentiment Analysis Section:
---

#### Overview

In the latter part of the project, a sentiment analysis model is constructed to predict the sentiment of film reviews from the IMDB dataset. The sentiment can be either positive or negative. The model's accuracy is evaluated based on its ability to correctly classify the sentiment of the reviews.

---

#### Procedure

1. **Data Formatting**: Two hyperparameters, maximum review length and dictionary size, format the data from IMDB. These parameters influence the quality and shape of the input data for the model.

2. **Model Construction with Attention**: The primary deep learning method employed here is the attention mechanism. The attention mechanism is applied to the IMDB review data without any recurrent components, focusing solely on attention layers. Restrictions are imposed on the type of Keras layers that can be used to ensure the model's simplicity and focus on attention.

---

#### Deep Learning Methods Employed

- **Attention Mechanism**: The attention mechanism allows the model to focus on specific parts of the input text, giving weight to words or sequences that are more informative for sentiment classification. In the context of sentiment analysis, attention can capture the nuances and emphases in the reviews, leading to more accurate sentiment predictions.

---

#### Benefits of the Attention Mechanism in Sentiment Analysis

1. **Selective Focus**: Attention allows the model to prioritize specific parts of the review text that are more indicative of the overall sentiment. This selective focus can improve model accuracy by giving more weight to the most influential words or phrases in the text.

2. **Handling of Long Sequences**: Reviews can be lengthy, and not every part of the text is equally relevant for sentiment prediction. The attention mechanism can effectively handle such long sequences by focusing on the most salient parts.

---

#### Conclusion

The sentiment analysis model, with its emphasis on the attention mechanism, showcases another application of deep learning in natural language processing. By capturing the nuances in film reviews, the model aims to predict sentiments with high accuracy. However, it's important to note that while the attention model achieved decent accuracy, it did not outperform the original RNN model in terms of accuracy on both the training and test sets.
