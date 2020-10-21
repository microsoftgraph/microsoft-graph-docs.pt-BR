---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 586925743f98706667483bd2a4a39c91d447a3be
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedObjects')
    .get();

```