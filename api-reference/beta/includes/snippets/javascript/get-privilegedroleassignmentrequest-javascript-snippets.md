---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12b3d66ceca7a522df68e12ca9bd49320ec2a301
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798427"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignmentRequests = await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .get();

```