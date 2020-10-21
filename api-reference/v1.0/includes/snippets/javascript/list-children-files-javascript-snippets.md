---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9a3a1f6423a29dfcafe0969eb7785c78d310620
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .get();

```