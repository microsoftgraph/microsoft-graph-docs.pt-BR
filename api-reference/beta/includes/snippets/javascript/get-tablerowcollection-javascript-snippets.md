---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e71fa3a29252528d80c291e8f7a311b2a6240d0f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .get();

```