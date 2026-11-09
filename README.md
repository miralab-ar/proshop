# Proshop — demo e-commerce store

**Live Demo:** [https://proshop-rosy.vercel.app](https://proshop-rosy.vercel.app)

Proshop is a **demonstration project** by [Miralab](https://miralab.ar): a full e-commerce flow (catalog, cart, checkout, admin panel) built to showcase architecture and user experience. It is not a real store — products, prices and contact details are sample data.

## 🚀 Tech Stack

- **Frontend**: [Next.js 16](https://nextjs.org/) (App Router), [React 19](https://react.dev/), [Redux](https://redux.js.org/) with React Redux and Redux Thunk
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: Bootstrap 5, React Bootstrap, CSS
- **Backend**: Next.js API Routes (Serverless)
- **Database**: [MongoDB](https://www.mongodb.com/) with Mongoose ODM
- **Auth & validation**: JWT, bcryptjs, Zod
- **Payments**: [PayPal](https://developer.paypal.com/) (`@paypal/react-paypal-js`)
- **Image uploads**: Cloudinary
- **Internationalization**: next-intl (EN/ES/IT)
- **Testing**: Jest, Testing Library

## ✨ Features

### 🛍️ User Features

- **Smart Search**: Predictive search bar with typeahead suggestions and debounce.
- **Advanced Filtering**: Dynamic Sidebar with Price Range, Category, Brand, and Rating filters.
- **Product Gallery**: High-definition interactive gallery with hover zoom and thumbnail navigation.
- **Related Products**: Intelligent suggestions of similar items on product detail pages.
- **Wishlist**: Save favorite products for later (Persistent local storage).
- **Shopping Cart**: Real-time cart management with instant updates.
- **Guest Checkout**: Seamless purchasing experience without mandatory registration.
- **Checkout**: Multi-step process (Shipping, Payment, Confirmation) with PayPal (PayPal balance or card).
- **Newsletter**: Email subscription form in the footer.
- **User Accounts**: Full authentication system (Login/Register) with profile management.
- **Order History**: Track past orders and view payment status.
- **Ratings**: Star rating and review count on each product.
- **Multilingual**: Interface available in English, Spanish and Italian.
- **Light/Dark theme**: Theme toggle in the header.

### 🛡️ Admin Features

- **User Management**: View, edit, and delete users.
- **Product Management**: Create, update, and delete products, with image upload.
- **Order Management**: Mark paid orders as delivered.
- **Secure Access**: Protected routes for admin-only operations.

### 💳 Payment Integration

- **PayPal**: Checkout using `@paypal/react-paypal-js`. It is the only payment method integrated; without a `PAYPAL_CLIENT_ID` the app falls back to PayPal's sandbox client.

## 🛠️ Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
MONGO_URI=<your_mongodb_connection_string>
JWT_SECRET=<your_jwt_secret>
PAYPAL_CLIENT_ID=<your_paypal_client_id>
CLOUDINARY_CLOUD_NAME=<your_cloudinary_cloud_name>
CLOUDINARY_API_KEY=<your_cloudinary_api_key>
CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>
```

## 📦 Installation & Run

1. **Clone the repository**

   ```bash
   git clone https://github.com/miralab-ar/proshop.git
   cd proshop
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Run the development server**

   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000).

## 📄 License

© Miralab. All rights reserved.
