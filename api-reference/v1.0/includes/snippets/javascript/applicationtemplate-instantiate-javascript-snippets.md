---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a89e82cdfbe57a53040b00dcb9ddea67ce4d2a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: 'My custom name'
};

await client.api('/applicationTemplates/{id}/instantiate')
    .post(applicationServicePrincipal);

```