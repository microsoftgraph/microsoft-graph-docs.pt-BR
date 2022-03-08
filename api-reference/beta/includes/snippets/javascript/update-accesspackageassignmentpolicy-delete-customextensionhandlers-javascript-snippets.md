---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78bdd39b1dfa24a5a546de97f78c48ec887f667e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63332977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
    id: '4540a08f-8ab5-43f6-a923-015275799197',
    displayName: 'policy with custom access package workflow extension',
    description: 'Run specified custom access package workflow extension at different stages.',
    accessPackageId: 'ba5807c7-2aa9-4c8a-907e-4a17ee587500',
    expiration: {
        type: 'afterDuration',
        duration: 'P365D'
    },
    requestApprovalSettings: null,
    requestorSettings: {
        acceptRequests: true,
        scopeType: 'AllExistingDirectorySubjects',
        allowedRequestors: []
    },
    accessReviewSettings: null,
    customExtensionHandlers: []
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197')
    .version('beta')
    .put(accessPackageAssignmentPolicy);

```