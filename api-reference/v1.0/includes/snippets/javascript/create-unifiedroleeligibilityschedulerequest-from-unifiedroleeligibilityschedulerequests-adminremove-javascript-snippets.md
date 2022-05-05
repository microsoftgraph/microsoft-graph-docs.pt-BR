---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 133bfa62bd8c74e83935a84ba33069a65480acc5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleEligibilityScheduleRequest = {
    action: 'adminRemove',
    roleDefinitionId: '8424c6f0-a189-499e-bbd0-26c1753c96d4',
    directoryScopeId: '/',
    principalId: '071cc716-8147-4397-a5ba-b2105951cc0b'
};

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .version('beta')
    .post(unifiedRoleEligibilityScheduleRequest);

```