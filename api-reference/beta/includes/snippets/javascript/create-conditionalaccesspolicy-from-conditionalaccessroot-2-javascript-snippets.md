---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98d4fafa41c954e034468d85a1c93a347ce6cb29
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Block access to EXO non-trusted regions.',
    state: 'enabled',
    conditions: {
        clientAppTypes: [
            'all'
        ],
        applications: {
            includeApplications: [
                '00000002-0000-0ff1-ce00-000000000000'
            ]
        },
        users: {
            includeGroups: ['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba']
        },
        locations: {
            includeLocations: [
                '198ad66e-87b3-4157-85a3-8a7b51794ee9'
            ]
        }
    },
    grantControls: {
        operator: 'OR',
        builtInControls: [
            'block'
        ]
    }
};

await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .post(conditionalAccessPolicy);

```