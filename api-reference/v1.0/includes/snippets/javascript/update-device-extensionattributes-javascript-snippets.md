---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66c8a4d3d78e48ae3af4d061001b9adfc0765ef9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696852"
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
    .update(device);

```