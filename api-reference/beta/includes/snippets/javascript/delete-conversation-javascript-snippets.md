---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94abda46b1c90e3db189126e51dc315265c9be51
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .delete();

```