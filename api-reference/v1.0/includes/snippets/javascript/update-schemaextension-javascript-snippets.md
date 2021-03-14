---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bcc72f9c714762fa4ce18cf29704b0814e8863c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
  properties: [
    {
      name: 'new-name-value',
      type: 'new-type-value'
    },
    {
      name: 'additional-name-value',
      type: 'additional-type-value'
    }
  ]
};

await client.api('/schemaExtensions/{id}')
    .update(schemaExtension);

```