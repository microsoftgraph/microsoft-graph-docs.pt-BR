---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d66f0a0769358341058c14a9a568e64d3657ede
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  displayName: "Custom permission grant policy"
};

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .update(permissionGrantPolicy);

```