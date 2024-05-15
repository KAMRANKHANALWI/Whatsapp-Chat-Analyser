## WhatsApp Chat Analyzer

This project is a simple web app to analyze your WhatsApp chat data. It gives you various insights and visualizations about your chat habits.

### Features

- **Upload WhatsApp Chat Data:** Easily upload your chat file.
- **See Chat Statistics:** View the total number of messages, words, media files, and links shared.
- **Monthly and Daily Activity:** See your chat activity over time.
- **Word Cloud:** Visualize the most frequently used words.
- **Most Common Words:** Find out which words you use the most.
- **Emoji Analysis:** See which emojis you use the most.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/KAMRANKHANALWI/whatsapp-chat-analyzer.git
   cd whatsapp-chat-analyzer
   ```

2. **Create and activate virtual environment (MAC):**
```bash
python3 -m venv venv
source venv/bin/activate 
```

3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

### How to Use

1. **Run the app:**
   ```bash
   streamlit run app.py
   ```

2. **Upload Your Chat File:**
   - Export your WhatsApp chat as a `.txt` file from the app.
   - Upload this file using the sidebar in the web app.

3. **View the Analysis:**
   - Choose a specific user or "Overall" to analyze the entire chat.
   - Click "Show Analysis" to see various stats and visualizations.

### Folder Structure

- **app.py:** Main script to run the Streamlit app.
- **preprocessor.py:** Functions to clean and prepare chat data.
- **helper.py:** Functions to generate statistics and visualizations.
- **requirements.txt:** List of Python packages needed for the app.

### Main Functions

#### preprocessor.py
- `preprocess(data)`: Cleans and formats the raw chat data.

#### helper.py
- `fetch_stats(selected_user, df)`: Gets total messages, words, media files, and links.
- `monthly_timeline(selected_user, df)`: Shows monthly message trends.
- `daily_timeline(selected_user, df)`: Shows daily message trends.
- `week_activity_map(selected_user, df)`: Shows activity by day of the week.
- `month_activity_map(selected_user, df)`: Shows activity by month.
- `create_wordcloud(selected_user, df)`: Creates a word cloud of frequently used words.
- `most_common_words(selected_user, df)`: Lists the most common words.
- `emoji_helper(selected_user, df)`: Analyzes and lists the most used emojis.

### Example

1. Export your WhatsApp chat as a `.txt` file.
2. Run the Streamlit app.
3. Upload the chat file in the sidebar.
4. Select a user or "Overall" for group analysis.
5. Click "Show Analysis" to view the results.

### Contributing

If you find any issues or have suggestions, feel free to create an issue or pull request.

