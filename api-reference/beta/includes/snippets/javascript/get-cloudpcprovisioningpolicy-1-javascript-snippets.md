---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01dc06e483c20589fd0634f190bba8866013baf198ceb17e4b6efd0a1dc9a8ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcProvisioningPolicy = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .get();

```