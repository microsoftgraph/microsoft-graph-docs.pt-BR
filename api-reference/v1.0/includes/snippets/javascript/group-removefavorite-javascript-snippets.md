---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: affc1001ae55c71c5b7c94d333311a9d71296cc1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/removeFavorite')
    .post();

```