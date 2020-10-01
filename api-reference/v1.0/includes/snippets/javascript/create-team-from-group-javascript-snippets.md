---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c92b87164050bb0ffcd118cb8852c76a32c46b84
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2020
ms.locfileid: "48315270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  group@odata.bind: "https://graph.microsoft.com/v1.0/groups('groupId')"
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```