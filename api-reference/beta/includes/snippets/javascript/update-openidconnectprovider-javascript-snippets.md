---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52014e18ea5accff108f46790a1c9d4c76f3d6b7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': '#microsoft.graph.socialIdentityProvider',
  responseType: 'id_token'
};

await client.api('/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7')
    .version('beta')
    .update(identityProviderBase);

```