---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f182b649a5eb3c07b20eaa1869b0247e76b3f81
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59998124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
    description: 'Group assignable to a role',
    displayName: 'Role assignable group',
    groupTypes: [
        'Unified'
    ],
    isAssignableToRole: true,
    mailEnabled: true,
    securityEnabled: true,
    mailNickname: 'contosohelpdeskadministrators',
    'owners@odata.bind': [
        'https://graph.microsoft.com/v1.0/users/99e44b05-c10b-4e95-a523-e2732bbaba1e'
    ],
    'members@odata.bind': [
        'https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0',
        'https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e'
    ]
};

await client.api('/groups')
    .post(group);

```