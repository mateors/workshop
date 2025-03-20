# AI Agent Development Environment Setup

## Operating System
* Linux
* Windows | WSL
* Mac

1. WSL
    * wsl --install -d `<Distro>`
    * wsl --list --online
    * wsl -l -v
    * wsl pwd
    * wsl --install -d Ubuntu-24.04

2. NodeJS
3. PostgreSQL
4. pgadmin
5. pgvector
6. n8n

## 1. WSL Installation

> *Step-1*: Install Ubuntu-24.04 on Windows with WSL -> `wsl --install -d Ubuntu-24.04`
![Step-1](./screens/step_1.png)

Wait 5 to 10 minutes depending on your internet speed
এই ধাপে ৫ মিনিট থেকে ৩০ মিনিট পর্যন্ত অপেক্ষা করতে হতে পারে (আপনার ইন্টারনেট স্পিড এর উপর নির্ভরশীল)
![Step-1.2](./screens/step_1_2.png)

> *Step-2*: `wsl -d Ubuntu-24.04`
![Step-2](./screens/step_2_0.png)

এই স্টেপে সিস্টেম আপনার কাছে ইউসার ও পাসওয়ার্ড চাইবে এবং পরবর্তিতে এই ইউসার এবং পাসওয়ার্ড ব্যবহার করেই আপনাকে WSL সিস্টেমে লগইন করবেন

বাই ডিফল্ট যে ইউসার তৈরী করেছেন সেটি দিয়ে লগইন হবে কিন্তু আপনি চাইলে রুট ইউসার হিসেবেও লগইন করতে পারবেন সেজন্য নিচের কমান্ডটি ব্যবহার করুন

> `wsl -d Ubuntu-24.04 -u root`

এর পর রুট ডিরেক্টরিতে যাবার জন্য `cd` লিখে কীবোর্ড এর `এন্টার` কী প্রেস করুন

## 2. NodeJS
NodeJS ইনস্টলেশনের জন্য এই লিঙ্কে [ক্লিক করুন](https://nodejs.org/en/download) 
এই ওয়েবসাইটি NodeJS এর অফিসিয়াল ওয়েবসাইট, এই ওয়েবসাইট থেকে NodeJS ইনস্টলেশন এর কমান্ড ও গাইডলাইন পাওয়া যাবেনদ

আমরা যেহতু WSL এর মাধ্যমে অপারেটিং সিস্টেম লিনাক্স এর Ubuntu-24.04 ডিস্ট্রো ব্যবহার করছি সুতরাং নিচের কমান্ড গুলো ক্রমান্নয়ে প্রয়োগের মাধ্যমে NodeJS ইনস্টলেশন সম্পন্ন করব

> `apt install -y ca-certificates curl gnupg`

> `mkdir -p /etc/apt/keyrings`

> `curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg`

> `echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_22.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list`

> `apt update`

> `apt install nodejs -y`

> `nodejs --version`

উপরের কমান্ড গুলো যদি সব ঠিক মত রান করে থাকেন তবে নিচের স্ক্রীনে দেখানো আউটপুট দেখা যাবে
![Step-2](./screens/nodejs.png)


## 3. PostgreSQL


## Resource Link
* https://learn.microsoft.com/en-us/windows/wsl/install