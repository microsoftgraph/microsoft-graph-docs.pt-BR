---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae1ae23d15764edb6fbdaccdbce368fc9a8ab697
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/deviceImages/{id}')
    .version('beta')
    .get();

```