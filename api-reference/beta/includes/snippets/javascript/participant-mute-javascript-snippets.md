---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e287f16903e088945d927dc14f4ce6c38e86e7c7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/{id}/mute')
    .version('beta')
    .post(CommsOperation);

```