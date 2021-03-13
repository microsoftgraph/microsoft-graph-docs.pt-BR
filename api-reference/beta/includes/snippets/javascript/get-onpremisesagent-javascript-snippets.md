---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9db0567cc5e75388f500eeacd817a6853e898f5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesAgent = await client.api('/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/')
    .version('beta')
    .expand('agentGroups')
    .get();

```