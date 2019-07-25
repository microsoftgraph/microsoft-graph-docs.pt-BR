---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 195be5614c6a364c4b2d474280847d70b7f491c0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/copy')
    .version('beta')
    .post(mailFolder);

```