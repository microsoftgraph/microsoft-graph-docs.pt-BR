---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a74448ae0a30d339556503d8e8c24c64df34d09b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRosterMember = {
  '@odata.type': '#microsoft.graph.plannerRosterMember',
  userId: 'String'
};

await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members')
    .version('beta')
    .post(plannerRosterMember);

```