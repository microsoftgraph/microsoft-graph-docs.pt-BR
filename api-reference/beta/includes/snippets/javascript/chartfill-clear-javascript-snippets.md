---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56834e164694d525d8d590b709921d9c5811fd75
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear')
    .version('beta')
    .post();

```