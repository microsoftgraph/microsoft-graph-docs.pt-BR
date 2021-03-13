---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea601d54e4f1ad1fe501986d8253f434808d63ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentOrder = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder')
    .version('beta')
    .get();

```