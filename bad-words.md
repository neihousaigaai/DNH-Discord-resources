## List of bad words

<details>
<summary><b>Warning:</b> Bad words, think carefully before clicking</summary>

```py
bad_words = [
# English
# source:
# - http://www.hyperhero.com/en/insults.htm
# - https://reallifeglobal.com/how-to-use-swear-words-in-english/
"ass",
"asshole",
"bitch",
"bullshit",
"butt",
"cock",
"cunt",
"dick",
"damn",
"faggot",
"fuck",
"fucker",
"motherfucker",
"shit",
"whore",

# Vietnamese
# source: 
# - http://qr.ae/TUp27Z
# - http://qr.ae/TUp27V
# - www.youswear.com/index.asp?language=Vietnamese
"buồi",
"bú buồi",
"bú cu",
"buscu",
"chịch",
"con bà mày",
"con bán hoa",
"thằng chó này",
"con chó chết",
"con chó đẻ",
"con cặc",
"con mẹ mày",
"con đĩ",
"cặc",
"cứt",
"kệ mẹ mày",
"kệ mẹ tao",
"kệ mẹ thằng",
"lồn",
"lìn",
"lỗ đít",
"mẹ đồ ngu",
"mẹ bố mày",
"mẹ bố thằng",
"thằng chó chết",
"thằng chó đẻ",
"vãi cứt",
"vãi lồn",
"vãi đái",
"ăn cu",
"ăn cứt",
"ăn máu lồn",
"đái",
"đcm",
"đéo",
"địt",
"đcmm",
"đm",
"đmm",
"đù má",
"đĩ",
"đĩ mẹ mày",
"địt",
"địt bà",
"địt bố",
"địt cha",
"địt con mẹ mày",
"địt con đĩ mẹ mày",
"địt cái lồn mẹ mày",
"địt cả lũ nhà mày",
"địt cụ",
"địt cụ mày",
"địt mẹ",
"địt mẹ mày",
"địt mẹ nhà mày",
"đồ chó chết",
"đồ chó đẻ",
"đụ",
"đụ má",
"đụ má mày",
"đụ má mày con chó",
"đụ má mày con đĩ",
"đụ mẹ mày",
"vếu",
"vú"
]
```

</details>

## Function

```py
def isBadWord(word):
    return word.lower() in bad_words

def isContainingBadWord(s):
    _s = s.lower()
    return any(_s.find(bad_word) != -1 for bad_word in bad_words)

def replaceBadWord(s):
    import re
    for bad_word in bad_words:
        s = re.sub(bad_word, r'*'*len(bad_word), s, flags=re.IGNORECASE)

    return s
```
