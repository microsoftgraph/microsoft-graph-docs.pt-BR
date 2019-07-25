---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84e09232bb12009b4ddae007f38dc3ca77ea2b60
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .get();

```