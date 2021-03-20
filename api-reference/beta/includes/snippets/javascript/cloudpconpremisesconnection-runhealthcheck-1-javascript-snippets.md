---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af47112a8a4017c8e7f53f0b675d209ec03ba91d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision')
    .version('beta')
    .post();

```