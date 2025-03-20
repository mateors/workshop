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

> *Step-1*: Install Ubuntu-24.04 on Windows with WSL -> `wsl --install -d Ubuntu-24.04`
![Step-1](./screens/step_1.png)

Wait 5 to 10 minutes depending on your internet speed
এই ধাপে ৫ মিনিট থেকে ৩০ মিনিট পর্যন্ত অপেক্ষা করতে হতে পারে (আপনার ইন্টারনেট স্পিড এর উপর নির্ভরশীল)
![Step-1.2](./screens/step_1_2.png)

> Step-2: `wsl -d Ubuntu-24.04`
![Step-2](./screens/step_2_0.png)

এই স্টেপে সিস্টেম আপনার কাছে ইউসার ও পাসওয়ার্ড চাইবে এবং পরবর্তিতে এই ইউসার এবং পাসওয়ার্ড ব্যবহার করেই আপনাকে WSL সিস্টেমে লগইন করবেন

বাই ডিফল্ট যে ইউসার তৈরী করেছেন সেটি দিয়ে লগইন হবে কিন্তু আপনি চাইলে রুট ইউসার হিসেবেও লগইন করতে পারবেন সেজন্য নিচের কমান্ডটি ব্যবহার করুন

> `wsl -d Ubuntu-24.04 -u root`

এর পর রুট ডিরেক্টরিতে যাবার জন্য `cd` লিখে কীবোর্ড এর `এন্টার` কী প্রেস করুন

2. NodeJS
3. PostgreSQL
4. pgadmin
5. pgvector
6. n8n


## Resource Link
* https://learn.microsoft.com/en-us/windows/wsl/install