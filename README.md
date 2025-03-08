# RT/RW Net Billing Management System

A comprehensive platform for managing network customer billing, payments, and notifications for RT/RW Net providers.

![Dashboard Preview](payment.jpeg)

## 🚀 Features

- **Customer Management**
  - Add, edit, and manage customer profiles
  - Track active/inactive status
  - View customer details and billing history
  - Package and speed management

- **Billing System**
  - Generate monthly bills automatically
  - Track payment status
  - Payment history tracking
  - Overdue payment monitoring

- **Reports & Analytics**
  - Monthly revenue overview
  - Payment history reports
  - Overdue payment reports
  - Export reports to CSV

- **Dashboard**
  - Real-time statistics
  - Revenue visualization
  - Quick overdue payment alerts
  - Customer activity monitoring

## 💻 Tech Stack

- **Frontend**: React.js with TypeScript
- **UI Components**: shadcn/ui + Tailwind CSS
- **Backend**: Express.js
- **Database**: PostgreSQL
- **State Management**: TanStack Query
- **Charts**: Recharts
- **Forms**: React Hook Form + Zod

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/rtrw-net.git
cd rtrw-net
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```

4. Start the development server:
```bash
npm run dev
```

## 📝 Environment Variables

```env
DATABASE_URL=postgresql://user:password@localhost:5432/rtrw_net
PORT=5000
```

## 🎯 Usage

### Customer Management
1. Navigate to the Customers page
2. Click "Add Customer" to create new customer profiles
3. Use the search and filter options to find specific customers
4. Click the view/edit/delete buttons to manage customer records

### Billing
1. Go to the Billing page
2. Use "Generate Monthly Bills" to create bills for all active customers
3. Mark bills as paid when payment is received
4. Filter and search bills by status or customer name

### Reports
1. Access the Reports page
2. Choose between Payment History or Overdue Reports
3. Use the search functionality to filter results
4. Export reports to CSV for external analysis

## 📊 Database Schema

### Customers Table
- id (Primary Key)
- name
- address
- phone
- packageName
- packageSpeed
- monthlyFee
- isActive

### Bills Table
- id (Primary Key)
- customerId (Foreign Key)
- amount
- dueDate
- isPaid
- paidAt
- period

## 👥 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [shadcn/ui](https://ui.shadcn.com/) for the beautiful UI components
- [TanStack Query](https://tanstack.com/query/latest) for data fetching
- [Recharts](https://recharts.org/) for the charts
- All contributors who have helped this project grow
- Jika butuh repo ini silahkan email : habizinnia@gmail.com
