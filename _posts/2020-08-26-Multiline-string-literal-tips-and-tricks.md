---
layout: post
title: "Multiline string literal (Thamizhil)"
author: "Rajeshkumar Lingavel"
---


எப்பவும் Source  Codeக்கு நடுவுல String இருக்க கூடாது. ஏனென்றால் மற்ற மொழிகளில் நம்முடைய Application ஐ மாற்ற முடியாது. ஆனால் ஒரு சில தவிர்க்க முடியாத நேரங்களில்  Strings ஐ  நமது Source code நடுவில் பயன்படுத்த வேண்டிய தேவை ஏற்படும். அந்த சமயத்தில் String literal நமக்கு மிகவும் உதவிகரமாக இருக்கும்


# எடுத்துக்காட்டாக:
```
let Essay = """
Sachin Tendulkar Essay
- Sachin Tendulkar was born on 24 April 1973 in Mumbai. 
- His father, Ramesh Tendulkar was a famous Mandl novelist.
- He has rightly earned the titles or nick names- ‘THE LITTLE MASTER’ and ‘MASTER BLASTER’.
"""
```
# பயன்பாடுகள்:

multiline string literals ல நம் கொடுத்த பார்மட் அப்படியே பயன்படுத்த முடியும் இதில் line break மட்டும் இல்லாமல் indentation bullet points என அனைத்தையும் அதில் String ல் இருப்பது  போல அப்படியே display செய்யும்.
```
let Essay = """
    Sachin Tendulkar Essay
    - Sachin Tendulkar was born on 24 April 1973 in Mumbai. 
    - His father, Ramesh Tendulkar was a famous Mandl novelist.
    - He has rightly earned the titles or nick names- ‘THE LITTLE MASTER’ and ‘MASTER BLASTER’.
"""
```

அது மட்டுமில்லாம இதுல எளிதாக Singe quotation , multiple quotation எல்லாவற்றையும் escape string  இல்லாமல் எளிதாக பயன்படுத்த முடியும்.

```
let HeightLight = """
    Hello please "HeightLight" this.
"""
```

multiline string literals மூலமாக String ஐ நாம் எளிதாக வாசிக்க முடியும்.

```
let balls = """
    Suresh found \(balls) under his bed.
"""
```

அதுபோல ஒரு new line உருவாவதை அந்த வரியின் இறுதியில் backslash கொண்டு தடுக்க முடியும் இது Log print செய்யும் சமயங்களில் நமக்கு பயன்படும்.

```
let errorInfo = """
You are using http API, \
Add App Transport Security Settings in your application plist
""")
```
 
