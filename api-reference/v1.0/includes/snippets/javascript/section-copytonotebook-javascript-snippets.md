---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b712cd0beadf417b7cbf6db87c8bb0767fd20a11
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/sections/{id}/copyToNotebook')
    .post(onenoteOperation);

```