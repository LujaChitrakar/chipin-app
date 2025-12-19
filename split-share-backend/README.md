# Chippin Backend

The social wallet that makes shared spending effortless with ChipIn. 
You and your friends can easily manage shared costs, split your bills, track your expenses and settle instantly all in one place.
You can stay connected, track every expense together, and move money globally without the limits or fees of traditional payment. 
How chipin works is You can create groups instantly, add your friends, add your expenses and settle them seemlessly. 
You can add your friends and transfer money to them with just few taps track all your expenses and never worry about unpaid settlements.

---

### Authentication Flow
Users authenticate through Privy, which handles wallet connection and user identity. Upon successful authentication, users receive a JWT token for subsequent API requests. The authentication system supports multiple wallet types and ensures secure access to all platform features.

---

### Friend Management System

**Adding Friends:**
- **Friend Requests**: Users can search for other users and send friend requests
- **QR Code Scanning**: Each user has a unique QR code that encodes their user ID. Other users can scan this QR code to instantly send a friend request
- **Request Management**: Users receive notifications for incoming friend requests and can accept or reject them
- **Friends List**: Once accepted, friends appear in the user's friends list for easy access

---

### Group Management System

**Creating & Managing Groups:**
- Users can create expense groups with custom names and descriptions
- Group creator automatically becomes the admin
- Each group gets a unique group code and QR code for easy joining

**Adding Members:**
- **Direct Addition**: Group admins can add existing friends directly to the group
- **Email Invitation**: Admins can invite users via email, even if they're not on the platform yet
- **QR/Code Join**: Users can join groups by scanning the group QR code or entering the group code manually

---

### Expense Tracking & Settlement

**Adding Expenses:**
- Users add expenses to groups with description, amount, and date
- Expenses can be split equally or with custom amounts among selected members
- The system automatically calculates who paid and who owes

**Smart Balance Calculation:**
- The app maintains a balance sheet for each group
- It calculates the optimal settlement path (who owes whom)
- Balances are updated in real-time as expenses are added

**In-App Settlement:**
- Instead of external payments, users can settle balances directly within Chippin
- Settlement is done using USDC on Solana blockchain
- Once settled, group balances are updated and marked as paid

---

### Payment System

**Friend-to-Friend Payments:**
- Users can send USDC directly to friends without knowing their wallet address

**QR Code Payments:**
- For non-friends or quick payments, users can scan a wallet address QR code

**Manual Address Entry:**
- Users can manually enter a Solana wallet address

---

### Lending & Borrowing System

**Lending Money:**
- Direct and straightforward process
- Lender selects a friend, enters amount, and sends the loan

**Borrowing Money:**
- Borrower sends a borrow request with amount and reason
- Lender can accept (sends USDC) or reject the request

**Tracking:**
- Dashboard shows all active loans/borrows
- Payment reminders can be set for overdue amounts

---

### Rewards & Referral System

**Points Program:**
- Users earn points through various activities (primarily referrals)
- Points balance is tracked in the user's profile
- Progress bar shows distance to next cashback milestone

**Referral System:**
- Each user gets a unique referral code and QR code
- New users can sign up using a referral code or scanning QR.

---

### Activity Tracking

**Comprehensive Activity Feed:**
- All user actions are logged: expenses added, payments sent, friend requests, group joins, etc.
- Activities are timestamped and categorized
- Users can view their complete transaction history
- Activities include: transaction type, amount, involved parties, and status

**Activity Types Tracked:**
- Expense additions and updates
- Payment transactions (sent/received)
- Friend requests (sent/accepted/rejected)
- Group creations and joins
- Lending and borrowing activities
- Settlements and repayments
- Referral sign-ups
- Cashback earnings

---

## Installation & Setup

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Start production server
npm start
```

---

## Support

For issues or questions, contact: chipinsolana@gmail.com
