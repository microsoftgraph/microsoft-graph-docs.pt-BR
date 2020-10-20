---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17193bc57dcde8edc176f77ab3d811bd80e65402
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .delete();

```