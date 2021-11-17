---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4cd3c44730f6b648184dc71c1a3ebf6895e30e89fafb780755d7c6e7be31c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managedDeviceComplianceTrend = await client.api('/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}')
    .version('beta')
    .get();

```