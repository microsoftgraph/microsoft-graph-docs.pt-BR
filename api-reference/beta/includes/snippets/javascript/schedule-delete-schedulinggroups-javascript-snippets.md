---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28283566fb366d20cd0c0f08ab08afd5b270c367ca3f2575d989a15a965fb392
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .version('beta')
    .delete();

```