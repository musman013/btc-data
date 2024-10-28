# Real-Time Cryptocurrency Trading App

This project is a real-time cryptocurrency trading application, providing live trade data streamed from the Binance WebSocket API. Built with NestJS for the backend and React.js with Chart.js for the frontend, the app visualizes BTC/USDT trading data on an interactive line chart.

## Features

- **Real-Time Trade Data:** Stream live BTC/USDT trade data from Binance’s WebSocket API.
- **Interactive Chart:** Visualize trade price data on a dynamically updating line chart with Chart.js.
- **Modular Code Structure:** Uses best practices and a clean folder structure in both frontend and backend.
- **Responsive UI:** A polished, responsive UI built with React and CSS.

## Tech Stack

- **Backend:** [NestJS](https://nestjs.com/), [Socket.io](https://socket.io/), [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket)
- **Frontend:** [React.js](https://reactjs.org/), [Chart.js](https://www.chartjs.org/), [Socket.io-client](https://www.npmjs.com/package/socket.io-client)

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Yarn](https://classic.yarnpkg.com/en/docs/install/) or npm

### Setup Instructions

#### Backend (NestJS)

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/Ali-web-0/task.git
    cd task
    ```

2. **Navigate to the Backend Directory**:
    ```bash
    cd backend
    ```

3. **Install Dependencies**:
    ```bash
    npm install
    ```

4. **Run the Backend Server**:
    ```bash
    npm run start:dev
    ```
    The NestJS server should be running at `http://localhost:3200`.

#### Frontend (React)

1. **Navigate to the Frontend Directory**:
    ```bash
    cd frontend
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

3. **Run the Frontend Server**:
    ```bash
    npm start
    ```
    The React app should be running at `http://localhost:3000`.

---

## Usage

1. Start the backend server to establish a WebSocket connection to Binance and enable real-time trade data streaming.
2. Start the frontend server to display the data in a live-updating line chart.
3. Open `http://localhost:3000` to view the real-time trading data and chart.

---

## Code Structure

### Backend (NestJS)

- **Gateway (`BinanceGateway`)**: Establishes a WebSocket connection to Binance, streams BTC/USDT trade data, and emits it to connected clients.
- **Error Handling & Reconnect**: Reconnects automatically if the connection to Binance drops.

### Frontend (React)

- **Socket Connection**: Connects to the backend WebSocket server and listens for incoming trade data.
- **Chart Integration**: Uses Chart.js to display live BTC/USDT prices on a line chart.
- **Dynamic UI Updates**: Renders real-time trade price and time labels on the chart.

---

### Deployment

frontend deploy on vercel 
and backned deploy on koyeb
Live Demo Link
  ```bash
    https://task-frontend-khaki.vercel.app/
    