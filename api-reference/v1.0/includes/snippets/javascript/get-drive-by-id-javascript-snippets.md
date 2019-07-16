---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43915ed94ba5ba944e634d99c31a084fe76935b9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}')
    .get();

```