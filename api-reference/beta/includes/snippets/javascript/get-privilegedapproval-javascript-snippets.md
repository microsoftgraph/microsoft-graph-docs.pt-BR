---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edf92b8ae5faace33e8ad3ac983931baca01be79
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedApproval')
    .version('beta')
    .get();

```