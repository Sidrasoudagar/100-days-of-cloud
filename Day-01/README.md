# Day 01 — Create an RSA Key Pair in AWS

## 🎯 Objective
Create an EC2 key pair named `devops-kp` with the RSA key type in the `us-east-1` region.

## 🧭 Steps Taken
1. Logged in to the AWS Management Console for the lab account.
2. Confirmed the region was set to **US East (N. Virginia) us-east-1**.
3. Navigated to **EC2 → Network & Security → Key Pairs**.
4. Clicked **Create key pair**.
5. Configured:
   - **Name**: `devops-kp`
   - **Key pair type**: **RSA**
   - **Private key format**: `.pem`
6. Downloaded the private key file `devops-kp.pem`.
7. Verified the key pair appeared in the Key Pairs list.

## ☁️ AWS Services Used
- **EC2** (Key Pairs)

## 💡 Key Learnings
- EC2 key pairs are **region-specific** — they must be created in the same region as the instances that will use them.
- **RSA** is one of the two supported key types (the other being **ED25519**).
- The private key file (`.pem`) can only be downloaded **once**. If lost, the key pair must be recreated.
- Private key files must be secured with `chmod 400` before SSH use.

## 🖼️ Screenshot
![Key Pair Created](./<img width="1903" height="775" alt="Screenshot 2026-09-16 154721" src="https://github.com/user-attachments/assets/6dd488ed-374f-41df-814f-1ff1f3b6af7d" />
)

## 🔗 Reference
- Task provided by: [KodeKloud 100 Days of Cloud](https://kodekloud.com/100-days-of-cloud)
