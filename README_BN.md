# Lyric Studio — একক পরিষ্কার প্রজেক্ট

এই সংস্করণে রাখা হয়েছে:
- বাংলা/ইংরেজি লিরিক লেখা ও প্রিভিউ
- এই ডিভাইসে খসড়া সেভ
- TXT ফাইলে লিরিক এক্সপোর্ট
- অফলাইন Style Box Builder
- Capacitor Android wrapper কনফিগারেশন
- GitHub Actions-এ Android APK বিল্ড workflow

ভিডিও/MP4 রেন্ডারিং এই সংস্করণে ইচ্ছাকৃতভাবে রাখা হয়নি, যাতে প্রথমে ছোট ও স্থিতিশীল ভিত্তি তৈরি করা যায়।

## GitHub-এ আপলোড
ZIP Extract করার পর এই ফোল্ডারের **ভেতরের সব ফাইল ও ফোল্ডার** repository root-এ আপলোড করুন। `package.json`, `capacitor.config.json`, `www/`, `.github/` root-এ থাকবে।

## APK তৈরি
1. GitHub repository-তে ফাইলগুলো আপলোড/কমিট করুন।
2. Actions ট্যাব খুলুন।
3. `Build Android APK` workflow বেছে `Run workflow` চাপুন।
4. সফল হলে run-এর Artifacts থেকে `lyric-studio-debug-apk` ZIP ডাউনলোড করুন।
5. Artifacts ZIP extract করে `app-debug.apk` ইনস্টল করুন।

## গুরুত্বপূর্ণ
এখানে APK বাইনারি আগে থেকে তৈরি নেই। GitHub Actions-এ বিল্ড সফল হলেই APK পাওয়া যাবে। বিল্ডের ফলাফল যাচাই না করে সফল বলা যাবে না।
