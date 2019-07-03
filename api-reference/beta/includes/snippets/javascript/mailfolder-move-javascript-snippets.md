---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2efcbf125863b0e5120bf22048cfd8a7d2b327ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/move')
    .version('beta')
    .post(mailFolder);

```