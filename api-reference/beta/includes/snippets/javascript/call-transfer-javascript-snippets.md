---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94673c807e8e94d8e57b5e3776ee085446071968
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: 'default',
    identity: {
        phone: {
          '@odata.type': '#microsoft.graph.identity',
          id: '+12345678901'
        }
    },
    languageId: 'languageId-value',
    region: 'region-value'
  },
  clientContext: '9e90d1c1-f61e-43e7-9f75-d420159aae08'
};

await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```