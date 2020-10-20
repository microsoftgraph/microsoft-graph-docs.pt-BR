---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5f8ddb3e5c3dadf91625304cbcf6c672b19cbea
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}')
    .version('beta')
    .delete();

```