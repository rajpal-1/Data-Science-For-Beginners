# डेटा का अवलोकन 
|![ Sketchnote by [(@sketchthedocs)](https://sketchthedocs.dev) ](../../../sketchnotes/03-DefiningData.png)|
|:---:|
|डेटा का अवलोकन  - _Sketchnote by [@nitya](https://twitter.com/nitya)_ |

डेटा मतलब तथ्य, माहिती और अनुभव है जिनका इस्तमाल करके नए खोज और सूचित निर्णयोंका समर्थन किया जाता है।

डेटा पॉइंट यह डेटासेट का सबसे छोटा प्रमाण है। डेटासेट यह एक डेटा पॉइंट्स का बड़ा संग्रह होता है। डेटासेट बोहोत सारे अलगअलग प्रकार और संरचनाका होता है, और बोहोत बार किसी स्त्रोतपे आधारित होता है। उदाहरण के लिए, किसी कम्पनी की कमाई स्प्रेडशीट मैं जतन की हो सकती है मगर प्रति घंटे के दिल की धकड़न की गति [JSON](https://stackoverflow.com/questions/383692/what-is-json-and-what-is-it-used-for/383699#383699) रूप मैं हो सकती है। डेटा वैज्ञानिकोकेलिए अलग अलग प्रकार के डेटा और डेटासेट के साथ काम करना आम बात होती है। 

यह पाठ डेटा को उसके स्त्रोत के हिसाब से पहचानने और वर्गीकृत करने पे केंद्रित है।

## [पाठ के पाहिले की परीक्षा](https://red-water-0103e7a0f.azurestaticapps.net/quiz/4)

## डेटा का वर्णन कैसे किया जाता है 
**अपक्व डेटा** ऐसे प्रकार का डेटा होता जो उसके स्त्रोत से आते वक्त जिस अवस्था मैं था वैसे ही है और उसका विश्लेषण या वर्गीकरण नहीं किया गया है। ऐसे डेटासेट से जरूरी जानकारी निकलने के लिए उसे ऐसे प्रकार मे लाना आवश्यक है जो इंसान समज सके और जिस टैकनोलजीका  उपयोग डेटा के विश्लेषण मे किया जाएगा उसको भी समज आये। डेटाबेसकी संरचना हमे बताती है की डेटा किस प्रकार से वर्गीकृत किया गया है और उसका  संरचित, मिश्र संरचित और असंरचित प्रकार मै वर्गीकरण कैसे किया जाता है। संरचना के प्रकार डेटा के स्त्रोत के अनुसार बदल सकते है मगर आखिर मै इन तीनो मैं से एक प्रकार के हो सकते है। 

### परिमाणात्मक डेटा 
परिमाणात्मक डेटा मतलब डेटासेट मे उपलब्ध होने वाला ऐसा संख्यात्मक डेटा जिसका इस्तमाल विश्लेषण,मापन और गणितीय चीजोंकेलिए हो सकता है। परिमाणात्मक डेटा के यह कुछ उदाहरण है: देश की जनसंख्या, इंसान की ऊंचाई या कंपनी की तिमाही कमाई। थोड़े अधिक विश्लेषण के बाद परिणामात्मक डेटा से मौसम के अनुसार वायु गुणवत्ता सूचकांक(Air Quality Index) के बदलाव पता करना या फिर किसी सामान्य कार्यदिवस पर भीड़भाड़ वाले घंटे के ट्रैफिक की संभावना का अनुमान लगना मुमकिन है.

### गुणात्मक डेटा 
गुणात्मक डेटा, जिसे वर्गीकृत डेटा भी कहा जाता है, यह एक डेटा का ऐसा प्रकार है जिसे परिमाणात्मक डेटा की तरह वस्तुनिष्ठ तरहसे नापा नहीं जा सकता। यह आम तौर पर अलग अलग प्रकार का आत्मनिष्ठ डेटा होता है जिस से किसी उत्पादन या प्रक्रिया की गुणवत्ता। कभी कभार गुणात्मक डेटा सांखिक स्वरुपमैं होके भी गणितीय कारणों के लिए इस्तमल नहीं किया जा सकता, जैसे की फोन नंबर या समय। गुणात्मक डेटा के यह कुछ उदाहरण हो सकते है: विडिओकी टिप्पणियाँ, आपके करीबी दोस्त के गाड़ी के पसंदिता रंग का नमूना बनाना। गुणात्मक डेटा का इस्तमाल करके ग्राहकोंको कोनसा उत्पादन सबसे ज्यादा पसंद आ रहा है या फिर नौकरी आवेदन के रिज्यूमे मैं सबसे ज्यादा इस्तमाल होने वाले शब्द ढूंढ़ना।

### संरचित डेटा 
संरचित डेटा वह डेटा है जो पंक्तियों और स्तंभों में संगठित होता है, जिसके हर पंक्तिमे समान स्तंभ होते है. हर स्तंभ एक विशिष्ट प्रकार के मूल्य को बताता है और उस मूल्यको दर्शाने वाले अनाम के साथ जाना जाता है. जबकी पंक्तियाँ मे वास्तविक मूल्य होते है। हर मूल्य सही स्तम्भ का प्रतिनिधित्व करते है की नहीं ये निश्चित करने के लिए स्तंभमे अक्सर मूल्यों पर नियमोंका प्रतिबन्ध लगा रहता है. उदाहरणार्थ कल्पना कीजिये ग्राहकोंकी जानकारी होने वाला एक स्प्रेडशीट फ़ाइल जीके हर पंक्तिमे फोन क्रमांक होना जरुरी है और फोन क्रमांकमे कभीभी वर्ण या व्यंजन नहीं रहते। तो फिर फोन क्रमांक के स्तंभ पर ऐसा नियम लगा होना चाहिए जिससे ये निश्चित हो की बह कभीभी खाली नहीं है और उसमें सिर्फ आकड़े ही है.

सरंचित डेटा का यह फायदा है की उसे स्तंभ और पंक्तियोंमे वर्गीकृत किया जा सकता है. तथापि, डेटा को एक विशिष्ट प्रकार मै वर्गीकृत करने के लिए आयोजित किये जाने के बजह से पुरे संरचना मे बदल करना बोहोत मुश्किल का काम होता है. जैसे की ग्राहकोंके जानकारी वाले स्प्रेडशीट फ़ाइलमे अगर हमें ईमेल आयडी खाली ना होने वाला नया स्तंभ जोड़ना हो तो हमे ये पता करना होगा की पहिलेसे जो मूल्य इस डेटासेट मे है उनका क्या होगा.  

संरचित डेटा के यह कुछ उदाहरण है: स्प्रेडशीट, रिलेशनल डेटाबेस, फोन नंबर, बैंक स्टेटमेंट

### असंरचित डेटा
असंरचित डेटा आम तौर पर स्तंभ और पांक्तोयोंमे वर्गीकृत नहीं किया जा सकता और किसी नियमोंसे बंधित भी नहीं रहता। संरचित डेटा के तुलना से असंरचित डेटा मैं कम नियम होने के कारण उसमे नया डेटा डालना बोहोत आसान होता है। अगर कोही सेंसर जो तापमानमापक के प्रेशर का दबाव हर दो मिनिट बाद दर्ज करता है, जिसके बजह से वह तापमान को मापके दर्ज कर सकता है, तो उसे असंरचित डेटा होने के कारण डेटाबेसमे पहिलेसे होने वाले डेटा को बदलने की आवश्यकता नहीं है। तथापि, ऐसे डेटा का विश्लेषण और जांच करने को ज्यादा समय लग सकता है।  
जैसे की, एक वैज्ञानिक जिसे सेंसर के डेटा से पिछले महीने के तापमान का औसत ढूंढ़ना हो, मगर वो देखता है की सेंसर ने कुछ जगह आधेअधूरे डेटा को दर्ज करने के लिए आम क्रमांक के बजाय 'e' दर्ज किया है, जिसका मतलब है की डेटा अधूरा  है।  
असंरचित डेटा के उदाहरण: टेक्स्ट फ़ाइलें, टेक्स्ट मेसेजेस, विडिओ फ़ाइलें।

### मिश्र संरचित डेटा 

मिश्र संरचित डेटा के ऐसे कुछ गन है जिसके बजह से उसे संरचित और असंरचित डेटा का मिश्रण कहा जा सकता है. वह हमेशा स्तंभ और पंक्तियोंके अनुरूप नहीं रहता मगर ऐसे तरह संयोजित किया गया होता है की उसे संरचित कहा जा सकता है और शायद किसी ठराविक नियमोंका पालन भी कर  है। डेटा की संरचना उसके स्त्रोत के ऊपर निर्भर होती है जैसे की स्पष्ट अनुक्रम या फिर थोडा लचीला जिसमे नया डेटा जोड़ना आसान हो. मेटाडाटा ऐसे संकेतक होते है जिनसे डेटा का संयोजन और संग्रहीत करने मे सहायता होती है, और उन्हें डेटा के प्रकार के अनुरूप नाम भी दिए जा सकते है. मेटाडेटाके आम उदाहरण है: टैग्स, एलिमेंट्स, एंटिटीज और एट्रीब्यूट्स. उदाहरणार्थ: एक सामान्य ईमेल को उसका विषय, मायना, और प्राप्तकर्ताओंकी सूची होगी और किसको कब भेजना है उसके हिसाब से संयोजित किया जा सकता है। 

मिश्र संरचित डेटा के उदाहरण: एचटीएमएल, सीइसव्ही फाइलें, जेसन(JSON)

### डेटा के स्त्रोत 

डेटा का स्त्रोत मतलब मतलब वो जगह जहाँ डेटा सबसे पहिली बार निर्माण हुवा था, और हमेशा कहा और कब जमा किया था इसके ऊपर आधारित रहेगा। उपयोगकर्ताके द्वारा निर्माण किये हुवे डेटा को प्रार्थमिक डेटा के नाम से पहचाना जाता है जबकि गौण डेटा ऐसे स्त्रोत से आता है जिसने सामान्य काम के लिए डेटा जमा किया था। उदाहरण के लिए, वैज्ञानिकों का समूह वर्षावनमे टिप्पणियों और सूचि कमा कर रहे है तो वोप्रार्थमिक डेटा होगा और  अगर उन्होंने उस डेटा को बाकि के वैज्ञनिकोके साथ बाँटना चाहा तो वो गौण डेटा कहलाया जायेगा।  

## डेटा के स्त्रोत 
डेटा का स्त्रोत मतलब मतलब वो जगह जहाँ डेटा सबसे पहिली बार निर्माण हुवा था, और हमेशा कहा और कब जमा किया था इसके ऊपर आधारित रहेगा। उपयोगकर्ताके द्वारा निर्माण किये हुवे डेटा को प्रार्थमिक डेटा के नाम से पहचाना जाता है जबकि गौण डेटा ऐसे स्त्रोत से आता है जिसने सामान्य काम के लिए डेटा जमा किया था। उदाहरण के लिए, वैज्ञानिकों का समूह वर्षावनमे टिप्पणियों और सूचि कमा कर रहे है तो वोप्रार्थमिक डेटा होगा और  अगर उन्होंने उस डेटा को बाकि के वैज्ञनिकोके साथ बाँटना चाहा तो वो गौण डेटा कहलाया जायेगा।  

डेटाबेस यह एक सामान्य स्त्रोत है और वह होस्टिंग और डेटाबेस मेंटेनन्स सिस्टिम निर्भर होता है। डेटाबेस मेंटेनन्स सिस्टिममे उपयोगकर्ता कमांड्स जिन्हें क्वेरीज़ कहा जाता है इस्तमाल करके डेटाबेस का डेटा खोज सकते है। डेटा स्त्रोत फ़ाइल स्वरुप मे हो तो आवाज, चित्र, वीडियो, स्प्रेडशीट ऐसे प्रकार मे हो सकता है। आंतरजाल के स्त्रोत डेटा होस्ट करने के बोहोत आम तरीका है। यहां डेटाबेस तथा फाइलें खोजी जा सकती है।अप्लीकेशन प्रोगरामिंग इंटरफेस, जिन्हे 'एपीआय'(API) के नाम से जाना जाता है, उसकी मद्त से प्रोग्रामर्स डेटाको बहार के उपयोगकर्ताओको आंतरजाल द्वारा इस्तमाल करने के लिए भेज सकते है। जबकि वेब स्क्रैपिंग नामक प्रक्रियासे आंतरजाल के वेब पेज का डेटा अलग किया जा सकता है। [डेटा के साथ काम करना](https://github.com/microsoft/Data-Science-For-Beginners/tree/main/2-Working-With-Data) यह पथ अलग अलग डेटा का इस्तमाल करनेपर ध्यान देता है।
## निष्कर्ष 
यह पथ मे हमने पढ़ा की:
- डेटा क्या होता है 
- डेटा का वर्णन कैसे किया जाता है
- डेटा का वर्गीकरण कैसे किया जाता है 
- डेटा कहा मिलता है 

## 🚀 चुनौती
Kaggle यह के मुफ्त के डेटाबेस का बोहोत अच्छा स्त्रोत है। [सर्च टूल ](https://www.kaggle.com/datasets) का इस्तमाल करके कुछ मजेदार डेटासेट ढूंढे और उनमेसे तीन-चार डेटाबेस का ऐसे वर्गीकरण कीजिए:
- डेटा परिमाणात्मक है या गुणात्मक?
- डेटा संरचित, असंरचित या फिर मिश्र संरचित है?

## [पाठ के बाद वाली परीक्षा](https://red-water-0103e7a0f.azurestaticapps.net/quiz/5)

## समीक्षा और स्वअध्ययन
- माइक्रोसॉफ्ट लर्न का [Classify your data](https://docs.microsoft.com/en-us/learn/modules/choose-storage-approach-in-azure/2-classify-data) पाठ संरचित, असंरचित और मिश्र संरचित डेटा के बारे मे और अच्छेसे बताता है। 

## अभ्यास 
[डेटा का वर्गीकरण](../assignment.md)