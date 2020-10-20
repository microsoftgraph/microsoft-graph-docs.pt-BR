---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 624517e7f1bff2c07e29277e2ad8e3c734f5c6ed
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```