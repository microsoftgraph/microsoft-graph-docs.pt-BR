---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 822e68d23922cbda2154ac84a21a9f89b27169bf
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522607"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .get();

```