---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d615ef458bdcfeb53e32496a822ac64ee9fe916
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const caseSettings = {
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
    .update(caseSettings);

```