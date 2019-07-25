---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24c83fcd169859ca77526cd97505af3b38c90abb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/transitiveMemberOf')
    .get();

```