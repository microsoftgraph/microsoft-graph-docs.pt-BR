---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2895c7ce220670b1be1785c59357a92c62125603710756dcf570986c66e53dc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcProvisioningPolicy = {
  '@odata.type': '#microsoft.graph.cloudPcProvisioningPolicy',
  displayName: 'Display Name value',
  description: 'Description value',
  onPremisesConnectionId: '6bf90392-5fea-459a-9e9d-a2484abbffff',
  imageId: 'Image ID value',
  imageDisplayName: 'Image Display Name value',
  imageType: 'gallery'
};

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .post(cloudPcProvisioningPolicy);

```