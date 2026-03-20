<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.md">English</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/mcp-tool-shop-org/brand/main/logos/portlight/readme.png" width="400" alt="Portlight">
</p>

<p align="center">
  <a href="https://github.com/mcp-tool-shop-org/npm-portlight/actions"><img src="https://github.com/mcp-tool-shop-org/npm-portlight/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://www.npmjs.com/package/@mcptoolshop/portlight"><img src="https://img.shields.io/npm/v/@mcptoolshop/portlight" alt="npm"></a>
  <a href="https://github.com/mcp-tool-shop-org/npm-portlight/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href="https://mcp-tool-shop-org.github.io/npm-portlight/"><img src="https://img.shields.io/badge/docs-landing_page-blue" alt="Landing Page"></a>
</p>

[Portlight](https://github.com/mcp-tool-shop-org/portlight) के लिए npm रैपर - यह एक व्यापार-केंद्रित समुद्री रणनीति कमांड-लाइन इंटरफेस (CLI) है। एक ही कमांड, पाइथन की आवश्यकता नहीं।

## पोर्टलाइट क्या है?

पोर्टलाइट एक टर्मिनल रणनीति गेम है जिसमें आप भूमध्य सागर और पश्चिम अफ्रीकी अर्थव्यवस्था में एक व्यापारी करियर बनाते हैं। कम कीमत पर खरीदें, खतरनाक मार्गों पर यात्रा करें, ऊंची कीमत पर बेचें, और अपने मुनाफे को बुनियादी ढांचे, प्रतिष्ठा और वाणिज्यिक लाभ में फिर से निवेश करें।

ज्यादातर ट्रेडिंग गेम्स के विपरीत, जो व्यापार को केवल एक बढ़ती हुई संख्या के रूप में दर्शाते हैं, पोर्टलाइट व्यापार को एक वाणिज्यिक अनुशासन के रूप में देखता है:

- **कीमतें आपके व्यापार पर प्रतिक्रिया करती हैं।** किसी बंदरगाह पर अनाज डंप करने से कीमत गिर जाती है। हर बिक्री से स्थानीय बाजार बदल जाता है।
- **यात्राओं में वास्तविक जोखिम होता है।** तूफान, समुद्री डाकू, निरीक्षण - आपके प्रावधान, जहाज और चालक दल महत्वपूर्ण हैं।
- **अनुबंधों के लिए प्रमाण की आवश्यकता होती है।** सही माल को सही बंदरगाह पर भेजें, जिसका स्रोत ट्रैक किया गया हो।
- **बुनियादी ढांचा आपके व्यापार के तरीके को बदलता है।** गोदाम माल की तैयारी करते हैं, ब्रोकर अनुबंधों में सुधार करते हैं, लाइसेंस प्रीमियम पहुंच अनलॉक करते हैं।
- **वित्त एक शक्तिशाली उपकरण है।** क्रेडिट आपको तेजी से आगे बढ़ने देता है। यदि आप चूक जाते हैं, तो रास्ते बंद हो जाते हैं।
- **जीतने के चार तरीके हैं।** वैध व्यापारिक घर, गुप्त नेटवर्क, समुद्री क्षेत्र, या वाणिज्यिक साम्राज्य - गेम यह देखता है कि आपने वास्तव में क्या बनाया है।

तीन कप्तान प्रकार (व्यापारी, तस्कर, नेविगेटर), 10 बंदरगाह, 8 व्यापारिक वस्तुएं, 17 मार्ग, 27 मील के पत्थर, और एक पूर्ण बीमा/क्रेडिट प्रणाली।

## शुरुआत कैसे करें

```bash
npx @mcptoolshop/portlight new "Captain Hawk" --type merchant
npx @mcptoolshop/portlight market
npx @mcptoolshop/portlight buy grain 10
npx @mcptoolshop/portlight sail al_manar
npx @mcptoolshop/portlight advance
npx @mcptoolshop/portlight sell grain 10
```

या इसे वैश्विक रूप से स्थापित करें:

```bash
npm install -g @mcptoolshop/portlight
portlight new "Captain Hawk" --type merchant
```

## यह कैसे काम करता है

यह पैकेज GitHub रिलीज़ से आपके प्लेटफ़ॉर्म के लिए पहले से निर्मित पोर्टलाइट बाइनरी को डाउनलोड करता है और इसे स्थानीय रूप से कैश करता है। पाइथन इंस्टॉलेशन की आवश्यकता नहीं है।

| चिंताएं | विवरण |
|---------|--------|
| **Network** | केवल `github.com` CDN के लिए HTTPS |
| **Filesystem** | केवल उपयोगकर्ता कैश में लिखता है (`~/.cache/mcptoolshop/portlight/`) |
| **Verification** | प्रत्येक डाउनलोड पर SHA256 चेकसम |
| **Telemetry** | कोई नहीं। कोई ट्रैकिंग नहीं, कोई विश्लेषण नहीं, कोई डेटा नहीं भेजा जाता। |
| **Platforms** | विंडोज (x64), macOS (x64/arm64), लिनक्स (x64) |

## यह भी pip के माध्यम से उपलब्ध है

यदि आपके पास पाइथन स्थापित है:

```bash
pip install portlight
```

## सुरक्षा

- केवल `github.com` से HTTPS के माध्यम से बाइनरी डाउनलोड करता है
- प्रत्येक डाउनलोड पर SHA256 चेकसम सत्यापन
- केवल उपयोगकर्ता-स्कोप वाले कैश निर्देशिका में लिखता है - सिस्टम निर्देशिकाओं को कभी नहीं छूता
- कोई टेलीमेट्री नहीं, कोई गुप्त जानकारी नहीं, कोई क्रेडेंशियल संग्रहीत नहीं
- प्रारंभिक बाइनरी डाउनलोड के अलावा कोई नेटवर्क एक्सेस नहीं

पूर्ण सुरक्षा नीति के लिए [SECURITY.md](SECURITY.md) देखें।

## लाइसेंस

MIT

<a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a> द्वारा निर्मित।
