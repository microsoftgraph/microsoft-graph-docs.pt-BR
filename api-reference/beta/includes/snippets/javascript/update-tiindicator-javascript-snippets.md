---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9725305a12db0a349566da56bc73055aae529880
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: 'additionalInformation-after-update',
  confidence: 42,
  description: 'description-after-update',
};

await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update(tiIndicator);

```