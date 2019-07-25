---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e50387b197d68ee44a79cde6a84e5af7ffe0cb05
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .version('beta')
    .get();

```