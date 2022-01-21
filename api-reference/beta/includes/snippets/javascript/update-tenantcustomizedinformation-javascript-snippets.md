---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f2dac25d0113aa19e56cddbb35644e6f5f398ae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantCustomizedInformation = {
  '@odata.type': '#microsoft.graph.managedTenants.tenantCustomizedInformation',
  tenantId: 'String',
  contacts: [
    {
      '@odata.type': 'microsoft.graph.managedTenants.tenantContactInformation',
      name: 'String',
      title: 'String',
      email: 'String',
      phone: 'String',
      notes: 'String'
    }
  ],
  website: 'String'
};

await client.api('/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}')
    .version('beta')
    .update(tenantCustomizedInformation);

```