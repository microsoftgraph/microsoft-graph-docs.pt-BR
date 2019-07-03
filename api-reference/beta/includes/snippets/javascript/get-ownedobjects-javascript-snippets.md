---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3f252b5a49dd6cd1ea611a47e6f769b96ee965c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518986"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedObjects')
    .version('beta')
    .get();

```