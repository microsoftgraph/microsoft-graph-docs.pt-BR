---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9599a0c0d7b015e0f6c5c8399b60f0b2ff72a894
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/favoritePlans')
    .version('beta')
    .get();

```