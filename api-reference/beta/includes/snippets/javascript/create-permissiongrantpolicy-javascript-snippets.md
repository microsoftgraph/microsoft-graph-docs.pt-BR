---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b3e3610e16783995029413b1e2747e867c11b4597cfca11b7b077ddd9e62a57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  id: 'my-custom-consent-policy',
  displayName: 'Custom application consent policy',
  description: 'A custom permission grant policy to customize conditions for granting consent.'
};

await client.api('/policies/permissionGrantPolicies')
    .version('beta')
    .post(permissionGrantPolicy);

```