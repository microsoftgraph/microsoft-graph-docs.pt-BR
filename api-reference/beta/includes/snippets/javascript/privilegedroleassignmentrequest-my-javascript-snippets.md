---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1bd8b70883aefeae797752f6c2b31e0f37e8d22
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignmentRequests/my')
    .version('beta')
    .get();

```