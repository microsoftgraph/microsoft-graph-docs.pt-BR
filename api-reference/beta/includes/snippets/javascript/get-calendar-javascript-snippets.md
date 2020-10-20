---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b2893395be79e6c0c4c7af22e2782f37b8524bb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603770"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .get();

```