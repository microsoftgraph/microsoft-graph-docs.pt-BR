---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7763d6999d8d7856ee00cb73dede0833a324d3bf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning')
    .version('beta')
    .expand('agentGroups')
    .get();

```