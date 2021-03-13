---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61c5896d1026d8623a83bb0a7bd1fb2e3bf21a3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
    defaultDisplayLanguage: {
        locale: 'en-US'
    },
    authoringLanguages: [
        {
            locale: 'fr-FR'
        },
        {
            locale: 'de-DE'
        }
    ],
    defaultTranslationLanguage: {
        locale: 'en-US'
    },
    defaultSpeechInputLanguage: {
        locale: 'en-US'
    },
    defaultRegionalFormat: {
        locale: 'en-GB'
    },
    regionalFormatOverrides: {
        calendar: 'Gregorian Calendar',
        firstDayOfWeek: 'Sunday',
        shortDateFormat: 'yyyy-MM-dd',
        longDateFormat: 'dddd, MMMM d, yyyy',
        shortTimeFormat: 'HH:mm',
        longTimeFormat: 'h:mm:ss tt',
        timeZone: 'Pacific Standard Time'
    },
    translationPreferences: {
        translationBehavior: 'Yes',
        languageOverrides: [
            {
                languageTag: 'fr',
                translationBehavior: 'Yes' 
            }
        ]
     }
};

await client.api('/me/settings/regionalandlanguagesettings')
    .version('beta')
    .put(regionalAndLanguageSettings);

```