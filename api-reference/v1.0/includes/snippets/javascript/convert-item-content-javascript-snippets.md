---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85433c1b5affc0c799315890f274d01a884a2f78
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/content?format=%7Bformat%7D')
    .get();

```