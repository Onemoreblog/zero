---
layout: post
title: "Multiline string literal tips and tricks"
author: "Rajeshkumar Lingavel"
---


எப்பவும் Source  Codeக்கு நடுவுல String இருக்க கூடாது. ஏனென்றால் மற்ற மொழிகளில் நம்முடைய Application ஐ மாற்ற முடியாது. ஆனால் ஒரு சில தவிர்க்க முடியாத நேரங்களில்  Strings ஐ  நமது Source code நடுவில் பயன்படுத்த வேண்டிய தேவை ஏற்படும். அந்த சமயத்தில் String literal நமக்கு மிகவும் உதவிகரமாக இருக்கும்


# எடுத்துக்காட்டாக:
```
let infoMessage = """
Welcome to my animation tool. You can use it to:
- Convert images into animations.
- Split an animation up into images.
- Change the frame rate of an animation.
"""
```

multiline string literals ல நம் கொடுத்த பார்மட் அப்படியே பயன்படுத்த முடியும் இதில் line break மட்டும் இல்லாமல் indentation bullet points என அனைத்தையும் அதில் String ல் இருப்பது  போல அப்படியே display செய்யும்.
```
let infoMessage = """
    Welcome to my animation tool. You can use it to:
        - Convert images into animations.
        - Split an animation up into images.
        - Change the frame rate of an animation.
"""
```

அது மட்டுமில்லாம இதுல எளிதாக Singe quotation , multiple quotation எல்லாவற்றையும் escape string  இல்லாமல் எளிதாக பயன்படுத்த முடியும்.

```
let infoMessage = """
    Hello please "HeightLight" this.
"""
```

multiline string literals மூலமாக String ஐ நாம் எளிதாக வாசிக்க முடியும்.

```
assertionFailure("""
An object for the key "\(key)" could not be found.
""")
```

அதுபோல ஒரு new line உருவாவதை அந்த வரியின் இறுதியில் backslash கொண்டு தடுக்க முடியும் இது Log print செய்யும் சமயங்களில் நமக்கு பயன்படும்.

```
assertionFailure("""
An object for the key "\(key)" could not be found, \
perhaps you forgot to add it using setObject(forKey:)?
""")
```


> Note: This is tamil translation of swiftbysundell. [originalblog](https://www.swiftbysundell.com/tips/multiline-string-literal-tips-and-tricks/)
 
