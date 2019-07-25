---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4bb85e0eed7e0d62609ac8ba5b64e6887011a48
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredUsers')
    .version('beta')
    .get();

```