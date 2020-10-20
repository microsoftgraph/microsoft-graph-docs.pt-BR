---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfeab76fee4f086cc4dd5759c4b487418905349c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads')
    .version('beta')
    .get();

```