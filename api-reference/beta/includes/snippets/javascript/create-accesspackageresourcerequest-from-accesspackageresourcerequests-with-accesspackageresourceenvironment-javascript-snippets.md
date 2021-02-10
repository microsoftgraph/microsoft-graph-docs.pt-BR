---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b77bc941d502b77192c2165726e78c6031b4b57
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRequest = {
    catalogId: "de9315c1-272b-4905-924b-cc112ca180c7",
    accessPackageResource: {
        displayName: "Community Outreach",
        description: "https://contoso.sharepoint.com/sites/CSR",
        resourceType: "SharePoint Online Site",
        originId: "https://contoso.sharepoint.com/sites/CSR",
        originSystem: "SharePointOnline",
        accessPackageResourceEnvironment@odata.bind: "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57"
    },
    requestType: "AdminAdd"
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .post(accessPackageResourceRequest);

```