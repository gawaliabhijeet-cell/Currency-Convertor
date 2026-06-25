# 💱 Currency Converter App

A modern and responsive Currency Converter built with **React.js**, **Custom Hooks**, and **Tailwind CSS**. This application allows users to convert currencies in real-time using live exchange rate data.

## 🚀 Features

* Convert between multiple currencies
* Real-time exchange rates
* Swap currencies with a single click
* Responsive UI using Tailwind CSS
* Custom React Hook for API fetching
* Reusable InputBox component
* Modern glassmorphism design

## 🛠️ Tech Stack

* React.js
* JavaScript (ES6+)
* Tailwind CSS
* Currency API
* Custom Hooks

## 📂 Project Structure

```bash
src/
│
├── components/
│   └── InputBox.jsx
│
├── hooks/
│   └── useCurrencyInfo.js
│
├── App.jsx
│
└── main.jsx
```

## 📸 Application Flow

```text
User enters amount
        ↓
Select source currency
        ↓
Select target currency
        ↓
Click Convert
        ↓
Fetch exchange rate
        ↓
Calculate converted amount
        ↓
Display result
```

## 📸 Preview

![Project Screenshot](./screenshot/one.png)


## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/gawaliabhijeet-cell/Currency-Convertor.git
```

### Navigate to Project Folder

```bash
cd Currency-Converter
```

### Install Dependencies

```bash
npm create vite@latest```


```bash
npm run dev
```

## 🔗 API Used

Currency data is fetched using:

```text
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/
```

Example:

```text
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/usd.json
```

## 🧠 Key Concepts Used

### React Hooks

* useState
* useEffect
* useId
* Custom Hooks

### Custom Hook

`useCurrencyInfo(currency)`

Responsible for:

* Fetching exchange rates
* Managing API calls
* Returning currency data

### Reusable Components

`InputBox`

Handles:

* Amount Input
* Currency Selection
* Callback Functions
* Controlled Components

## 🔄 Currency Conversion Logic

```javascript
const convert = () => {
  setConvertedAmount(amount * currencyInfo[to]);
};
```

Formula:

```text
Converted Amount = Amount × Exchange Rate
```

Example:

```text
100 USD × 83.50
= 8350 INR
```

## 🔁 Swap Functionality

```javascript
const swap = () => {
  setFrom(to);
  setTo(from);
  setConvertedAmount(amount);
  setAmount(convertedAmount);
};
```

Allows users to instantly switch source and target currencies.

## 🎨 UI Features

* Full-screen background image
* Glassmorphism card effect
* Responsive design
* Clean user interface
* Accessible form controls

## 📚 Learning Outcomes

Through this project, I learned:

* React State Management
* Custom Hooks
* API Integration
* Controlled Components
* Component Reusability
* Tailwind CSS Styling
* Event Handling in React

## 👨‍💻 Author

**Abhijeet Gawali**

Frontend Developer | React Learner

## ⭐ Future Improvements

* Currency search feature
* Conversion history
* Dark mode support
* Favorite currencies
* Loading spinner
* Error handling UI


