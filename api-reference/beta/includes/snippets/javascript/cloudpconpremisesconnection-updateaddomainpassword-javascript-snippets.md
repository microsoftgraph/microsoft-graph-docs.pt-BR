---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b88f65b2cc53a1edff638ff3f96bcd9b79365b9
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAdDomainPassword = {
  adDomainPassword: "AdDomainPassword value"
};

let res = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword')
    .version('beta')
    .update(updateAdDomainPassword);

```