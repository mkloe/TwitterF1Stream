# TwitterF1Stream

## Project Description
#### Business objective 
- The goal is to select the driver of the day during Formula 1 race. 
- The driver of the day is a F1 driver whose name was mentioned the most times in tweets including a hashtag #F1DriverOfTheDay during a F1 race.

#### How it works (on a high level)?
- In the project one can configure what tweet topics should be streamed via the Twitter Streaming API. 
- The tweets are streamed to a port on a localhost. 
- Spark collects tweets from the localhost and processes in real-time to extract only relevant data (e.g., filters certain hashtags etc.). 
- The results are visualized on charts.

## How to run the project?
1. Open `twitter_data_streaming.ipynb` and run the code blocks.
2. Open `spark_processing.ipynb` and run the code blocks 1-4.
3. Wait until you collect enough data and stop the kernel.
4. Run rest of cells `spark_processing.ipynb` for data visualisation.
4. You can also change request params for twitter API endpoints in `Twitter_Setup.ipynb`.

## More information
- It is a university project. 
- My part was Twitter API, streaming on the localhost, and basic real-time processing of tweets with PySpark. 
- My colleagues did real-time saving into CSV file and charts.
- Our work was partially based on https://www.toptal.com/apache/apache-spark-streaming-twitter.
