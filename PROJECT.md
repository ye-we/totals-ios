# Totals

## What is Totals?

Totals is a personal finance app built specifically for Ethiopian bank users. It automatically reads your bank SMS notifications and turns them into a clear, organized view of your money, across all your banks, in one place.

In Ethiopia, every bank transaction triggers an SMS: deposits, withdrawals, transfers, payments, mobile money. Totals captures these messages, understands them, and builds your complete financial picture without you typing a single number.

## The Problem

Ethiopian banks don't talk to each other. If you have accounts at CBE, Awash, and Telebirr (which most people do), there's no way to see your total balance or track where your money is going. Each bank's app — if it even has one — only shows its own data. International finance apps don't support Ethiopian banks at all.

The only universal record of your transactions is SMS. Every bank sends them. Totals uses that.

## How It Works

### Android

The Android app runs in the background and listens for incoming bank SMS messages. When one arrives, it automatically parses it, extracts the transaction details, and adds it to your history. You don't need to do anything — open the app and your finances are there.

### iOS

Apple doesn't let apps read SMS directly. Totals works around this using iOS Shortcuts — Apple's built-in automation system. When a bank SMS arrives, a Shortcut fires, parses the message, and saves the transaction to iCloud Drive. The Totals app reads from there and presents the same full dashboard experience.

Setup requires a one-time configuration of these Shortcuts, but once done, everything is automatic.

## Supported Banks

Totals supports the major Ethiopian banks and mobile money services:

- **Commercial Bank of Ethiopia (CBE)** — Ethiopia's largest bank
- **Awash Bank**
- **Bank of Abyssinia (BOA)**
- **Dashen Bank**
- **Zemen Bank**
- **Nib Bank**
- **Amhara Bank**
- **Telebirr** — Ethio Telecom's mobile money (transfers, deposits, agent transactions, airtime)
- **M-Pesa** — Safaricom's mobile money

Each bank has multiple SMS formats for different transaction types. Totals recognizes all of them — transfers in and out, deposits, withdrawals, agent transactions, airtime purchases, fee deductions, and more.

## What You Can Do

### See Everything in One Place

Your total balance across all banks. Today's spending. This week's income. Recent transactions. Charts showing where your money goes. All on one screen, updated automatically.

### Track Every Transaction

Every parsed SMS becomes a searchable, filterable transaction record. Filter by bank, account, date range, income or expense, or category. Search by receiver name, reference number, or amount.

### Organize with Categories

Tag transactions as Food, Transport, Rent, Salary, or anything you want. Create your own custom categories. Set up rules to auto-categorize — for example, every transfer to a specific person automatically tagged as "Rent."

### Budget Your Money

A full budgeting system inspired by YNAB (You Need A Budget). Create category groups like Needs, Wants, and Savings. Assign amounts each month. Track how you're doing with progress indicators and spending pace. Budgets can recur monthly or be one-time.

### Manage Multiple Accounts

Add and name your accounts across all your banks. Group them into profiles — maybe "Personal" and "Business" — and switch between views. Each bank shows its own balance, accounts, and transaction history.

### Share Account Details

Generate a QR code containing your bank account details. Someone else with Totals can scan it to save your accounts to their contacts — useful when you need to share account numbers with friends or family. No more typing long account numbers or sending them over chat.

### Tools

- **Contacts** — Save bank account details of people you frequently transact with. Import from QR codes or add manually. Search, edit, delete.
- **SMS Parser** — Manually paste a bank SMS that wasn't automatically captured. The app parses it and lets you save the transaction.
- **Failed Messages** — Review SMS messages that couldn't be parsed. Retry them after pattern updates, or dismiss ones that aren't real transactions.
- **Payment Verifier** — Look up a transaction by its reference number to verify it exists.

### Analytics & Charts

Visual breakdowns of your spending: by bank, by category, over time. Income vs. expense comparisons. See trends and understand your financial habits at a glance.

## Privacy

- **Everything stays on your phone.** There are no servers, no cloud accounts, no sign-ups.
- **No internet required.** The app works completely offline.
- **SMS parsing is local.** Your messages are never sent anywhere.
- **No tracking.** No analytics, no telemetry, no ads.
- **Account numbers are masked** in the display for security.

Your financial data is yours alone.

## Technical Details

- **Android**: Built with Flutter
- **iOS**: Built as a Scriptable script with a web-based dashboard, using iOS Shortcuts for SMS automation
- **Data storage**: Plain text files (JSON lines format) stored locally on Android, in iCloud Drive on iOS
- **Currency**: Ethiopian Birr (ETB)
- **Themes**: Dark mode, light mode, or follow system preference

## What Makes Totals Different

**It's built for Ethiopia.** Not a Silicon Valley finance app with Ethiopian support as an afterthought. Every feature — from the SMS parsing to the bank list to the currency formatting — is designed around how Ethiopian banking actually works.

**It's automatic.** No manual entry. Your transactions appear as they happen.

**It's multi-bank.** One app, all your banks, one complete picture.

**It's private.** No servers, no accounts, no data leaving your device.

**It's free.** No subscription, no premium features behind a paywall, no ads.
