---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c54a8e0db5e0858158e46fc9dde725c13723ea88
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Require MFA to EXO from non-complaint devices.',
    state: 'enabled',
    conditions: {
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
        },
        devices: {
            includeDevices: [
                'All'
            ],
            excludeDevices: [
                'Compliant'
            ]
        }
    },
    grantControls: {
        operator: 'OR',
        builtInControls: [
            'mfa'
        ]
    }
};

await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .post(conditionalAccessPolicy);

```