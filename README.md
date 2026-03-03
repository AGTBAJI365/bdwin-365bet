# bdwin-365bet

**আপনার অনলাইন বেটিং এবং গেমিং প্ল্যাটফর্ম**

bdwin-365bet একটি আধুনিক এবং নিরাপদ অনলাইন বেটিং প্ল্যাটফর্ম যা ব্যবহারকারীদের বিভিন্ন ক্রীড়া এবং গেমে অংশগ্রহণের সুযোগ প্রদান করে।

## বৈশিষ্ট্য

- ✅ নিরাপদ ব্যবহারকারী প্রমাণীকরণ
- ✅ লাইভ বেটিং সুবিধা
- ✅ একাধিক পেমেন্ট গেটওয়ে
- ✅ রিয়েল-টাইম লিডারবোর্ড
- ✅ মোবাইল-বান্ধব ডিজাইন
- ✅ ২৪/৭ কাস্টমার সাপোর্ট

## প্রযুক্তি স্ট্যাক

- **ব্যাকএন্ড**: Python/Django
- **ফ্রন্টএন্ড**: HTML, CSS, JavaScript, Bootstrap
- **ডাটাবেস**: PostgreSQL
- **ক্যাশিং**: Redis
- **ডিপ্লয়মেন্ট**: Docker, Kubernetes

## ইনস্টলেশন

### প্রয়োজনীয় সফটওয়্যার

- Python 3.8+
- PostgreSQL 12+
- Redis 6+
- Docker (ঐচ্ছিক)

### স্থানীয় সেটআপ

```bash
# রিপোজিটরি ক্লোন করুন
git clone https://github.com/AGTBAJI365/bdwin-365bet.git
cd bdwin-365bet

# ভার্চুয়াল পরিবেশ তৈরি করুন
python -m venv venv
source venv/bin/activate  # Windows এর জন্য: venv\Scripts\activate

# প্যাকেজ ইনস্টল করুন
pip install -r requirements.txt

# ডাটাবেস মাইগ্রেশন
python manage.py migrate

# সার্ভার শুরু করুন
python manage.py runserver
```

## Docker সহ সেটআপ

```bash
docker-compose up -d
```

## প্রজেক্ট স্ট্রাকচার

```
bdwin-365bet/
├── backend/              # Django ব্যাকএন্ড
│   ├── accounts/         # ব্যবহারকারী ব্যবস্থাপনা
│   ├── betting/          # বেটিং লজিক
│   ├── games/            # গেম কনফিগারেশন
│   ├── payments/         # পেমেন্ট প্রসেসিং
│   └── settings.py       # Django সেটিংস
├── frontend/             # ফ্রন্টএন্ড ফাইল
│   ├── index.html
│   ├── css/
│   ├── js/
│   └── images/
├── tests/                # টেস্ট ফাইল
├── docs/                 # ডকুমেন্টেশন
├── docker-compose.yml
├── Dockerfile
├── requirements.txt
└── README.md
```

## পরিবেশ ভেরিয়েবল (.env)

```
DEBUG=False
SECRET_KEY=your-secret-key-here
DATABASE_URL=postgresql://user:password@localhost:5432/bdwin365bet
REDIS_URL=redis://localhost:6379/0
STRIPE_SECRET_KEY=your-stripe-key
STRIPE_PUBLISHABLE_KEY=your-stripe-public-key
```

## এপিআই এন্ডপয়েন্ট

### প্রমাণীকরণ
- `POST /api/auth/register/` - নতুন অ্যাকাউন্ট তৈরি
- `POST /api/auth/login/` - লগইন
- `POST /api/auth/logout/` - লগআউট

### বেটিং
- `GET /api/bets/` - সমস্ত বেট দেখুন
- `POST /api/bets/place/` - নতুন বেট রাখুন
- `GET /api/bets/{id}/` - বেটের বিবরণ

### গেম
- `GET /api/games/` - সমস্ত গেম
- `GET /api/games/{id}/` - গেমের বিবরণ

### অ্যাকাউন্ট
- `GET /api/account/profile/` - প্রোফাইল দ��খুন
- `PUT /api/account/profile/` - প্রোফাইল আপডেট করুন
- `GET /api/account/wallet/` - ওয়ালেট ব্যালেন্স

## অবদান রাখুন

আমরা অবদানকে স্বাগত জানাই! অনুগ্রহ করে নিম্নলিখিত পদক্ষেপ অনুসরণ করুন:

1. ফর্ক করুন এই রিপোজিটরি
2. একটি নতুন শাখা তৈরি করুন (`git checkout -b feature/AmazingFeature`)
3. আপনার পরিবর্তন কমিট করুন (`git commit -m 'Add some AmazingFeature'`)
4. শাখায় পুশ করুন (`git push origin feature/AmazingFeature`)
5. একটি Pull Request খুলুন

## লাইসেন্স

এই প্রজেক্ট MIT লাইসেন্স এর অধীন। বিস্তারিত জন্য [LICENSE](LICENSE) ফাইল দেখুন।

## যোগাযোগ

- **ইমেইল**: support@bdwin-365bet.com
- **ওয়েবসাইট**: https://bdwin-365bet.com
- **সাপোর্ট ফোরাম**: https://forum.bdwin-365bet.com

## সম্প্রদায়

আমাদের সম্প্রদায়ে যোগ দিন এবং অন্যান্য ব্যবহারকারী এবং ডেভেলপারদের সাথে সংযোগ করুন।

---

**সর্বশেষ আপডেট**: ২০২৬-০৩-০৩