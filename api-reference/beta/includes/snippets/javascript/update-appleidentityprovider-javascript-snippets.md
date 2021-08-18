---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3c6c4fb7fa59b5b57f0d7cb8a84e66a60b1a9e74583b9ee6db40c6b54415785
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899763"
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
    .version('beta')
    .update(identityProviderBase);

```