---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19a6ba5fb1a41f1b0a5fa37315caf50cdcc83e04
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```