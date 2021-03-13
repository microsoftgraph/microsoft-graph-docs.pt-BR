---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69dcdda798de5ac85260f30958ea945b5882a1e6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks')
    .version('beta')
    .get();

```