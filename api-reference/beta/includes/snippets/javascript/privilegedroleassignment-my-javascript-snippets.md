---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fa7c27e7b2360818f576d9381ab8cf61d113bae
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/my')
    .version('beta')
    .get();

```