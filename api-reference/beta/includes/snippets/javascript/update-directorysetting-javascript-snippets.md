---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16840b85f25924bfe77d907faaf75eb4f9547f91
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  values: [
    {
      name: 'name-value',
      value: 'value-value'
    }
  ]
};

await client.api('/settings/{id}')
    .version('beta')
    .update(directorySetting);

```