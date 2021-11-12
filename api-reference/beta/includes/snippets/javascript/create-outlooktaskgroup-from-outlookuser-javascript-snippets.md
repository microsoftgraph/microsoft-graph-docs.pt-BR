---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c332faafa4e1fdd2a1a437372d5c568af12a989e1c011bd772679eac56cf458
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: 'Leisure tasks'
};

await client.api('/me/outlook/taskGroups')
    .version('beta')
    .post(outlookTaskGroup);

```