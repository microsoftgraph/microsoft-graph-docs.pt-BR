---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b0e601dfc2637114e9352fb46dbbd4ff917fb0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/sharedWithMe')
    .version('beta')
    .get();

```