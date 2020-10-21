---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e775e342f3e317174b2a01f0f3960d1ee53f089d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .get();

```