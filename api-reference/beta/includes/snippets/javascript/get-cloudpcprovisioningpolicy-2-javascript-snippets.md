---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8536bc5313b45a6e7cc6928de22911fa8d59dc02a8d5c4ebe34c8b76136c0ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcProvisioningPolicy = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .expand('assignments')
    .get();

```