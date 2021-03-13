---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2de5d7de1d6321d9eb8e9f7f0e1ad2c846d4a7bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806161"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .get();

```