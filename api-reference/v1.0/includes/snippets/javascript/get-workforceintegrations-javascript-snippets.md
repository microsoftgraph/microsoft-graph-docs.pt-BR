---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2c3c4ba9014f539b159b9f2e51092b12bfc5801
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegrations = await client.api('/teamwork/workforceIntegrations')
    .get();

```