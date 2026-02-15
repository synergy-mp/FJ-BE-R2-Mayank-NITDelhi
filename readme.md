⚡ SatoshiTrack: Bitcoin Portfolio & Budget Manager
A full-stack financial tool designed for the Bitcoin standard.

SatoshiTrack is not just a finance tracker; it is a Bitcoin-native portfolio manager that allows users to track their net worth in Satoshis (sats), audit real-time on-chain balances, and set budget alerts based on live market data.

Built with Node.js, PostgreSQL, and Prisma, this project demonstrates integration with the Bitcoin ecosystem via real-time blockchain APIs.

🚀 Live Demo
https://fj-be-r2-mayank-nitdelhi.onrender.com
(Note: Please allow ~30 seconds for the initial load as the free instance spins up.)

₿ Summer of Bitcoin Features
Designed specifically to demonstrate competency with Bitcoin data structures and APIs.
⚡ Live Sats Conversion: The application fetches the real-time Bitcoin price via the CoinGecko API and dynamically converts all fiat entries (USD, INR, EUR) into Satoshis.

⛓️ On-Chain Audit (Watch-Only Wallet): Users can paste any public Bitcoin address (e.g., bc1q...). The app queries the Mempool.space API to verify the address's confirmed on-chain balance and integrates it into the user's total net worth.
📉 Sats-Denominated Budgeting: Budget goals can be set in fiat, but the tracking and visualizations reflect the user's standing in the Bitcoin economy.

✨ Standard Features
🔐 Secure Authentication: Google OAuth 2.0 implementation (Passport.js) for secure, password-less login.
📧 Automated Budget Alerts: Uses Nodemailer to send instant email notifications when spending exceeds defined limits.
📊 Visual Analytics: Interactive Chart.js dashboards to visualize Income vs. Expenses.
🧾 Receipt Management: Image upload functionality (Multer) to attach proof-of-payment to transactions.
🌍 Multi-Currency Support: Seamless toggling between USD, INR, EUR, and SATS.

🛠️ Tech Stack
Backend
Runtime: Node.js & Express.js
Database: PostgreSQL (Hosted on Neon)
ORM: Prisma
Bitcoin Data: CoinGecko API (Price), Mempool.space API (On-Chain Data)
Email Service: Nodemailer (SMTP)
Frontend
UI: Semantic HTML5, CSS Grid, Vanilla JavaScript
Charts: Chart.js
DevOps
Deployment: Render
Version Control: Git & GitHub
⚙️ Local Installation & Setup
Follow these steps to run the project locally on your machine.

1. Clone the Repository
Bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
2. Install Dependencies
Bash
npm install
3. Configure Environment Variables
Create a .env file in the root directory and add the following keys:

Code snippet
# Database Connection (PostgreSQL)
DATABASE_URL="postgresql://user:password@host:port/database"

# Google OAuth 2.0 Credentials
GOOGLE_CLIENT_ID="your_google_client_id"
GOOGLE_CLIENT_SECRET="your_google_client_secret"
SESSION_SECRET="your_random_secret_string"

# Nodemailer (Gmail App Password)
EMAIL_USER="your_email@gmail.com"
EMAIL_PASS="your_16_char_app_password"
4. Initialize Database
Push the Prisma schema to your database:

Bash
npx prisma db push
npx prisma generate
5. Run the Server
Bash
node server.js
Visit http://localhost:3000 in your browser.

📡 API Integrations
This project relies on the following public APIs:
CoinGecko API: Used to fetch the live bitcoin price in usd, inr, and eur.
Mempool.space API: Used to fetch chain_stats and mempool_stats for public Bitcoin addresses.

👨‍💻 Author
Mayank Prakash  
Role: Full Stack Developer & Bitcoin Enthusiast
GitHub: https://github.com/synergy-mp
LinkedIn: https://www.linkedin.com/in/mayank-prakash-1a2737323/
📝 License
This project is open-source and available under the MIT License.