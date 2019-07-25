---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3874501ecd3b5c90e8cb0a6ebbc428c479f10d70
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups')
    .version('beta')
    .get();

```