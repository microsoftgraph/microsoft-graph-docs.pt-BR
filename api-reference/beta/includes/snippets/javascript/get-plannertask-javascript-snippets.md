---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3f50f91876e70af95488daadf4a5a6ac4e41a28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTask = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh')
    .version('beta')
    .get();

```