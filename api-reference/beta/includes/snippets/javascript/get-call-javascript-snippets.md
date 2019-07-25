---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebcc192d9edb2fd9a611c70290be363e9f661eb5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}')
    .version('beta')
    .get();

```