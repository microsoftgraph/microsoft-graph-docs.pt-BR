---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 512bd57f245ec1a01fbaea3916138b645d865d73
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}')
    .version('beta')
    .get();

```