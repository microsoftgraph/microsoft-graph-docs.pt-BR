---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86efc52ecf3f329f631cbefb8a9ebe8875796a12
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .get();

```