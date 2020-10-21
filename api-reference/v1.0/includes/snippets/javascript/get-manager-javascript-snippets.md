---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a70bdc11967e30b239d0d64ba4c2b274409eea4f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/manager')
    .get();

```