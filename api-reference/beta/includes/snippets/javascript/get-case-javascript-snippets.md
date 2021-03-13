---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 922749451e4dbda1c0f23b13b0328f95989698fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _case = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .get();

```