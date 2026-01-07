# Parity

Mukando Digital is a next-generation financial platform designed to formalize and secure traditional informal savings groups (known as Mukando or Round). By blending community trust with high-tech accountability, the app enables groups to save, lend, and grow their wealth with total transparency.

## Description

### Main Purpose
To bridge the gap between informal community finance and formal digital banking. The app eliminates the risks of manual record-keeping, cash theft, and lack of accountability in traditional savings circles.

### Key Features
- **Dynamic Contribution Tracking:**
  Real-time ledgers showing who has paid, who is pending, and the total group "pot" balance.

- **Mobile Money Integration:**
  Direct API hooks for M-Pesa, EcoCash, MoMo, and Airtel Money, allowing one-tap contributions and instant payouts.

- **Automated Loan Engine:**
  - Calculates interest rates based on group-defined rules.
  - Generates amortization schedules for members borrowing from the pool.
  - Auto-deducts repayments from member wallets.

- Target iOS: iOS 26.0+

## Requirements

- Xcode 15.0 or later
- iOS 26.0+
- Swift 5.9+

## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/juss-ron/Parity.git
   cd Parity
   ```

2. **Open the project**
   - Open `Group Investment Tracker.xcodeproj` in Xcode

3. **Build and run**
   - Select your target device or simulator
   - Press `Cmd + R` to build and run the project

## Project Structure

```
Parity/
├── Group Investment Tracker/
├── Group Investment Tracker/
│   ├── Assets.xcassets
│   ├── Logic/
│   │   ├── Models
│   │   │   ├── Club.swift
│   │   │   ├── Member.swift
│   │   │   ├── Response.swift
│   │   │   ├── Transaction.swift
│   │   │   └── User.swift
│   │   ├── Services
│   │   │   ├── AuthService.swift
│   │   │   ├── ClubService.swift
│   │   │   └── MemberService.swift
│   │   ├── Utility
│   │   │   ├── Theme.swift
│   │   │   └── Validator.swift
│   ├── Views/
│   │   ├── AssistantViews/
│   │   │   ├── CreateNewView.swift
│   │   │   ├── LogoView.swift
│   │   │   └── TransactionView.swift
│   │   ├── Authentication/
│   │   │   ├── ForgotPasswordView.swift
│   │   │   ├── ResetPasswordView.swift
│   │   │   ├── SignInView.swift
│   │   │   ├── SignUpView.swift
│   │   │   ├── VerifyEmailView.swift
│   │   │   └── WelcomeView.swift
│   │   ├── Clubs/
│   │   │   ├── ClubView.swift
│   │   │   ├── ClubsView.swift
│   │   │   └── MemberView.swift
│   │   └── ProfileView.swift
│   ├── ContentView.swift
│   └── Group_Investment_TrackerApp.swift
└── .gitignore
```

## Features

- **Multi-Layer Member Verification**:
  Ensures every member of the Mukando is a real person. The app utilizes IdentityKit to scan government IDs and cross-reference them with FaceID biometrics. This builds a "Trust Score" for each group, reducing the risk of fraud or "ghost" members.
  
- **Real-Time Contribution Ledger**:
  A transparent, immutable record of every cent moved within the group.
  - **Visual Progress:** See the "pot" grow with dynamic progress rings.
  - **History:** Exportable PDF/CSV reports for group meetings or auditing purposes.

- **Automated Loan & Interest Engine**:
  Removes the headache of manual math and prevents disputes over interest.
  - **Smart Calculations:** Instantly calculates repayment amounts based on group-defined interest rates (Simple or Compound).
  - **Penalty Logic:** Automatically applies late fees or grace periods according to the group's specific "constitution."
  - **Amortization:** Generates a clear repayment schedule for the borrower to view in their own dashboard.


## Contact

Linked In - [Ron Harifiyati]([https://twitter.com/yourhandle](https://www.linkedin.com/in/ron-harifiyati-723391350/)) - ronshadreck@gmail.com

Project Link: [https://github.com/juss-ron/Parity](https://github.com/juss-ron/Parity)
