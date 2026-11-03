# 🚀 Traccar, Wialon & GPS - Official WhatsApp SMS Gateway

[![5MinutesAPI](https://img.shields.io/badge/Powered%20By-5MinutesAPI-25D366?style=for-the-badge&logo=whatsapp)](https://5minutesapi.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

The most reliable, zero-markup **WhatsApp Cloud API Bridge** for GPS Fleet Tracking Servers. Replace expensive traditional SMS gateways with official, end-to-end encrypted WhatsApp alerts.

Perfectly optimized for **Traccar**, **Wialon**, **GPS**, and custom GPS logistics software operating in Saudi Arabia (KSA), UAE, Oman, Qatar, and Globally.

## 🔥 Why Switch from SMS to 5MinutesAPI?
* 💰 **Cut Costs by 90%:** Stop paying $0.05 per SMS. Meta's official API is significantly cheaper, and 5MinutesAPI charges **Zero Markup**.
* 🚫 **No More Bans:** Unofficial QR-code bots get banned constantly. We use the Official Meta API with safe Utility Templates.
* ⚡ **Instant Alerts:** Real-time delivery for Ignition ON/OFF, Overspeed, Fuel Theft, and Geofence alerts.
* 🛠️ **Zero Coding Required:** Just paste our Universal Bridge URL into your GPS software's SMS settings.

---

## ⚙️ How to Configure in Traccar (Setup in 2 Minutes)

You do not need to download any complex plugins. 5MinutesAPI acts as a drop-in replacement for your default `HttpSmsManager`.

### Step 1: Get Your API Key
1. Go to [5MinutesAPI.com](https://5minutesapi.com) and create an account.
2. Generate your **Master API Key** from the developer dashboard.

### Step 2: Edit your `traccar.xml`
Open your Traccar server's configuration file (`traccar.xml`) and add/replace the SMS manager entry with the following snippet:

```xml
<!-- 5MinutesAPI Official WhatsApp Gateway -->
<entry key='notificator.sms.manager.class'>org.traccar.sms.HttpSmsManager</entry>
<entry key='notificator.sms.manager.url'>[https://api.5minutesapi.com/v1/bridge/universal?api_key=YOUR_5MINUTESAPI_KEY_HERE&amp;template=system_alert&amp;to=](https://api.5minutesapi.com/v1/bridge/universal?api_key=YOUR_5MINUTESAPI_KEY_HERE&amp;template=system_alert&amp;to=){phone}&amp;var1={message}</entry>
(Make sure to replace YOUR_5MINUTESAPI_KEY_HERE with your actual API key)

Step 3: Restart Traccar
Restart your Traccar service. Your fleet alerts will now instantly deliver to your clients' WhatsApp!

🌐 Supported Platforms
This universal HTTP bridge works out-of-the-box with:

Traccar (Open Source GPS)

Wialon (Fleet Management)

GPS

Navixy

Custom Logistics & Rent-a-Car software

🎁 Need a Custom Setup? (100% Free Integration)
Don't have a technical team? Our integration engineers will set up the official WhatsApp API on your Traccar/Wialon server completely free of charge (Limited time offer for 2026).
