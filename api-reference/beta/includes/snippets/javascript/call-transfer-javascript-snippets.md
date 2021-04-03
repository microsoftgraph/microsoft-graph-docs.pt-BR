---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16b91dc1cf0af9b392ab6656ebb5aeec1214b248
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573019"
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
  }
};

await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```