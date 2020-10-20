---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5534e8f54394a1f5ac5f0e1dbd82fe215370c3b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .version('beta')
    .get();

```