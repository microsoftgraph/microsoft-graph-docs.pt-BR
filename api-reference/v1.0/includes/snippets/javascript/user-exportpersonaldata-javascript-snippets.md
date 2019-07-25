---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d86c65a0187562659ef7f77ae12c8dba0829945
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: "storageLocation-value"
};

let res = await client.api('/users/{id}/exportPersonalData')
    .post(exportPersonalData);

```