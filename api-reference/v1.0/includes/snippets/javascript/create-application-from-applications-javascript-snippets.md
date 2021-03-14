---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bef72d6b5457824344b60b382fd5c26c064e7ec1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'Display name'
};

await client.api('/applications')
    .post(application);

```