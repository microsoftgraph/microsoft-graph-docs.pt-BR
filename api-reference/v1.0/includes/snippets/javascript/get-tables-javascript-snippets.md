---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff3943137225eeb44c9ffe9c67fe744c584d2917
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .get();

```