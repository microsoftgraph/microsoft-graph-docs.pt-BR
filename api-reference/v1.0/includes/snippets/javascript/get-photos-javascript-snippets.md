---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee2ff962a98f4a4d0cdf3b2429d9131a8da22787
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613827"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .get();

```