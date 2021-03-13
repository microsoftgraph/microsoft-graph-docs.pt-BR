---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3934762fd2a4dccac6839aa359acb54d49c93b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  name: 'Contoso HR Service Tickets',
  description: 'Connection to index HR service tickets'
};

await client.api('/connections/contosohr')
    .version('beta')
    .update(externalConnection);

```