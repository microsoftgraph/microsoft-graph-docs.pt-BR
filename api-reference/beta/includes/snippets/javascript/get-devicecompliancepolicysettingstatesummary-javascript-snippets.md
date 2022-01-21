---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7bad35fba6145ffd1e7bb64c1497b978f9f4270
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceCompliancePolicySettingStateSummary = await client.api('/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}')
    .version('beta')
    .get();

```