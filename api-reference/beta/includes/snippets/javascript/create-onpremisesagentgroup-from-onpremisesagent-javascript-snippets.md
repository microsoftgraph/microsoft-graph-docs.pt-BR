---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daeecf8b4af0cc8c44af2f60f9926f05142c299e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref')
    .version('beta')
    .post();

```