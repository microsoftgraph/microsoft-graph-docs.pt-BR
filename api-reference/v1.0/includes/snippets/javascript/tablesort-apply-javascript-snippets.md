---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 633f2fc790d1e57bdce491d22c9ccc15bdf2942d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  fields: [
    {
      key: 99,
      sortOn: "sortOn-value",
      ascending: true,
      color: "color-value",
      dataOption: "dataOption-value",
      icon: {
        set: "set-value",
        index: 99
      }
    }
  ],
  matchCase: true,
  method: "method-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply')
    .post(apply);

```