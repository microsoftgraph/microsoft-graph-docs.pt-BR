---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af591270fcb5528cfa25cf5004ad092fbcc38d26
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .get();

```