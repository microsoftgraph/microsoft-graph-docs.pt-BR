---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67744a98619020efb2f65bfe4a791aa33422b130
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .get();

```