---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a99fd5cd2f260cbeb1ce6f53dc66b8748fca8270
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sets = await client.api('/termStore/groups/{groupId}/sets')
    .version('beta')
    .get();

```