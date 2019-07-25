---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbd71f1137e25ff96640d98d58536f5a4811980d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709151"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Social events"
};

let res = await client.api('/me/calendar')
    .version('beta')
    .update({calendar : calendar});

```