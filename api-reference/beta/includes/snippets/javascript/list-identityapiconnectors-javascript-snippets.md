---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4435f40324cd8dc21102962ddb245f476b9b8260
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/apiConnectors')
    .version('beta')
    .get();

```