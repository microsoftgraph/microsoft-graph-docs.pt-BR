---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92701daf99351040b40e57026cdb560515764e86
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5')
    .version('beta')
    .delete();

```