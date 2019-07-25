---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa6b65bbfbc0ef5b9ee05016e712bf3c82d1ce45
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .delete();

```