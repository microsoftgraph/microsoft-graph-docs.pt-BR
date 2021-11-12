---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57bfe523a9813bdcc67230724025c6c5de6e99516a9d985d757f08a6dd79415
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159569"
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