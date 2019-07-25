---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f85d6ba0aa1c506f47f0f6b91279a0e3ccb9b61e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .version('beta')
    .get();

```