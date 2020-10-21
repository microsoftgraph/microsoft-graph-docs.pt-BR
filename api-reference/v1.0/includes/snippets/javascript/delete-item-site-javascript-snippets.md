---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 740e67aa6ec5c20a8731ebac84942b01c603f808
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}')
    .delete();

```