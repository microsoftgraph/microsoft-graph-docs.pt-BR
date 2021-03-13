---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e971b9a6e2956f1300c1491cc2565ad78ddcf714
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  '@odata.id': 'https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}'
};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref')
    .version('beta')
    .post(connectorGroup);

```