---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 647980c58407442f0f87cd3d45c6c7faac27aefa
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201386"
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