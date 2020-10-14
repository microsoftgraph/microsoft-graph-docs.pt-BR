---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f33fedcdcabafbd0d8ceff8ef653b8966b692659
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459606"
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
    .version('beta')
    .update(permissionGrantPolicy);

```