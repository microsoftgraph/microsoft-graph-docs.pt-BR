---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbccdcdd25ab414794ef1b0aea4e776edd398cb0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: 'textBox'
};

await client.api('/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}')
    .update(identityUserFlowAttributeAssignment);

```