---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d636417de97e4c3a56392cd7b21de07ef33d31a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .delete();

```