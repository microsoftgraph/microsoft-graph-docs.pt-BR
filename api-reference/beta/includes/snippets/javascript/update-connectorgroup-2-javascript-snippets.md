---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 250b41b7e91ec6225cd8b4e5ae79d156319529f2240de98335904429f9df6fba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156258"
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