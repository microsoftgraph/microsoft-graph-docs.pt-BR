---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 219424553fb67656c616992ad79fbfd43aaeca12
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value"
};

let res = await client.api('/me/onenote/pages/{id}/copyToSection')
    .post(onenoteOperation);

```