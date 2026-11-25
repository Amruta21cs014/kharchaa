# Kharcha – private money tracker for two

Your data never leaves your phones. No server, no login, no analytics.

## Put it online (free, 5 min) – GitHub Pages
1. Create a new GitHub repo, e.g. `kharcha`.
2. Upload EVERYTHING in this folder, including the `lib` folder (drag the whole folder contents into GitHub's upload page).
3. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/root` → Save.
4. Open `https://<your-username>.github.io/kharcha/` after ~1 minute.
(Only the app code is public. Your expenses are stored only inside each phone.)

## Install
- iPhone: open the link in **Safari** → Share → **Add to Home Screen**.
- Android: open in **Chrome** → ⋮ menu → **Install app / Add to Home screen**.

## First run (each phone)
- iPhone: You = Amruta, Partner = Tathya. Android: tap "Swap" (You = Tathya, Partner = Amruta).
- Enter your 3 bank account names + current balances.
- More → set the **same sync passcode** on both phones (tell each other in person).

## Syncing "Together" expenses
Together tab → "Send to Tathya" → share via WhatsApp. On the other phone: Together → "Receive file" → pick it. Lists merge; edits/deletes sync too. Files are AES-256 encrypted.

## Keep it safe
- Use it from the Home Screen icon (iOS can clear data of sites not added to Home Screen).
- More → "Save backup" once a month.

## Adding expenses
Tap **+ Add**, then either:
- type in the top box: `450 zomato from SBI`, `sent 5000 to appa`, `rd 2000`, `petrol 500 yesterday`
- tap 🎤 and say it
- tap 📷 and pick a bill photo or UPI screenshot (read on the phone, offline)
- tap 📋 to paste a bank SMS (set each account's last 4 digits in More → Accounts so SMS map to the right bank)
Check the filled fields → **Save**. Unknown words (e.g. "gym 1500") become a new category automatically.

## Files in lib/
Offline photo reading (tesseract.js, Apache-2.0), Excel export (SheetJS, Apache-2.0), QR sync (qrcode-generator MIT, jsQR Apache-2.0). They load from your own site only.
