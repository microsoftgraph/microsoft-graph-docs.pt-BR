---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b3b0d904298615f36c14a1ee934a3f07965eb6b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: 'displayName-value',
    templateId: 'templateId-value',
    values: [
      {
        name: 'name-value',
        value: 'value-value'
      }
    ]
  }
};

await client.api('/groups/{id}/settings')
    .version('beta')
    .post(directorySetting);

```