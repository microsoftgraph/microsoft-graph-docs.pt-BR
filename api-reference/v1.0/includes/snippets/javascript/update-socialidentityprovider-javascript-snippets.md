---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0ce1f0740630200fc211f7de44b43590bb1696a
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': 'microsoft.graph.socialIdentityProvider',
  clientSecret: '1111111111111'
};

await client.api('/identity/identityProviders/Amazon-OAUTH')
    .update(identityProviderBase);

```