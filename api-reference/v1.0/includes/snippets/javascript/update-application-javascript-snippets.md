---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1df57396b6029ddae55744a6c7c58d098d7d1eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  displayName: 'New display name'
};

await client.api('/applications/{id}')
    .update(application);

```