---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 490939194e9c1870bc551a3050828db4734acca8
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  displayName: "My Sample Team",
  description: "My Sample Team’s Description",
  owners@odata.bind: [
    "https://graph.microsoft.com/beta/users('userId')"
  ]
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```