---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 951288fa801e43c4d376d94bf12a94b7f1b845f4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': '#microsoft.graph.socialIdentityProvider',
  displayName: 'Apple'
};

await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .update(identityProviderBase);

```