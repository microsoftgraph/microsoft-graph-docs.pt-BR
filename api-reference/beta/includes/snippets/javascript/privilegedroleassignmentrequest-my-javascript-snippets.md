---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 154c50fa23678aa992da41ea73ab0c8e42bcc2a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let my = await client.api('/privilegedRoleAssignmentRequests/my')
    .version('beta')
    .get();

```