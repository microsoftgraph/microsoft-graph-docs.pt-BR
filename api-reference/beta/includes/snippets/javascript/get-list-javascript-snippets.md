---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0780a954208438e9fd60076f510ae345bb825709
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}')
    .version('beta')
    .get();

```