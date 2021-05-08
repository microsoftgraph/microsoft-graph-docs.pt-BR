---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5c1312931b1bd792d56097bf68fa1bf15747280
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updateAudienceById = {
  memberEntityType: 'String',
  addMembers: [
    'String'
  ],
  removeMembers: [
    'String'
  ],
  addExclusions: [
    'String'
  ],
  removeExclusions: [
    'String'
  ]
};

await client.api('/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById')
    .version('beta')
    .post(updateAudienceById);

```