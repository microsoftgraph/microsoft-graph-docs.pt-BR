---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da2414ec62fc8a4752e33c4d810e5da965a99d58
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .get();

```