# 智能毕业纪念APP

## 产品需求

| 发布日期   | 2019.12.3    |
| ---------- | --- |
| 文件名称   |  智能毕业纪念APP   |
| 文件现状   | 完善中    |
| 文件的主人 | 林咏妍    |
| 设计师     | 林咏妍    |
| 开发者     | 林咏妍    |
| 测试者     | 林咏妍    |

## 目标

建立一个动态的毕业回忆录，根据学校的地标和用户自定标签分类整理用户的回忆，并且每个普通用户能关联5个用户，查看他们的回忆。用户可根据自己的需求建立动态毕业册和定制毕业纪念品。

## 背景和战略契合处

- 背景：学生毕业时都希望自己有一本毕业纪念册，但是非常多学校都没有官方的毕业纪念册，学生自发组织创建毕业册。但纸质毕业册制作费用较贵，并且需要学生自己去找商家，比较麻烦，而且传统相册没有活动，不能满足学生需求。

- 战略契合处：

             1.满足毕业生动态毕业册的需求。

             2.能够让毕业生找到同校毕业生，建立毕业生组织。

             3.关联用户后，可看到关联用户的回忆，寻找记忆的共同点。

             4.能在APP上进行毕业纪念品的定制，不需要学生重新去找商家。

             5.根据地图去整理回忆，能看到学校的状况和变化。

## 假设条件

- 用户在使用手机时：

1.首页能够看到学校的平面和立体地图，可以对地图进行放大和缩小，点击地图相应图标建筑可以进行该地的回忆查看

2.进入同校的讨论区，在讨论区内进行交流，寻找校友，成立校友会。

3.进入购买页面，可以购买本校的周边产品，并且联系APP提供的商家进行周边的定制。

4.查看关联人物时，可以关联不同学校的人，进入关联人页面后，能查看他的学校地图和回忆，但不能查看他关联的人。

## 需求

| #   | 标题     | 用户故事                                                                    | 重要性 | 笔记 |
| --- | -------- | --------------------------------------------------------------------------- | ------ | ---- |
| 1   | 查看回忆 | 毕业很久了，以前的照片不见了，想找回之前的记忆。打开手机APP能看到大学时的照片，找回之前的记忆 |必须有        | 必须在当时毕业时绑定手机号、QQ号、微信号或微博，将记忆导入，否则无法寻找     |
| 2   | 寻找校友 |  想找以前的校友，但是没有途径，学校的校友群范围太大，不能精准找到专业的校友                                                                           | 必须有       | 只能寻找本校校友，不能寻找外校     |
| 3   | 关联人物 | 想查看挚友和恋人的大学记忆，但是他跟我不同一个学校，我要寻找跟他同校的人才能看                           |   必须有     | 每人只能关联5个人物，关联更多需要充值会员     |
|  4    | 购买周边 | 想购买或者定做大学的周边，但是没有途径 | 必须有 | APP只提供购买渠道和退货渠道，如果没有相关产品不负责提供 |


## PRD价值主张设计

![价值主张设计](https://images.gitee.com/uploads/images/2019/1120/194330_bf91a14c_1532294.png "价值主张设计")


### PRD1 加值宣言

##### 以微软azure API为例

- 人脸识别：查看回忆的照片时，通过人脸识别，可以看到跟你一起拍照的人的基本信息，包括姓名、性别、年级、院系、专业。

- 计算机影像：

         
             1.识别名人和地标：上传照片时，自动识别图片中的位置，将图片放到合适的地标中。
           
             2.生成缩略图：当你点击地标时，地标上方会显示你在该地记忆图片的相关缩略图。


- 内容审查器：图像/文本审查对用户上传的内容进行审查，不符合互联网规范的内容会禁止上传。

- 文本翻译：轻松并准确地检测任何文本字符串的语言，可简化开发过程并快速发送翻译或提供本地化内容。

- 语音服务：将语音转换为文本，实现直观的交互，用户可以进行声音的记录，也可将声音转为文字保留下来。

### PRD2 核心价值 

- 人脸识别：用户注册账号后，需要上传自己的照片，搜索并识别人脸，使用APP提供的同校数据标记人员和组并进行搜索，以便与先前未看的人脸相匹配。

- 计算机影像：除了能够识别学校的特定地标，地标模型识别功能可识别全世界 9000 个自然和人工地标，满足用户的需求。

- 内容审查器：从根源上阻止不合乎规范的内容上传。

- 文本翻译：翻译语言，提供中文简体、中文繁体和英语三种语言。

- 语音服务：定制语音识别模型，以适应用户的说话风格、表达方式和特有词汇，以及背景噪音、口音和语音模式，轻松记录你的语言。

### PRD3 核心价值与用户痛点

- **痛点一：用户想要知道跟他一起拍照的是哪位同学，跟他有什么共同的记忆。** 


            采用人脸识别，快速识别出同学，并寻找与他的共同图片。


- **痛点二：用户忘记了图片中的地方是哪里，或者学校环境变了，用户想要知道之前的照片在哪里拍的。**


            采用计算机影像，识别图片中的地标，快速帮用户找到地标。


- **痛点三：用户的关联人在港澳台读书，用户看不懂繁体中文或者英文。**

           
            采用文本翻译，支持简体中文、繁体中文和英文互转，满足内容本地化需求。


- **痛点四：用户普通话不标准，或者想要记录下方言词汇，打字无法满足需求。**


         采用语音服务，定制语音识别模型，以适应用户的说话风格、表达方式和特有词汇，以及背景噪音、口音和语音模式，记录你的语言。


### PRD4 人工智能概率性与用户痛点

- **人脸识别API：** 检测图像中的一张或多张人脸，获取图像中人脸所在位置背面的矩形，以及包含基于机器学习的面部特征预测的人脸属性。提供的 面部属性特征包括：年龄、表情、性别、姿势、微笑和面部毛发，以及图像中每张脸上的 27 个特征点，准确率>95%。

- **计算机影像API：**

- 识别名人和地标：名人模型识别功能可识别 20 万商业、政治、体育和娱乐界名人。地标模型识别功能可识别全世界 9000 个自然和人工地标。特定于域的模型是计算机影像 API 内不断发展的功能，准确率>95%。

- 生成缩略图：基于任何输入图像生成充分利用存储空间的高质量缩略图。使用缩略图生成来修改图像，从而最好地满足你的大小、形状和风格需要。应用智能裁剪来生成与原始图像纵横比不同却保留感兴趣区域的缩略图，准确率>95%。

- **内容审查器API：** 通过基于机器学习的分类器、自定义列表和光学字符识别技术 (OCR)，增强检测可能具有冒犯性或不必要的图像的能力；使用内容筛选来检测 100 多种语言中潜在的猥亵语言，根据上下文（公共预览版）标记可能被视为不当的文本，并将文本与自定义列表进行匹配。内容审查器还可帮助检查个人身份信息 (PII)；启用计算机辅助内容审查，检测视频中可能存在的色情和低俗内容。视频审查服务（公共预览版）作为 Azure 媒体服务的一部分提供，准确率>95%。

- **文本翻译API：** 自动检测语言，轻松并准确地检测任何文本字符串的语言，可简化开发过程并快速发送翻译或提供本地化内容。

- **语音服务API：** 轻松将实时语音到文本功能添加到应用程序中，以用于语音命令、对话听录和调用中心日志分析等方案。定制语音识别模型，以适应用户的说话风格、表达方式和特有词汇，以及背景噪音、口音和语音模式。准确率>95%。

### PRD5 需求列表与人工智能API加值

###### 核心功能的排序

1.用户照片查看： 

- 人脸识别API，不仅能看自己的照片，还能寻找跟你们拍照的人的共同回忆。

- 计算机影像API： 地标识别功能 ，识别照片中的地标  

- 语音服务API：对照片进行记录，通过语音转文字进行记录，既能记录下语音，也能记录下文字。 
         
2.关联人物查看： 

- 文本翻译API：查看关联人物的记忆，了解他的大学生活。

3.社区交流： 

- 内容审查API：对于上传的内容进行审查，发现不规范的内容不予上传。

4.购买周边



## API产品使用关键AI或机器学习之API的输出入展示 

### API1 使用水平

- #### 人脸识别API：面部检测

```
import requests
import json

# set to your own subscription key value
subscription_key = None
assert subscription_key

# replace <My Endpoint String> with the string from your endpoint URL
face_api_url = 'https://<My Endpoint String>.com/face/v1.0/detect'

image_url = 'https://upload.wikimedia.org/wikipedia/commons/3/37/Dagestani_man_and_woman.jpg'

headers = {'Ocp-Apim-Subscription-Key': subscription_key}

params = {
    'returnFaceId': 'true',
    'returnFaceLandmarks': 'false',
    'returnFaceAttributes': 'age,gender,headPose,smile,facialHair,glasses,emotion,hair,makeup,occlusion,accessories,blur,exposure,noise',
}

response = requests.post(face_api_url, params=params,
                         headers=headers, json={"url": image_url})
print(json.dumps(response.json()))
```

- #### 计算机影像API：识别名人和地标

```
import requests
# If you are using a Jupyter notebook, uncomment the following line.
# %matplotlib inline
import matplotlib.pyplot as plt
from PIL import Image
from io import BytesIO

# Add your Computer Vision subscription key and endpoint to your environment variables.
if 'COMPUTER_VISION_SUBSCRIPTION_KEY' in os.environ:
    subscription_key = os.environ['COMPUTER_VISION_SUBSCRIPTION_KEY']
else:
    print("\nSet the COMPUTER_VISION_SUBSCRIPTION_KEY environment variable.\n**Restart your shell or IDE for changes to take effect.**")
    sys.exit()

if 'COMPUTER_VISION_ENDPOINT' in os.environ:
    endpoint = os.environ['COMPUTER_VISION_ENDPOINT']

analyze_url = endpoint + "vision/v2.1/analyze"

# Set image_path to the local path of an image that you want to analyze.
image_path = "C:/Documents/ImageToAnalyze.jpg"

# Read the image into a byte array
image_data = open(image_path, "rb").read()
headers = {'Ocp-Apim-Subscription-Key': subscription_key,
           'Content-Type': 'application/octet-stream'}
params = {'visualFeatures': 'Categories,Description,Color'}
response = requests.post(
    analyze_url, headers=headers, params=params, data=image_data)
response.raise_for_status()

# The 'analysis' object contains various fields that describe the image. The most
# relevant caption for the image is obtained from the 'description' property.
analysis = response.json()
print(analysis)
image_caption = analysis["description"]["captions"][0]["text"].capitalize()

# Display the image and overlay it with the caption.
image = Image.open(BytesIO(image_data))
plt.imshow(image)
plt.axis("off")
_ = plt.title(image_caption, size="x-large", y=-0.1)
```

- #### 计算机影像API：生成缩略图

```
import requests
# If you are using a Jupyter notebook, uncomment the following line.
# %matplotlib inline
import matplotlib.pyplot as plt
from PIL import Image
from io import BytesIO

# Add your Computer Vision subscription key and endpoint to your environment variables.
if 'COMPUTER_VISION_SUBSCRIPTION_KEY' in os.environ:
    subscription_key = os.environ['COMPUTER_VISION_SUBSCRIPTION_KEY']
else:
    print("\nSet the COMPUTER_VISION_SUBSCRIPTION_KEY environment variable.\n**Restart your shell or IDE for changes to take effect.**")
    sys.exit()

if 'COMPUTER_VISION_ENDPOINT' in os.environ:
    endpoint = os.environ['COMPUTER_VISION_ENDPOINT']

thumbnail_url = endpoint + "vision/v2.1/generateThumbnail"

# Set image_url to the URL of an image that you want to analyze.
image_url = "https://upload.wikimedia.org/wikipedia/commons/9/94/Bloodhound_Puppy.jpg"

headers = {'Ocp-Apim-Subscription-Key': subscription_key}
params = {'width': '50', 'height': '50', 'smartCropping': 'true'}
data = {'url': image_url}
response = requests.post(thumbnail_url, headers=headers,
                         params=params, json=data)
response.raise_for_status()

thumbnail = Image.open(BytesIO(response.content))

# Display the thumbnail.
plt.imshow(thumbnail)
plt.axis("off")

# Verify the thumbnail size.
print("Thumbnail is {0}-by-{1}".format(*thumbnail.size))
```

- #### 内容审查器API


```
import os.path
from pprint import pprint
import time
from io import BytesIO
from random import random
import uuid

from azure.cognitiveservices.vision.contentmoderator import ContentModeratorClient
import azure.cognitiveservices.vision.contentmoderator.models
from msrest.authentication import CognitiveServicesCredentials
```

- #### 文本翻译API

```
key_var_name = 'TRANSLATOR_TEXT_SUBSCRIPTION_KEY'
if not key_var_name in os.environ:
    raise Exception('Please set/export the environment variable: {}'.format(key_var_name))
subscription_key = os.environ[key_var_name]

endpoint_var_name = 'TRANSLATOR_TEXT_ENDPOINT'
if not endpoint_var_name in os.environ:
    raise Exception('Please set/export the environment variable: {}'.format(endpoint_var_name))
endpoint = os.environ[endpoint_var_name]
```


- #### 语音服务API

```
$SpeechServiceURI =
'https://speech.platform.bing.com/speech/recognition/interactive/cognitiveservices/v1?language=en-us&format=detailed'

# $OAuthToken is the authorization token returned by the token service.
$RecoRequestHeader = @{
  'Ocp-Apim-Subscription-Key' = 'YOUR_SUBSCRIPTION_KEY';
  'Transfer-Encoding' = 'chunked';
  'Content-type' = 'audio/wav; codec=audio/pcm; samplerate=16000'
}

# Read audio into byte array
$audioBytes = [System.IO.File]::ReadAllBytes("YOUR_AUDIO_FILE")

$RecoResponse = Invoke-RestMethod -Method POST -Uri $SpeechServiceURI -Headers $RecoRequestHeader -Body $audioBytes

# Show the result
$RecoResponse
```

### API2 使用比较分析

- 一开始考虑的是微软azure的API，最后使用的也是微软azure的API。我查阅了百度的API和微软azure的API，在生成缩略图这一部分，微软azure拥有此功能，而百度没有，其他使用的API，百度也拥有。因此综合来看，选择了微软azure的API。

- 在内容审查器上曾经设想过使用百度API的自然语言处理API，但因为百度的自然语言处理API分级太多，分区太细。在调用API时需要调用多个API进行检测，虽然检测得会更加精细，但是因为太麻烦，因此选择检测相对没有那么精细，但是调用方便的微软azure的内容审查器API。

### API3 使用后风险报告 

- 目前微软azure的API精确度较高，但在使用语音服务API时，还是无法完全准确的识别文字，对于带有方言口音的普通话识别度不高，而且没有识别粤语的选项，无法满足用户的需求。

- 尝试内容审查器API，输入在小说网站上被认定为“敏感文本”的文字，例如人体部位，azure都能识别出来，并进行**的标记。上传电影《五十度黑》进行测试时，azure发出提醒并阻止该内容，说明内容审查器API能满足此APP的需求。

### API4 加分项

见PRD2 核心价值