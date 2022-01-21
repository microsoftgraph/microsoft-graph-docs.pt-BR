---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d928eb4754b1fe1b1d6886e3e60b18504692dee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
  displayName: 'HR provisioning policy',
  description: 'Provisioning policy for India HR employees',
  onPremisesConnectionId: '4e47d0f6-6f77-44f0-8893-c0fe1701b553'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .update(cloudPcProvisioningPolicy);

```