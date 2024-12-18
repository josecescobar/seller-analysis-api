# Seller Analysis API

A robust backend API for Amazon seller analysis and product research. This API helps sellers make data-driven decisions by providing product analysis, fee calculations, and market insights.

## Features

- Product search and analysis
- FBA fee calculation
- Profit margin analysis
- Market competition insights
- User authentication
- Historical price tracking

## Tech Stack

- Node.js
- Express.js
- MongoDB
- JWT Authentication

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- Amazon MWS credentials

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/josecescobar/seller-analysis-api.git
cd seller-analysis-api
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory:
```env
PORT=5000
NODE_ENV=development
MONGO_URI=mongodb://localhost:27017/seller_analysis
AMAZON_API_KEY=your_amazon_api_key
AMAZON_SECRET_KEY=your_amazon_secret_key
JWT_SECRET=your_jwt_secret
```

4. Start the development server:
```bash
npm run dev
```

## API Endpoints

### Products
- `GET /api/products/search/:asin` - Search for a product by ASIN
- `GET /api/products/:asin` - Get detailed product information

### Analysis
- `POST /api/analysis/calculate` - Calculate fees and profitability

### Users
- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - User login

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details