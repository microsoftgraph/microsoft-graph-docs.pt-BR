---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be16d9d73cbf393913fbf46533bd566aed336c44
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}')
    .version('beta')
    .get();

```