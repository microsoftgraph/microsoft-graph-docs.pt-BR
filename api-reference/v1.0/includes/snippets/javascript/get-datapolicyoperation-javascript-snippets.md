---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ee7a15fdbca1cabe3228a998a99ef5611eb2e7f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/dataPolicyOperations/{id}')
    .get();

```