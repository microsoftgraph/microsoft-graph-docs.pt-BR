---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa20e7d40f226de09d3ffbcc32de06331e5b815c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/users/{id}')
    .version('beta')
    .update(user);

```