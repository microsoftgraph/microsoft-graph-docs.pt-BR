---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c584d7048126f4d41af819850f92d5f2bdceaf5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  'template@odata.bind': 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
  'group@odata.bind': 'https://graph.microsoft.com/v1.0/groups(\'groupId\')'
};

await client.api('/teams')
    .version('beta')
    .post(team);

```