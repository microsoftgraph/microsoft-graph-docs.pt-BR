---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b9032f1b05a19c85ac8394f542e92d0b59f394a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastColumn')
    .get();

```