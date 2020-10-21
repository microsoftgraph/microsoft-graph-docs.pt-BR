---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2899d5e46380611c0f266d35e0cc4d198289795b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/{object-id}/restore')
    .post();

```