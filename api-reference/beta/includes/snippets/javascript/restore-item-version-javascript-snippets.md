---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81efc74f2adbc8c5acb7df5d48caf18108df8d0d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .version('beta')
    .post();

```