---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fbdd8c0041e4e76f1af16b22e8ca35e2ab05e3b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .get();

```