---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da2e628b388dc29c0ba8dc56a2697f3fd2513ad9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .post();

```