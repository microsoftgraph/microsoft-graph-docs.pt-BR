---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fb9c6bcb3e5c3fb59cfca1d82a7099bbba60c20
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .delete();

```