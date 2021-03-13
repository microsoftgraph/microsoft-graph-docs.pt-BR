---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c09d067c1fe39dc245f4105d0ad7ad4b402eec10
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  templateId: 'templateId-value',
  values: [
    {
      name: 'name-value',
      value: 'value-value'
    }
  ]
};

await client.api('/settings')
    .version('beta')
    .post(directorySetting);

```