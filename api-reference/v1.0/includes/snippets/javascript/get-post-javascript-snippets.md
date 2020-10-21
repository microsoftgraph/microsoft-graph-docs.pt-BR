---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18a9237877bb717816697f51dfaa80150079e489
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}')
    .get();

```