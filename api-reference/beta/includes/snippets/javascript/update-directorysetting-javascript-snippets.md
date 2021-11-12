---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4a41698cf358e66d9e2397fb638143d6d5faf18ddeca9998679e30b1fb5dc5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899805"
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