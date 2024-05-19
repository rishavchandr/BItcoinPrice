# Bitcoin Price

Bitcoin Price is an iOS application that allows users to view the current price of Bitcoin in various currencies. The app fetches data from the CoinAPI.io API and displays it in a user-friendly interface. Users can select different currencies using a UIPickerView.

## Features

- **Real-time Bitcoin Prices:** Fetches and displays the current price of Bitcoin.
- **Multiple Currencies:** Users can select from various currencies to view the Bitcoin price.
- **User-friendly Interface:** Simple and intuitive design for ease of use.

## Screenshot

### Bitcoin Price in Different Currencies
<img src="https://github.com/rishavchandr/BitCoinPrice/assets/110689353/35c6ccdf-d870-4076-b75b-fbb1cbec3d8b" width="200px">

## Installation

### Prerequisites
- Xcode installed on your macOS
- A CoinAPI.io API key (you can get one by signing up on their website)

### Steps

1. **Clone the repository:**
    ```bash
    git clone https://github.com/rishavchandr/BitCoinPrice.git
    cd BitCoinPrice
    ```

2. **Open the project:**
    Open the `.xcworkspace` file in Xcode:
    ```bash
    open BitCoinPrice.xcworkspace
    ```

3. **Configure API Key:**
    Open the project in Xcode, find the file where the API call is made, and replace `YOUR_API_KEY` with your actual CoinAPI.io API key.

4. **Build and run the project:**
    Select the target device or simulator in Xcode and press `Command + R` to build and run the app.

## Usage

1. **Select a Currency:**
   - Open the app and use the UIPickerView to select the desired currency.
   
2. **View Bitcoin Price:**
   - The app will display the current price of Bitcoin in the selected currency.

## Implementation Details

### Fetching Bitcoin Prices
- The app uses the CoinAPI.io API to fetch real-time Bitcoin prices. 
- An HTTP GET request is made to the API endpoint with the selected currency.

### UIPickerView for Currency Selection
- A UIPickerView is used to allow users to select different currencies.
- The selected currency is used to fetch the corresponding Bitcoin price from the API.

### Storing API Key
- The API key should be securely stored and not hardcoded in the source code for security reasons. Consider using secure storage mechanisms provided by iOS.
