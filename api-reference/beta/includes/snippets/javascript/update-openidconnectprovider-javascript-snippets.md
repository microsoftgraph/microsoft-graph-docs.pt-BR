---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8f56fa9c1c3f45ffa3f3a92b69647fca7962107
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921209"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  responseType: 'id_token'
};

await client.api('/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7')
    .version('beta')
    .update(identityProviderBase);

```