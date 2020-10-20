---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ba7f9c70f6c802000ab048a1b11c90e7f546fee
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .delete();

```