---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 528e76396e8bc1ff24f2508b419d39cfd25c3bd4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowIdentityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test'
};

await client.api('/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref')
    .version('beta')
    .update(userFlowIdentityProviders);

```