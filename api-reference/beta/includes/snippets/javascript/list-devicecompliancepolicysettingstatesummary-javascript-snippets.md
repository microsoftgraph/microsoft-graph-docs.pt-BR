---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630850e89dbb5a0ec628e0aa434ed10ea583d723
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceCompliancePolicySettingStateSummaries = await client.api('/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummaries')
    .version('beta')
    .get();

```