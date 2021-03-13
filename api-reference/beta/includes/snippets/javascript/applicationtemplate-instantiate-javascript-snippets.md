---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39dcede4f3354df9d03e95660b577e8b14dd928e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779345"
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
    .version('beta')
    .post(applicationServicePrincipal);

```