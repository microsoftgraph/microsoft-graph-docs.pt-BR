---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7276630f4a176a34220e4c85d55941dbd55cb302
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conditionalAccessPolicy = {
    displayName: 'Access to EXO requires MFA',
    state: 'enabled',
    conditions: {
        clientAppTypes: [
            'mobileAppsAndDesktopClients',
            'browser'
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
                'All'
            ],
            excludeLocations: [
                'AllTrusted'
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
    .post(conditionalAccessPolicy);

```