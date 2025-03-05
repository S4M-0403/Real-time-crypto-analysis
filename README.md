# README - Fetching and Analyzing Top 50 Live Cryptocurrency Data

## Project Overview
This project is designed to fetch, analyze, and store real-time cryptocurrency market data. The script retrieves the top 50 cryptocurrencies by market cap, processes their price trends, and saves the data into an Excel file for further analysis.

## Features
- Fetches real-time cryptocurrency data.
- Analyzes price trends and stores insights.
- Saves data periodically in an Excel file (`Live_Crypto_Data.xlsx`).
- Implements robust file-handling techniques to prevent errors.

## Installation & Setup
1. **Clone the Repository:**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```
2. **Install Dependencies:**
   ```sh
   pip install -r requirements.txt
   ```
3. **Run the Script:**
   ```sh
   python crypto.py
   ```

## Challenges & Solutions
### File Access Issues
- **Issue:** The script encounters errors when trying to update the Excel file while it is open.
- **Solution:** Ensure the file is closed before running the script.

### File Overwriting Conflicts
- **Solution:** Save the file with a unique timestamp (`Live_Crypto_Data_YYYYMMDD_HHMMSS.xlsx`).

### File Locking
- **Solution:** Implement `try-except` handling to manage locked files gracefully and notify the user.

## Testing & Results
- Manual closure of the file before execution resolved access issues.
- Timestamp-based file saving allowed better data tracking.
- Implementing file lock handling improved script reliability.

## Conclusion
This project demonstrates efficient cryptocurrency data collection and storage, integrating best practices for file management. Future improvements could include database integration and automated reporting.

## Author
Shikhar Maheshwari

## License
[Specify license, e.g., MIT, Apache, etc.]

