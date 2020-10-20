---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfbb178b7cdb481d0db75c38292dd76929e4b159
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .version('beta')
    .get();

```