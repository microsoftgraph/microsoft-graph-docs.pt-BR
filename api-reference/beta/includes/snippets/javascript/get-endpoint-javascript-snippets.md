---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 191ec0b1d2a6103c3b3b1e6708fcb1f6d19d5721
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints/{id}')
    .version('beta')
    .get();

```