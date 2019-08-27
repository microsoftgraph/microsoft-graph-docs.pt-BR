---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 255904f4500b7ba27d9904214ef191b1bc6d99fd
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: "Demo provisioning (updated)"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d')
    .version('beta')
    .update(publishedResource);

```