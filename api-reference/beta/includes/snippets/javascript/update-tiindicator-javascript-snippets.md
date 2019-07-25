---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f62830d67a9a05603cc2801ff9e494228f948fd3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: "additionalInformation-after-update",
  confidence: 42,
  description: "description-after-update",
};

let res = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update({tiIndicator : tiIndicator});

```