---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89db32dc558edf3578eb6d9473e7e6a335cc94d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIn = await client.api('/auditLogs/signIns/{id}')
    .version('beta')
    .get();

```