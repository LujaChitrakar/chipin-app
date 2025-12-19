# Chipin

A modern, intuitive mobile application for expense splitting and peer-to-peer USDC payments built with React Native and Expo.

## Overview

The social wallet that makes shared spending effortless with ChipIn.
You and your friends can easily manage shared costs, split your bills, track your expenses and settle instantly all in one place.  
You can stay connected, track every expense together, and move money globally without the limits or fees of traditional payment.
How chipin works is 
You can create groups instantly, add your friends, add your expenses and settle them seemlessly.
You can add your friends and transfer money to them with just few taps track all your expenses and never worry about unpaid settlements.

### Friend Management
**Discovering & Adding Friends:**

**Method 1 - Search & Request:**
- Users can search for friends by username or email
- Receipent Can accept or reject from notifications or friends tab

**Method 2 - QR Code (Preferred):**
- Each user has a unique QR code in their profile
- Other users open camera scanner from friends tab
- Scan QR code → instant friend request sent
- No typing needed, works great for in-person connections

**Managing Friends:**
- Friends list shows all connections with recent activity
- Tap friend to view profile, transaction history
- Option to unfriend or view mutual groups
- See pending requests (sent and received)

**Flow:**
1. User A taps "Add Friend" button
2. Options appear: "Scan QR Code" or "Search"
3. User A selects "Scan QR Code"
4. Camera opens with scanner overlay
5. User A scans User B's QR code from their profile
6. Friend request automatically sent to User B
7. User B receives push notification
8. User B opens notifications, sees request from User A
9. User B taps "Accept" → both are now friends
10. Both users see each other in friends list

### Expense Tracking & Settlement

**Adding Expenses:**
- From group screen, tap "Add Expense"
- Enter description (e.g., "Groceries")
- Enter total amount
- Select who paid (defaults to you)
- Select participants who should split the cost
 to each person
- Tap "Add" → expense is recorded

**Settling Balances:**
- Tap "Settle" on balance tab
- Transaction is broadcast to Solana
- Balance updates to $0 for that person
- Settlement is recorded in activity history

**Flow:**
1. Group of 4 friends goes to dinner, bill is $100
2. User A pays the full $100 bill
3. User A opens Chippin, navigates to "Dinner Group"
4. Taps "Add Expense"
5. Enters: "Dinner at Italian Place", $100
6. Splits equally among all 4
7. System calculates: User B, C, D each owe $25
8. User B opens app, sees "You owe $25" on group screen
9. User B taps "Settle Up" → selects User A
12. Transaction processes on Solana blockchain
13. Both are displayed "Settled"
14. Group balance updates: User C and D still owe $25 each

### Direct Payments

**Sending Money to Friends:**
- Navigate to Home page
- Click on Send button
- Enter amount in USDC
- Add optional purpose
- Click Send and Done

**QR Code Payment:**
- Tap "Send By QR"
- Camera opens with QR scanner
- Scan friend's or merchant's wallet QR code
- App decodes wallet address
- Enter amount and confirm
- Transaction is sent

**Manual Address Entry:**
- Tap "Send Direct" and "Public Key"
- Paste or type Solana wallet address
- App validates address format
- Enter amount and confirm
- Useful for sending to external wallets

### Lending & Borrowing

**Lending Money (Direct):**
- Navigate to Lending tab
- Tap "Lend Money"
- Select friend from list
- Enter amount
- Optional: enter purpose
- Confirm → USDC is sent immediately
- Loan is tracked in "Money Lent" section
- Friend sees it in their "Money Borrowed" section

**Borrowing Money (Request):**
- Navigate to Lending tab
- Tap "Request to Borrow"
- Select friend you want to borrow from
- Enter amount needed
- Add reason/purpose (required)
- Optional: suggest repayment date
- Send request
- Friend receives notification with request details
- Friend can accept (sends USDC) or reject with message
  
### Rewards & Referrals

**Accessing Referral Code:**
- Navigate to Profile tab
- Tap "Rewards & Referrals"
- View your unique referral code and QR code
- See current points balance
- View progress to next cashback milestone

**Sharing Referrals:**
- Tap "Share Referral" button
- Options: Share QR code image, Copy referral code, Share via social media
- When friend signs up and enter the code
- Points are awarded to both.

### Activity Feed

**Real-Time Activity Tracking:**
- Home screen shows recent activities at the top
- Dedicated Activities tab for complete history
- Activities auto-refresh when new actions occur
- Push notifications for important activities

**Activity Details:**
- Tap any activity to view full details
- See transaction hash for blockchain transactions
- View related group or friend profile
- Access related receipts or photos

## Installation & Setup

```bash
# Install dependencies
npm install

# Start development server
npm start

# Run on iOS simulator
npm run ios

# Run on Android emulator
npm run android
```

## Platform Support

- **Android**: API level 21 (Android 5.0) and above


## License

MIT License

## Support

For help or questions: chipinsolana@gmail.com
