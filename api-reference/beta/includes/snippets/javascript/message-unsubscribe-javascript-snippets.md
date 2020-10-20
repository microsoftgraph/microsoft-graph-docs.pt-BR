---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcfc6b6f0d660256d3764849facd6330d1e498ab
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/unsubscribe')
    .version('beta')
    .post();

```