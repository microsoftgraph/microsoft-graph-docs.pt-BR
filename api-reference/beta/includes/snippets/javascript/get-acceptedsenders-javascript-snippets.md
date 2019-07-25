---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f10f5de697bfa9a909347f1bdf34456416e06425
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/acceptedSenders')
    .version('beta')
    .get();

```