---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3060921e418909d368b80c156f1cc5e6c832ebaa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{driveId}')
    .version('beta')
    .get();

```