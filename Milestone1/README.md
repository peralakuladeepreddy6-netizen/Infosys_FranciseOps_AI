# ⚡ Infosys Springboard 7.0 - Milestone 1: User Authentication Module

## Overview
This repository contains the Milestone 1 deliverable for the Infosys Springboard Internship. It is a secure, multi-page User Authentication Portal built entirely in Python using Streamlit. 

## Features Implemented
* **Secure Login & Signup:** Incorporates strict Regex validation for emails and complex passwords.
* **JWT Session Management:** Generates stateless JSON Web Tokens (JWT) upon successful login for secure routing.
* **Dual-Route Password Recovery:** Users can reset passwords via a registered Security Question or via a 6-digit OTP sent to their Gmail.
* **Role-Based Dashboards:** Distinct routing for standard users and a protected Admin Control Panel.
* **Database Management:** Uses SQLite3 to store user credentials, employing `bcrypt` for secure password hashing.

## Tech Stack
* **Frontend/UI:** Streamlit, Streamlit Option Menu, Plotly
* **Backend:** SQLite3, PyJWT, Bcrypt
* **Networking & Email:** Pyngrok, Smtplib, MIME

## How to Run in Google Colab
1. Upload the `.ipynb` file to Google Colab.
2. Add the following keys to your Colab **Secrets** tab (enable Notebook Access):
   - `JWT_SECRET`: Any secure random string.
   - `NGROK_AUTHTOKEN`: Your personal ngrok auth token.
   - `EMAIL_ADDRESS`: The sender Gmail address.
   - `EMAIL_PASSWORD`: The 16-character Gmail App Password.
3. Run all cells. 
4. Click the generated Ngrok public URL to launch the portal.

## Screenshots
* [Login Page](./screenshots/login.png)
* [Signup Page](./screenshots/signup.png)
* [Forgot Password - OTP Route](./screenshots/forgot_otp.png)
* [Forgot Password - Security Question Route](./screenshots/forgot_sq.png)
* [OTP Email Received](./screenshots/otp_email.png)
* [User Dashboard](./screenshots/user_dashboard.png)
* [Admin Dashboard](./screenshots/admin_dashboard.png)
