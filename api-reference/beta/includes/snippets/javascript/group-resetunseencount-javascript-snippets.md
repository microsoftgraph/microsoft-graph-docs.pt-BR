---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4a94b12db2601efbf5ff3cfec81b485bb5f4900
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/resetUnseenCount')
    .version('beta')
    .post();

```