---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4516f75c2ac3f306696b8a2aabbcd126ce85b364
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  displayName: 'Apple'
};

await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .update(identityProviderBase);

```