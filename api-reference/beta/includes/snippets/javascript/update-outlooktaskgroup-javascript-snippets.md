---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04dae46db287e4a92df0a4c0b599250adce41c08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: 'Personal Tasks',
};

await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .update(outlookTaskGroup);

```