---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462b6fe2c91155e0a849710e8da766385b52ca26
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```