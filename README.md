# CloneBotUpdateVersion (PersonalUse)
Source: https://github.com/jagrit007/Telegram-CloneBot
<p align="center">
<img src="https://i.imgur.com/SjeoNU1.jpg">
</p>

ဒီbot လေးကို GDrive ရှိပြီး bot လုပ်ရခက်နေသူတွေအတွက် ဖန်တီးထားခြင်းဖြစ်ပါတယ်။ Pro သမားများအဆင်ပြေမည်မဟုတ်ပါ။ ယခုနောက်ပိုင်း user rate exceed/limit စတဲ့ error များ ရှင်းထားပါတယ်။ Edu SD အများစုထံကူးလို့ရပါတယ်။

**အထူးသတိပြုရန်**
Service Acc သုံးပါက Source Drive နှင့် ကူးမည့်မိမိShareDrive တိုတွင် googlegroup mail ကို contributor အဖြစ် add ထားမှ ကူးလိုရမှာပါ။ addနည်းကို ဒီမှာကြည့်ပါ။https://tiny.one/dwtykxca

# ဘယ်လိုSetUp လုပ်ရမလဲ? ၁။ www.koyeb.com  (အကောင့်ဖွင့်လျှင် Cc or Card ထည့်ရပါတယ်။ Charges free)

ပထမဆုံး https://app.koyeb.com မှာအရင် အကောင့်ဖွင့်ပါ။ ဖွင့်ပြီးသားဆို login ဝင်ထားပါ။
Dockerfile ထဲမှ image name ကူးပါ။

anasaty17/gclone:public     ဒါကိုကူးပြီး လုပ်ရမှာပါ။


Koyeb တွင် github source ဖြင့်မလုပ်ပဲ Docker image ဖြင့်လုပ်ပါ။
ကျန် koyeb settingများ ပုံမှန်လုပ်သွားပြီး advanced ကိုဖွင့်ပါ။
Env Vars ၃ ခုဖြည့်ရပါမယ် စာလုံးမှားလို့မရပါ
- Name                  -(Type)-              Value
- BOT_TOKEN             -(Plaintext)-         https://t.me/BotFather မှ token ထည့်ပါ
- USE_SERVICE_ACCOUNTS  -(Plaintext)-         True သို့မဟုတ် False ထည့်ရန်။ SA ပါလျှင် True
- ZIP                   -(Plaintext)-         https://www.~~~~~~~/ZIP.zip ထည့်ရန်
  

# ZIP varriable ဘယ်လိုလုပ်ရမလဲ

Service accounts သုံးမယ်ဆိုလျှင် (0-99.json) ဖိုင်များပါသော ၁။ accounts ဖိုလ်ဒါ  
၂။ token.pickle ဖိုင်
၃။ credentials.json ဖိုင်

ဒီ 3ခု (folder 1 + files 2) ကို select ပြီး zip ပါ။ Name ကို ⭐ ZIP.zip  လို့ပေးပါ။ တခြားနာမည်ဆို Bot က မဖတ်ပါ။

ZIP.zip ဖိုင်ကို မိမိ google drive ရှိ mydrive တွင်တင်ပါ။
ထို ဖိုင်ကို " share with anyone with link " ဖြင့် share link ယူပါ။
ထို share link ကို http://gist.github.com တွင် paste ပါ file name ကို ZIP.zip လို့ပဲ ပေးပါ။
ထို့နောက် create secret gist ကို နှိပ်ပါ။ ပြီးလျှင် ညာဖက် အပေါ်နားက Raw ကို နှိပ်ပါ။
✅ထို ရလာသော link ကို အပေါ်က ZIP ရဲ့ vars မှာ ဖြည့်ပါ။

**ထို vars 3ခု ဖြည့်ပြီး လျှင် အောက်နားရှိ port နေရာတွင် 8080 ကို 80 ဟုပြင်ပါ။

ပြီးလျှင် koyeb deploy process ဆက်သွားပါ။

# Render တွင် free host သုံးမယ်

heroku ေနာက်ပိုင်း free ရတဲ့ အဆင်ပြေတဲ့ service ပါ။
mail တစ်ခုရှိရင် အကောင့်ဖွင့်လို့ရပါပြီ။ Card မလိုပါ။

deploy guide : [Click Here](https://telegra.ph/DeployGcloneonRender-01-12)

မေးမြန်းလိုသည်များရှိလျှင် https://t.me/drivetalk သို့ လာခဲ့ပါ။
