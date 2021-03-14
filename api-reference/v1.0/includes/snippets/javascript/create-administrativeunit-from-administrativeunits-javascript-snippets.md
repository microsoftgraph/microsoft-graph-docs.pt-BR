---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb9d1f7685bfb89cc0bd5f45ee099829df7b066d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Seattle District Technical Schools',
    description: 'Seattle district technical schools administration',
    visibility: 'HiddenMembership'
};

await client.api('/directory/administrativeUnits')
    .post(administrativeUnit);

```