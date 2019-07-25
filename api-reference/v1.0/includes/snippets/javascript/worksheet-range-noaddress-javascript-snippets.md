---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcead142be60368a6674669501d84aba940c04b8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/range')
    .get();

```