# About the Kokuji
Kokuji, also known as “Japanese kanji characters created in Japan,” are kanji characters that were invented in Japan rather than being imported from China.   
These characters were developed to express concepts, objects, or ideas that were unique to Japanese culture and society. Unlike most kanji, which have their origins in Chinese characters, kokuji were specifically created to meet the linguistic needs of the Japanese language.   
Examples of kokuji include characters such as “峠” (mountain pass), “働” (to work), and “畑” (field). These characters often combine existing kanji components in new ways to create meanings that did not exist in Chinese.

Sources:
- [Kokuji - Wikipedia](https://en.wikipedia.org/wiki/Kokuji)
- [Kokuji: “Made In Japan,” Kanji Edition](https://howto-learn-japanese.blogspot.com/2012/09/kokuji-made-in-japan-kanji-edition.html)
- [Kokuji – Kanji That’s Made In Japan](https://www.lingualift.com/blog/kanji-made-in-japan/)

## How to Determine the Pinyin for Kokuji
The document “日本汉字的汉语读音规范” (i.e. Standard for Chinese Pronunciation of Japanese Kanji) provides guidelines for how to pronounce Japanese kanji in Chinese. 
It categorizes kanji and suggests using Chinese pronunciations where possible, adopting readings from phonetic or semantic components if necessary, and using similar characters when direct readings are not available. 
The following is a flowchart interpreting the 'Standard for Chinese Pronunciation of Japanese Kanji'.

![日本汉字的汉语读音规范](./img/日本汉字的汉语读音规范.svg)

```mermaid
flowchart TD
    A[汉字分类] --> B{日本自造汉字?}
    B -->|yes| C{可视为形声或会意兼形声?}
    C -->|yes| D['取声旁的读音<br/>例如: 畑取tián（田）音,<br/>辻取shí（十）音,<br/>込取rù（入）音,<br/>鴫取tián（田）音']
    C -->|no| E['取形似字或形似声旁的读音<br/>例如: 麿取形似字磨的字音mó,<br/>峠右边声旁跟卡形似, 取kǎ音']
    
    B -->|no| F{中日同形字?}
    F -->|yes| G{中国汉字有读音?}
    G -->|yes| H['直接取同形的中国汉字读音<br/>例如: 匂与中国汉字匀的早期字形相同, 取yún音,<br/>槇与中国汉字槙的旧字形相同, 取zhēn音']
    G -->|no| I{可视为形声或会意兼形声?}
    I -->|yes| J['一般取声旁读音<br/>例如: 杣可视为形声字, 取shān（山）音']
    I -->|no| K[另定读音]
    
    F -->|no| L{中国古字或俗字?}
    L -->|yes| M{判定为中国古字或俗字?}
    M -->|yes| N['按中国汉字读音<br/>例如: 俣是中国古字, 读yǔ,<br/>搾是中国汉字榨的异体字, 读zhà']
    M -->|no| O['另定读音<br/>例如: 籾按形声字处理, 取rèn（刃）音']
    
    L -->|no| P{日本略字（日本简体字）?}
    P -->|yes| Q{日本简体字形的繁体与中国内地简化字形的繁体为同一汉字字形?}
    Q -->|yes| R['按相应的中国简化字读音<br/>例如: 広（日）广（中）的繁体同为廣, 读广（guǎng）音,<br/>桜（日）樱（中）的繁体同为櫻, 读樱（yīng）音']
    Q -->|no| S['按相应的中国传承字读音<br/>例如: 拂日本简化为払, 中国不简, 払读拂（fú）音,<br/>醉日本简化为酔, 中国不简, 酔读醉（zuì）音']
    
    P -->|no| T[结束]
    
    D --> T
    E --> T
    H --> T
    J --> T
    K --> T
    N --> T
    O --> T
    R --> T
    S --> T
```


Since there are patterns that do not fit within the ‘Standard for Chinese Pronunciation of Japanese Kanji,’ I expanded the interpretation. The following flowchart was used to determine the pinyin.

![拼音选择流程_中文](./img/拼音选择流程_中文.svg)

> [!NOTE]
> The original flowchart contained special Unicode characters (𭬺, 𢌽, 𫡷, 𱁬, 䨺龘) that caused parsing errors in Mermaid format, so SVG images are used instead for proper display.

# Organized Table of Kokuji
Refer to [Organized-Table-of-Kokuji](https://github.com/MaruTama/kokuji-pinyin-data/wiki).
