---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f10f5de697bfa9a909347f1bdf34456416e06425
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610487"
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