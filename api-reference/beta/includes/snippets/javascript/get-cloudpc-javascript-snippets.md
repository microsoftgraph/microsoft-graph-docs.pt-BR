---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd8bffdc0b6f59ee9e2941d56378cd2990a3093c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/cloudPCs/{id}')
    .version('beta')
    .get();

```