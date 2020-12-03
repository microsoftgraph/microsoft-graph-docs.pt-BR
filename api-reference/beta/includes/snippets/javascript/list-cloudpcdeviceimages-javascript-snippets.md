---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf4d01dea5e0570909989ff0d3ee9171b3374d9e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .get();

```