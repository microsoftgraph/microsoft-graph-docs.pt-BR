---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7283d71f273ee225a9e94182d0a0210e861fc6a3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const settings = {
    redundancyDetection: {
        isEnabled: false,
        similarityThreshold: 70,
        minWords: 12,
        maxWords: 400000
    },
    topicModeling: {
        isEnabled: false,
        ignoreNumbers: false,
        topicCount: 50,
        dynamicallyAdjustTopicCount: false
    },
    ocr: {
        isEnabled: true,
        maxImageSize: 12000
    }
};

await client.api('/compliance/ediscovery/cases/{caseId}/settings')
    .version('beta')
    .update(settings);

```