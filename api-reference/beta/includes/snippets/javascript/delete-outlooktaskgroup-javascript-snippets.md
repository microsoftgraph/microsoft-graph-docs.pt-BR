---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa6b65bbfbc0ef5b9ee05016e712bf3c82d1ce45
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620417"
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