---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24c83fcd169859ca77526cd97505af3b38c90abb
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/transitiveMemberOf')
    .get();

```