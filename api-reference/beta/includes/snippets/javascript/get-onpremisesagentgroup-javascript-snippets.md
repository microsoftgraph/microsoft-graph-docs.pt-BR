---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42c8c6ed8fd37f490b4086a48709bde3f84ece9bc15f767c7544cec2f62bc137
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesAgentGroup = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/')
    .version('beta')
    .expand('agents')
    .get();

```