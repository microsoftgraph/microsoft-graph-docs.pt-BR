---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 158d7cd555452e5f9de5d5080493e0be04bcdd82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/deviceImages/{id}')
    .version('beta')
    .delete();

```