---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 323ae24e7a1adf27b59a75e3be43f4bf472aab69
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .get();

```