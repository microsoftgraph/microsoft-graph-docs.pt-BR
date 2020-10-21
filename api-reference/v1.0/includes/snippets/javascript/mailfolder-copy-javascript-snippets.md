---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddd65f5a006f7894b8dd3c67f737a9a9542b5f0f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616863"
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
    .post(mailFolder);

```