---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc73682911d58aae7f4faccd4358814eaea8bb9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: 'name-value',
  region: 'region-value'
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}')
    .version('beta')
    .update(connectorGroup);

```