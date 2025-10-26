# Database Setup Documentation

## Database Tables

The GamerZone e-commerce website uses Trickle's built-in database with three main tables:

### 1. Product Table
- **Name**: Product name
- **Description**: Product description
- **Category**: Product category
- **Price**: Product price
- **Stock**: Available stock quantity
- **ImageURL**: Product image URL

### 2. Customer Order Table (customer_order)
- **OrderID**: Unique order identifier
- **CustomerName**: Customer's full name
- **Email**: Customer email
- **Phone**: Customer phone number
- **Address**: Full shipping address
- **OrderedProducts**: JSON string of ordered items
- **OrderDate**: Order date in ISO format
- **OrderStatus**: Current status (Processing, Shipped, Delivered, Cancelled)
- **Total**: Order total amount

### 3. Review Table
- **ProductName**: Name of reviewed product
- **ProductID**: Product identifier
- **CustomerName**: Reviewer's name
- **Rating**: Star rating (1-5)
- **Comment**: Review text
- **Date**: Review submission date

## Admin Panel Access

- **URL**: `/admin.html`
- **Default Password**: `admin123`
- **Features**: Product, order, and review management

## Integration

All customer actions (placing orders, submitting reviews) are automatically saved to the database. The admin panel provides full management capabilities.