---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35f669d6d339991e5c224bf652f800faae7ac5ae
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/onlineMeetings/{id}')
    .version('beta')
    .get();

```