---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3308613031b767470cfccac5dc560c731a0c308
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/Range')
    .version('beta')
    .post();

```