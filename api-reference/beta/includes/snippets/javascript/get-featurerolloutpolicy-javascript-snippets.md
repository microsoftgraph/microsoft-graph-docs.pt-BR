---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 647980c58407442f0f87cd3d45c6c7faac27aefa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .version('beta')
    .expand('appliesTo')
    .get();

```