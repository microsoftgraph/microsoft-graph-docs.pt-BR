---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a55e8153aea254eadcbd7bb8574b69e872a5a9e8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
    extensionAttributes: {
        extensionAttribute1: 'BYOD-Device'
    }
};

await client.api('/devices/{id}')
    .version('beta')
    .update(device);

```