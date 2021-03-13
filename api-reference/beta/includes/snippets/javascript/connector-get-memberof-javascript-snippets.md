---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ede2a32a3d2896a11bcf4d7b4f8d0dc1f7b45304
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf')
    .version('beta')
    .get();

```