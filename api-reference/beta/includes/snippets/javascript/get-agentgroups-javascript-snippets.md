---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49e4da040f342c6f7f87d8b54d99e10de40a0bd5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agentGroups = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .expand('agents,publishedResources')
    .get();

```