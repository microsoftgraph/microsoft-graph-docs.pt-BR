---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b389c27441502a3377ff5d26d343f39b0e49d838
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings')
    .get();

```