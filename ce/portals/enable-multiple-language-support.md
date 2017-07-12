---
title: "Enable multiple-language portal support in Dynamics 365 | MicrosoftDocs"
description: ""
ms.custom: ""
ms.date: 05/22/2017
ms.service: crm-online
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: article
ms.assetid: e3a00fbf-d78f-4cf1-9451-251dc37569ab
ms.reviewer: ""
author: sbmjais
ms.author: shjais
manager: sakudes
---
# Enable multiple-language portal support
Business is not confined to a single language. One portal’s surface content can now exist in multiple languages to reach customers around the world while keeping a single content hierarchy. To enable multiple languages for a portal, follow these steps after signing in to [!INCLUDE[pn-dynamics-crm](../includes/pn-dynamics-crm.md)]:

1.  [Enable languages in a [!INCLUDE[pn-dynamics-crm](../includes/pn-dynamics-crm.md)] organization.](https://technet.microsoft.com/library/dn832148.aspx)  
2.  Go to **Portals** &gt; **Website** &gt; **Websites**.
3.  Select the website to add language support to.
4.  Find the **Supported Languages** section under the **General** tab, and click the **+** button.
5.  Fill in the form, including **Portal Language** (a lookup of languages that are activated in the organization and are supported by portals) and **Publishing State**.

![Add a new portal language](media/add-new-portal-language.png "Add a new portal language")  

![Set default language for your portal](media/set-default-language-portal.png "Set default language for your portal")  

## Supported languages

The table below shows all the languages currently available out of the box. This list can be found in [!INCLUDE[pn-dynamics-crm](../includes/pn-dynamics-crm.md)] by going to **Portals** &gt; **Content** &gt; **Portal Languages**. The Portal Display Name of a language can be changed after selecting the language to change from this page. Note that the list now includes East Asian languages (Japanese, Chinese, and Korean).

| **Name**                           | **Language Code** | **LCID** | **Portal Display Name** |
|------------------------------------|-------------------|----------|-------------------------|
| Basque - Basque                    | eu-ES             | 1069     | euskara                 |
| Bulgarian - Bulgaria               | bg-BG             | 1026     | български               |
| Catalan - Catalan                  | ca-ES             | 1027     | català                  |
| Chinese - China                    | zh-CN             | 2052     | 中文(中国)              |
| Chinese - Hong Kong SAR            | zh-HK             | 3076     | 中文(香港特別行政區)    |
| Chinese - Traditional              | zh-TW             | 1028     | 中文(台灣)              |
| Croatian - Croatia                 | hr-HR             | 1050     | hrvatski                |
| Czech - Czech Republic             | cs-CZ             | 1029     | čeština                 |
| Danish - Denmark                   | da-DK             | 1030     | dansk                   |
| Dutch - Netherlands                | nl-NL             | 1043     | Nederlands              |
| English                            | en-US             | 1033     | English                 |
| Estonian - Estonia                 | et-EE             | 1061     | eesti                   |
| Finnish - Finland                  | fi-FI             | 1035     | suomi                   |
| French - France                    | fr-FR             | 1036     | français                |
| Galician - Spain                   | gl-ES             | 1110     | galego                  |
| German - Germany                   | de-DE             | 1031     | Deutsch                 |
| Greek - Greece                     | el-GR             | 1032     | Ελληνικά                |
| Hindi - India                      | hi-IN             | 1081     | हिंदी                   |
| Hungarian - Hungary                | hu-HU             | 1038     | magyar                  |
| Indonesian - Indonesia             | id-ID             | 1057     | Bahasa Indonesia        |
| Italian - Italy                    | it-IT             | 1040     | italiano                |
| Japanese - Japan                   | ja-JP             | 1041     | 日本語                  |
| Kazakh - Kazakhstan                | kk-KZ             | 1087     | қазақ тілі              |
| Korean - Korea                     | ko-KR             | 1042     | 한국어                  |
| Latvian - Latvia                   | lv-LV             | 1062     | latviešu                |
| Lithuanian - Lithuania             | lt-LT             | 1063     | lietuvių                |
| Malay - Malaysia                   | ms-MY             | 1086     | Bahasa Melayu           |
| Norwegian (Bokmål) - Norway        | nb-NO             | 1044     | norsk bokmål            |
| Polish - Poland                    | pl-PL             | 1045     | polski                  |
| Portuguese - Brazil                | pt-BR             | 1046     | português (Brasil)      |
| Portuguese - Portugal              | pt-PT             | 2070     | português (Portugal)    |
| Romanian - Romania                 | ro-RO             | 1048     | română                  |
| Russian - Russia                   | ru-RU             | 1049     | русский                 |
| Serbian (Cyrillic) - Serbia        | sr-Cyrl-CS        | 3098     | српски                  |
| Serbian (Latin) - Serbia           | sr-Latn-CS        | 2074     | srpski                  |
| Slovak - Slovakia                  | sk-SK             | 1051     | slovenčina              |
| Slovenian - Slovenia               | sl-SI             | 1060     | slovenščina             |
| Spanish (Traditional Sort) - Spain | es-ES             | 3082     | español                 |
| Swedish - Sweden                   | sv-SE             | 1053     | svenska                 |
| Thai - Thailand                    | th-TH             | 1054     | ไทย                     |
| Turkish - Turkey                   | tr-TR             | 1055     | Türkçe                  |
| Ukrainian - Ukraine                | uk-UA             | 1058     | українська              |
| Vietnamese - Vietnam               | vi-VN             | 1066     | Tiếng Việt              |

## Create content in multiple languages

In [!INCLUDE[pn-dynamics-crm](../includes/pn-dynamics-crm.md)], go to **Portals** &gt; **Content** &gt; **Web Pages** to see a list of content. For each web page, there will be a parent version of the page and a child version of the page for each language activated for the portal. To add a new localization of the page, navigate to a base page and scroll down to **Localized Content**. Click on the **+** button on the right side to create a look-up for the localized version.

![Add new localized content](media/Add-new-localized-content.png "Add new localized content")  

> [!Note]
> The configuration fields on the home page of a content page is not inherited to the existing content pages. They are used only in creation of new content pages. You must update the content page configurations individually.

If a portal will be in multiple languages, it is best to create the portal after all the languages you want have been activated in the organization. This will allow for the drop-down menu at the top of the **Web Pages** window to be translated into all the chosen languages. If languages are activated after the portal has been provisioned, this menu will not be translated into the newly activated languages.

![Multi-language dropdown](media/multi-language-dropdown.png "Multi-language dropdown")  

Knowledge articles will only be displayed if they have been translated into the language the user sets the portal to. However, forums and blogs allow for more control over how they are presented in other languages. After navigating to a forum or blog entity in [!INCLUDE[pn-dynamics-crm](../includes/pn-dynamics-crm.md)], changing the **Form Language** field will allow for control over how these entities are translated. If specific languages are defined, it will function like the knowledge articles. If the field is blank it will be agnostic and show up in all versions of the portal as the primary language of the organization.

Web link sets are the navigation links at the top of the portal. By navigating to **Portals** &gt; **Content** &gt; **Web Link Sets** you can control how this content is translated. When a language is active for the portal, a new set of links will be created for the newly activated language.

![Active weblink for new language](media/active-weblink-new-language.png "Active weblink for new language")