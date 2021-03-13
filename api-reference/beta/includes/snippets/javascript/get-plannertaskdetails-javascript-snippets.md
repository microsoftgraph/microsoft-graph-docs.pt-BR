---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83dad0890b2d8a9c0bda9bd143f87734334e46fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTaskDetails = await client.api('/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details')
    .version('beta')
    .get();

```