---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01fb0a91ac79405b985d6da88d0ee2992e8e5452
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  displayName: "My Class Team",
  description: "My Class Team’s Description"
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```