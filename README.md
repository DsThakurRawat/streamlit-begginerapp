
# 🏛️ CampusConnect - The Digital Heartbeat of Your University

<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 220942.jpg" alt="CampusConnect Landing Page"/>
</p>

**CampusConnect** is not just another social network; it's a vibrant, all-in-one digital ecosystem designed exclusively for university students and alumni. It bridges the gap between academics, social life, and professional networking, creating a unified hub where campus life thrives. With a sleek, intuitive interface and a powerful set of features, CampusConnect is the ultimate tool to enrich your university journey and unlock your future.

### ✨ Live Demo

[**[Link to your live project deployment]**](https://example.com) &lt;-- *Replace this with your actual live URL!*

---

## 📸 A Glimpse into CampusConnect

| Login & Onboarding | The Campus Feed | Explore Events & Topics |
| :---: | :---: | :---: |
| <img src=".github/assets/Screenshot 2025-09-28 221115.png" alt="Login Screen" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221235.jpg" alt="Campus Feed" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221307.jpg" alt="Explore Page" width="250"/> |
| **Professional Networking** | **Real-Time Messaging** | **Code & Connect Leaderboard** |
| <img src=".github/assets/Screenshot 2025-09-28 221443.jpg" alt="Networking Directory" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221424.jpg" alt="Messaging Interface" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221501.jpg" alt="Code & Connect Page" width="250"/> |

---

## 🚀 Core Features

CampusConnect is packed with features designed to enhance every aspect of student and alumni life.

### Authentication & Onboarding
A seamless and secure entry point. New users can create detailed accounts, specifying their status (student/alumni) and graduation year, while returning users are greeted with a familiar login.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221139.png" alt="Create Account Screen"/>
</p>

### 🌐 The Campus Pulse: Real-Time Feed
The central hub of activity. Share your updates, post photos, ask questions, and stay in the loop with everything happening across the university. The dynamic feed is complemented by widgets for **Stories** and discovering **Communities**.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221235.jpg" alt="The Campus Feed"/>
</p>

### 🔭 Explore Campus
Discover what's new and exciting. The Explore page showcases live events, workshops, trending campus topics via hashtags, and a directory of clubs and groups, making it easy to find your niche and get involved.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221307.jpg" alt="Explore Campus Page"/>
</p>

### 🤝 Professional Networking & Alumni Directory
A built-in professional network. Browse a directory of students and alumni, discover their professional roles, and initiate conversations. It's like having a university-exclusive LinkedIn at your fingertips.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221443.jpg" alt="Networking Directory"/>
</p>

### 💬 Real-Time Messaging
Connect privately with your peers. A fully-featured, real-time messaging interface allows for one-on-one conversations with anyone in your network.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221424.jpg" alt="Real-time Messaging"/>
</p>

### 💻 Code & Connect
For the tech enthusiasts! This unique feature showcases the top coders and developers in the university. A leaderboard tracks points, and detailed profiles display social links and platform stats, fostering a spirit of friendly competition and collaboration.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221501.jpg" alt="Code & Connect Leaderboard"/>
</p>

### 👤 Comprehensive & Customizable Profiles
Your digital identity on campus. Users can create rich profiles that go beyond the basics, including work experience, skills, and even dynamic stats from GitHub, LeetCode, and Codeforces.
<p align="center">
  <img src=".github/assets/Screenshot 2025-09-28 221528.jpg" alt="User Profile Page"/>
  <img src=".github/assets/Screenshot 2025-09-28 221552.png" alt="Profile with GitHub and Coding Stats"/>
</p>

### ❤️ Cupid's Arrow: A Fun Way to Connect
Injecting a bit of fun into campus life! This feature allows users to anonymously express interest in their crush.
* **Love Quest:** Secretly submit the name of someone you're interested in.
* **It's a Match!** If two users submit each other's names, a match is created!
* **Secret Message:** Matched users get one chance to send a one-time anonymous message to break the ice. Your identity is only revealed if they reply!
* **Blind Crush Board:** Post wholesome, anonymous messages for people on campus, spreading positivity and intrigue.

| Love Quest & Matching | Blind Crush Board | A Successful Match! |
| :---: | :---: | :---: |
| <img src=".github/assets/Screenshot 2025-09-28 221713.jpg" alt="Love Quest" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221822.jpg" alt="Blind Crush Board" width="250"/> | <img src=".github/assets/Screenshot 2025-09-28 221912.jpg" alt="Secret Message" width="250"/> |


---

## 🛠️ Technology Stack

This project was built using modern, scalable, and efficient technologies.

* **Frontend:**
    * **HTML5**
    * **CSS3** with **Tailwind CSS** (for a utility-first, responsive design system)
    * **Vanilla JavaScript** (for interactivity and API communication)
* **Backend & Database:**
    * **Supabase:** The open-source Firebase alternative. We use it for:
        * **PostgreSQL Database:** Storing all user data, posts, messages, etc.
        * **Real-time APIs:** Powering the live feed and chat functionalities.
        * **Authentication:** Secure user login and management.
        * **Storage:** (Optional) For hosting user-uploaded images.

---

## 🔧 Getting Started

To get a local copy up and running, follow these simple steps.

#### **Prerequisites**
You will need a code editor (like VS Code) and a modern web browser.

#### **Installation & Setup**

1.  **Clone the Repository**
    ```sh
    git clone [https://github.com/your-username/campusconnect.git](https://github.com/your-username/campusconnect.git)
    cd campusconnect
    ```

2.  **Configure Supabase Credentials**
    * Navigate to the file containing your JavaScript logic.
    * Replace the placeholder values with your actual Supabase Project URL and Anon Key.
    ```javascript
    const SUPABASE_URL = "YOUR_SUPABASE_PROJECT_URL";
    const SUPABASE_ANON_KEY = "YOUR_SUPABASE_ANON_KEY";
    const supabase = window.supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
    ```
    > **⚠️ Security Warning:** Never commit your secret keys to a public repository. For a production app, use environment variables.

3.  **Set Up the Supabase Database Schema**
    * Create a new project in your [Supabase Dashboard](https://supabase.com/).
    * Go to the **SQL Editor** and run the following queries to create the necessary tables.
    ```sql
    -- Profiles Table (stores public user data)
    CREATE TABLE profiles (
      id UUID PRIMARY KEY REFERENCES auth.users(id) ON DELETE CASCADE,
      username TEXT UNIQUE NOT NULL,
      full_name TEXT,
      avatar_url TEXT,
      status TEXT, -- e.g., 'Student', 'Alumnus'
      graduation_year INT,
      title TEXT,
      about TEXT
    );

    -- Posts Table
    CREATE TABLE posts (
      id BIGINT PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
      user_id UUID REFERENCES profiles(id) ON DELETE CASCADE,
      content TEXT NOT NULL,
      image_url TEXT,
      created_at TIMESTAMPTZ DEFAULT NOW()
    );

    -- Crushes Table (for the Cupid feature)
    CREATE TABLE crushes (
      id BIGINT PRIMARY KEY GENERATED ALWAYS AS IDENTITY,
      submitter_id UUID REFERENCES profiles(id) ON DELETE CASCADE,
      crush_id UUID REFERENCES profiles(id) ON DELETE CASCADE,
      created_at TIMESTAMPTZ DEFAULT NOW(),
      UNIQUE(submitter_id, crush_id) -- Prevents duplicate submissions
    );

    -- Enable Row Level Security (CRUCIAL for security)
    ALTER TABLE profiles ENABLE ROW LEVEL SECURITY;
    ALTER TABLE posts ENABLE ROW LEVEL SECURITY;
    ALTER TABLE crushes ENABLE ROW LEVEL SECURITY;

    -- Create RLS Policies (examples)
    CREATE POLICY "Public profiles are viewable by everyone." ON profiles FOR SELECT USING (true);
    CREATE POLICY "Users can insert their own profile." ON profiles FOR INSERT WITH CHECK (auth.uid() = id);
    CREATE POLICY "Users can update their own profile." ON profiles FOR UPDATE USING (auth.uid() = id);
    ```
    *You will need to create similar, appropriate RLS policies for `posts`, `messages`, and `crushes` based on your application's logic.*

4.  **Run the Application**
    * Simply open the `index.html` file in your browser.
    * For the best development experience, use an extension like **Live Server** in VS Code.

---

## 🤝 Contributing

Contributions are what make the open-source community an amazing place to learn and create. Any contributions you make are **greatly appreciated**. Please read the contribution guidelines before submitting a PR.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'feat: Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE.txt` for more information.

---

## 📧 Contact

**Sankalp Thorat** - [sankalp@email.com](mailto:sankalp@email.com) &lt;-- *Update your contact info!*

Project Link: [https://github.com/your-username/campusconnect](https://github.com/your-username/campusconnect) &lt;-- *And your repo link!*
