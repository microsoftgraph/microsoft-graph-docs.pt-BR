---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d952b1f0cbde3504b85df85b141a724fb012f48b
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  accessPackageId: "56ff43fd-6b05-48df-9634-956a777fce6d",
  displayName: "direct",
  description: "direct assignments by administrator",
  accessReviewSettings: null,
  requestorSettings: {
    scopeType: "NoSubjects",
    acceptRequests: true,
    allowedRequestors: []
  },
  requestApprovalSettings: {
    isApprovalRequired: false,
    isApprovalRequiredForExtension: false,
    isRequestorJustificationRequired: false,
    approvalMode: "NoApproval",
    approvalStages: []
  }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```