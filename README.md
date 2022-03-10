# Intent Evaluation samples

#### Scripts
- The intents you want to eval should be in a file named `statements.csv`. Alternately, you can change the name of the file in `intent_prediction.py`. Each statement to be evaluated should be on its own line (if you're using Excel, its own row).
- Change `api_string` to the string for your environment. For more details, refer to the [Rasa API spec](https://rasa.com/docs/rasa/pages/http-api).
- Check the API spec to find other data you want to include in your report, and make sure to add a heading for it and account for the data to be written. (Follow the comments in the file.)

#### Config
For your evaluation, select the proper pipeline components. The attached `config.yml` file is the default natural language pipeline configuration in Rasa.

#### Credentials
To successfully use this script, make sure you've turned on your REST endpoint in Rasa. Simply uncomment the line for `rest:` to make the endpoint available.
